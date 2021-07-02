def spiralPrint(matrix):
  left = 0
  right = len(matrix[0])
  bottom =len(matrix) 
  top =0
  direction = 0
  
  while(left<right and bottom>top):
      
    if direction == 0:
      for i in range(left, right):
        print(matrix[top][i])
      top+=1
      direction = 1

    if direction == 1:
      for i in range(top, bottom):
        print(matrix[i][right-1])
      right-=1
      direction = 2

    if direction == 2:
      for i in range(right, left, -1):
        print(matrix[bottom-1][i-1])
      bottom -=1
      direction = 3

    if direction == 3:
      for i in range(bottom, top, -1):
        print(matrix[i-1][left])
      left +=1
      direction = 0


matrix = [
  [1,2,3], 
  [4,5,6], 
  [7,8,9],
  [10,11,12]
  ]

spiralPrint(matrix)
