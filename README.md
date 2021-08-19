# javscript-one-line-helpers
Awesome JavaScript One-Liners Utilities for Daily Usage

## Generate a Random Boolean
We know that Math.random returns a value between 0 and 1. We can use that knowledge to create a very simple boolean generator.

```
const randomBoolean = () => Math.random() >= 0.5;
```

## Generate a Random Number
We will take advantage of the Math.random API once more. By multiplying the result by our max number and rounding it. We then will obtain a number between 0 and max.

```
const randomNumber = (max) => Math.round(Math.random() * max);
```

It is simple to extend this method further to accept min and max ranges.

```
const randomNumber = (min, max) => Math.round(Math.random() * (max - min) + min);
```

## Generate a Random ID
For generating this utility we will rely on the toString method. It will let us convert our random numbers to strings.

```
const randomId = () => Math.random().toString(36).substring(2);
```

To be continued...
