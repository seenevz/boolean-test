#For Loops Video Lesson

## What is expected

Assume the audience are complete beginners, although they already know about variables and arrays at this point.
Record a 30 minute lecture explaining for loops in JavaScript

## Deliverables

- What are loops and why we need them
- The basic sintax of For Loops
- For Loops and arrays
- Gotchas of using loops


## Revision

Talk briefly about how we declare and access variables and arrays. Introduce Console.log

## What are loops and why we need them

Talk about the need of execute a set of instructions a repeated amount of times a.k.a iteration

There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times.

Programatically repeat a task

## The basic sintax of For Loops

```js
for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statementBlock
```

The loop runs in the following order:

  1. *initialExpression* happens; This is where we gonna initialise vars like counters, but in truth we can run more complex expressions here

  2. *conditionalExpression* is evaluated; This expression has to be either `true` or `false`; This is going to determine if the loop will continue to
  run or immediately terminate

  3. *statementBlock* is executed; here we have the statement/s that we want to repeatedly run

  4. *incrementExpression* runs; in here we have an expression that runs after so we can do things like update our counters

  5. And now we are looping back to step 2, where we gonna rinse and repeat the steps!


## Gotchas of using loops

The main gotcha we need to be careful with are infinite loops. These can happen for different reasons, such as never reaching conditional Statement,
not updating the counters, or some flawed logic that interact with these.

We can also use for loops without all 3 expressions in its statement; In this case we also need to be careful we don't end up in an infinite loop

Talk about `if statements` and `brake` statements

```
no initialization
var i = 0;
for (; i < 9; i++) {
    console.log(i);
    // more statements
}

no condition
for (let i = 0;; i++) {
   console.log(i);
   if (i > 3) break;
   // more statements
}

no increment
var i = 0;
for (;;) {
  if (i > 3) break;
  console.log(i);
  i++;
}

```

## For loops and arrays

We can access any element in an array through its index; Im this way we can use the index notation and the counter of a loop to iterate over an array;
This way we have a programmatic way of accessing and operating in every element of an array.


```
arr = []

for (let i = 0; i < 9; ++i) arr[i] = i
```
