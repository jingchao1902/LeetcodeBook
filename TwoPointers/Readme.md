# Overview

## Explanation

- ![must-have][must-have] means __must do__ question, that includes many key points;
- ![recommended][recommended] means __good question__, that is quite clear and enjoyable;
- ![easy][easy] means __this is easy__ for me, that there might only be no fancy things;
- ![medium][medium] means __this is medium__ for me, that there is at least one important thing;
- ![hard][hard] means __this is hard__ for me, that it's hard to code;
- ![star][star] means __how many times I've done__ for this question;
- ![freq][freq] means __this is frequently asked__ in interviews.

## Category

### Partition

- [KthLargestElement](KthLargestElement.md) ![hard][hard] ![must-have][must-have] ![star][star]
- [PartitionArray](PartitionArray.md) ![must-have][must-have]
- [SortColors](SortColors.md) ![must-have][must-have] ![hard][hard]
- [RemoveDuplicateNumbersInArray](RemoveDuplicateNumbersInArray.md) ![easy][easy]

### Two sum

- [TwoSumDataStructure](TwoSumDataStructure.md) ![must-have][must-have]
- [TwoSumInputArraySorted](TwoSumInputArraySorted.md) ![easy][easy]
- [TwoSumUniquePairs](TwoSumUniquePairs.md) ![easy][easy] ![must-have][must-have]
- [TwoSumLessThanOrEqualTo](TwoSumLessThanOrEqualTo.md) ![easy][easy]
- [TwoSumClosest](TwoSumClosest.md) ![easy][easy]
- [TwoSumDifferenceEqual](TwoSumDifferenceEqual.md) ![medium][medium]
- [3Sum](3Sum.md) ![medium][medium] ![must-have][must-have]

## Notes

- Most generally, for questions that have two or more variables, how do we do?

  NOTE: We can loop through one variable, and see how the second variable changes.

- Why can we use HashMap to reduce running time and easily solve two sum?

  Because HashMap is about reducing running time based on the value content, and this question is exactly about value sum.

- For different direction pointers, how do we choose end condition?

  It depends. If you are just move left and right pointers one step by step, then it's easier, `while(left < right)` should be sufficient. But if you are moving by multiple steps or calculating steps by yourself, then there could be more edge cases.

- What are the common tricks in array?

  1. HashMap
  1. Sort

- Why we can reduce O(n^2) to O(n) sometime?

  Because we are doing aggregation on result data. A simple example is [TwoSumLessThanOrEqualTo](TwoSumLessThanOrEqualTo.md).

[must-have]: https://jaywcjlove.github.io/sb/ico/min-bibei.svg
[recommended]: https://jaywcjlove.github.io/sb/ico/min-tuijian.svg
[easy]: https://jaywcjlove.github.io/sb/ico/min-free.svg
[medium]: https://jaywcjlove.github.io/sb/ico/min-oss.svg
[hard]: https://jaywcjlove.github.io/sb/ico/min-hot.svg
[freq]: https://jaywcjlove.github.io/sb/ico/min-app-store.svg
[star]: https://jaywcjlove.github.io/sb/star/red.svg
[star0]: https://jaywcjlove.github.io/sb/star/red0.svg
[star1]: https://jaywcjlove.github.io/sb/star/red1.svg
[star2]: https://jaywcjlove.github.io/sb/star/red2.svg
[star3]: https://jaywcjlove.github.io/sb/star/red3.svg
[star4]: https://jaywcjlove.github.io/sb/star/red4.svg
[star5]: https://jaywcjlove.github.io/sb/star/red5.svg