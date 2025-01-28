# Count-Partitions-With-Even-Sum-Difference


Problem Description : 

You are given an integer array nums of length n. A partition is defined as an index i where 0 <= i < n - 1, splitting the array into two non-empty subarrays such that:
The left subarray contains indices [0, i].
The right subarray contains indices [i + 1, n - 1].
Your task is to count the number of partitions where the difference between the sum of the left and right subarrays is even.

Algorithm :

Calculate the Total Sum: Start by calculating the total sum of the array.
Iterate Over Possible Partitions:
Maintain a running sum for the left subarray.
Calculate the right subarray sum as total_sum - left_sum.
Check if the difference (left_sum - right_sum) is even.
Count Valid Partitions: Increment the count whenever the difference is even.

Key Observations :

A number is even if it is divisible by 2.
The difference between two sums is even if both sums are either even or odd.

Complexity :

Time Complexity: O(n) since we iterate through the array once.
Space Complexity: O(1) as no extra space is used other than variables.
