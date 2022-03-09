**COVERAGE Improvement**

With white-box testing setting, we had access to the source-code to be tested. We monitored the source codes and assessed the coverage to see which statements or branches are missed by our previous test suites. Accordingly, we designed some new tests to cover the missed parts in this assignment. Method-wise details for the new test cases design are as follows.

1. **Class DataUtilitites**

**1.1. calculateColumnTotal()**

**1.1.1. calculateColumnTotalTest\_LastColumnWithANullElement()**

- **Description:** We previously missed a branch where every element of the array is checked to see whether it is null or not. In assignment-2, we did not have any test/input data to check that condition. So our branch coverage and condition coverage were not 100% for this method.

In this assignment, we modified our test input slightly by adding null element in the input array as follow.

Previous mocked Valued2D Array (Assignment-2):

7.5 5.5 4.5

2.5 -10.5 1.0

3.5 1.5 6.5

New mocked Valued2D Array (Assignment-3):

7.5 5.5 4.5

2.5 -10.5 1.0

3.5 1.5 **null**

We modified the mocking implementation as follows.

![](RackMultipart20220309-4-10nyl4x_html_27a83a0ae6bdebc0.png)

Hence, our previous test case, where we were testing the sum of the last column, now is capable to cover the previously missed condition. We renamed the test from &quot;calculateColumnTotalTest\_LastColumn&quot; to &quot;calculateColumnTotalTest\_LastColumnWithANullElement&quot;. The test case is as below:

![](RackMultipart20220309-4-10nyl4x_html_399c7d650cf2586d.png)

After that, the condition and branch coverage for this method hit 100%.

- **Input:** 4.5 + 1 + null
- **Expected Output:** 5.5
- **Test Result:** Pass

**1.2. calculateRowTotal()**

**1.1.1. calculateColumnTotalTest\_LastRowWithANullElement()**

- We previously missed a branch where every element of the array is checked to see whether it is null or not. In assignment-2, we did not have any test/input data to check that condition. So our branch coverage and condition coverage was not 100% for this method.

In this assignment, we modified our test input slightly by adding null element in the input array as follow.

Previous mocked Valued2D Array (Assignment-2):

7.5 5.5 4.5

2.5 -10.5 1.0

3.5 1.5 6.5

New mocked Valued2D Array (Assignment-3):

7.5 5.5 4.5

2.5 -10.5 1.0

3.5 1.5 **null**

We modified the mocking implementation as follows.

![](RackMultipart20220309-4-10nyl4x_html_27a83a0ae6bdebc0.png)

Hence, our previous test case, where we were testing the sum of the last row, now is capable to cover the previously missed condition. We renamed the test from &quot;calculateRowTotalTest\_LastColumn&quot; to &quot;calculateRowTotalTest\_LastColumnWithANullElement&quot;. The test case is as below:

![](RackMultipart20220309-4-10nyl4x_html_23b2ecf1ec6dedd7.png)

After that, the condition and branch coverage for this method hit 100%.

- **Input:** 1.5 + 3.5 + null
- **Expected Output:** 5.0
- **Test Result:** Pass

1.3.
