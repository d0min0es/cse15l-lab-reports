# Lab Report 2

## Part 2: Failing Output
![Image](testreverse.jpg)
```
@Test
public void testReversed() {
int[] input1 = {1, 2, 3};
assertArrayEquals(new int[]{3, 2, 1}, ArrayEquals.reversed(input1));

}
```
### Failure-Inducing Output
- One example of a failure-inducing ouput for the `Reverse` method in `ArrayExamples.java` is the input above, `int[] input1 = {1, 2, 3}` which ends up returning an array of all 0's ( `{0, 0, 0}` ) instead of reversing the order of the elements in the provided list.

```
public void testReversed() {
int[] input2 = {0, 0, 0, 0};
assertArrayEquals(new int[]{0, 0, 0, 0}, ArrayEquals.reversed(input2));

}
```
### Non-Failure Inducing Output
- An example of an input that doesn't produce a failure would be a array list like the one given above, `int[] input2 = {0, 0, 0, 0}`

### The Symptom
-
