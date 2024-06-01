# two_sum
class Solution:
    nums = list(map(int,input().split()))   #2 1 5 3
    target = int(input())
    def two_sum(nums, target):
        prev_map = {} # val : index

        for i, n in enumerate(nums):
            diff = target - n
            if diff in prev_map:
                return [prev_map[diff], i]
            prev_map[n]=i
           
            
    print(two_sum(nums, target))
