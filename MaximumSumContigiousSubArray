import sys

def max(a, b):
  return a if a>b else b

def maxSumOfSubArray(array):
  prev_sum = 0
  current_sum = 0
  maxSum = -sys.maxsize

  for i in array:
    if i>maxSum:
      maxSum = i

    if i>0:
      current_sum+=i
    else:
      if prev_sum < current_sum:
        prev_sum = current_sum
        current_sum = 0

  if prev_sum == 0 and current_sum==0:
    print(maxSum)
  else:
    print(max(prev_sum, current_sum))
        

l = [10, -5, -7, -2, -3, -9, 4, 10]
maxSumOfSubArray(l)
