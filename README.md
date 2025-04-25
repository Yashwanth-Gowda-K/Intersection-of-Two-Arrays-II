# Intersection-of-Two-Arrays-II


Given two arrays nums1 and nums2, return their intersection, i.e., the common elements between the two arrays, considering the duplicate values as well. Each element in the result should appear as many times as it shows in both arrays.

Example:
Input:
nums1 = [4,9,5]
nums2 = [9,4,9,8,4]

Output:
[4,9]

----- > Solution Overview < -------
The approach to solving this problem is as follows:

Count the Frequency of Elements in nums1:

Use Python's Counter from the collections module to store the count of each element in nums1.

Iterate through nums2:

For each number in nums2, check if it exists in nums1 and if it’s still available (i.e., its count is greater than 0).

If so, add it to the result list and decrease the count in nums1 to ensure we only count the element as many times as it appears in nums1.

Return the Result List:

The result list contains all the common elements between nums1 and nums2 with duplicates handled correctly.

