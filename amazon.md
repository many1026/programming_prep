TWO ARRAYS SUM

def twoNumberSum(array, targetSum):
    # Write your code here.
    dict = {}
    for num in array:
        if targetSum - num in dict:
            return [targetSum - num, num]
        else:
            dict[num] = True
    return []
