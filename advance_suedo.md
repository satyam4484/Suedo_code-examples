
### **Debugging Questions in Pseudocode**

1. **Question 1:**
   ```pseudocode
   function findMax(arr: array of integers)
       max = arr[0]
       for i = 1 to length(arr)
           if arr[i] > max then
               max = arr[i]
       end for
       return max
   end function
   ```

2. **Question 2:**
   ```pseudocode
   function isPalindrome(str: string)
       left = 0
       right = length(str) - 1
       while left < right
           if str[left] != str[right] then
               return false
           left = left + 1
           right = right - 1
       end while
       return true
   end function
   ```

3. **Question 3:**
   ```pseudocode
   function calculateAverage(arr: array of integers)
       sum = 0
       for i = 0 to length(arr)
           sum = sum + arr[i]
       end for
       return sum / length(arr)
   end function
   ```

4. **Question 4:**
   ```pseudocode
   function countVowels(str: string)
       vowels = "aeiou"
       count = 0
       for i = 0 to length(str)
           if str[i] in vowels then
               count = count + 1
       end for
       return count
   end function
   ```

5. **Question 5:**
   ```pseudocode
   function bubbleSort(arr: array of integers)
       for i = 0 to length(arr) - 1
           for j = 0 to length(arr) - i
               if arr[j] > arr[j + 1] then
                   swap(arr[j], arr[j + 1])
       end for
       return arr
   end function
   ```

6. **Question 6:**
   ```pseudocode
   function factorial(n: integer)
       if n < 0 then
           return 0
       if n == 0 then
           return 1
       else
           return n * factorial(n - 1)
       end if
   end function
   ```

7. **Question 7:**
   ```pseudocode
   function mergeArrays(arr1: array of integers, arr2: array of integers)
       merged = []
       for i = 0 to length(arr1) + length(arr2)
           if i < length(arr1) then
               merged[i] = arr1[i]
           else
               merged[i] = arr2[i - length(arr1)]
       end for
       return merged
   end function
   ```

8. **Question 8:**
   ```pseudocode
   function fibonacci(n: integer)
       a = 0
       b = 1
       for i = 0 to n
           c = a + b
           a = b
           b = c
       end for
       return a
   end function
   ```

9. **Question 9:**
   ```pseudocode
   function reverseString(str: string)
       reversed = ""
       for i = length(str) to 0
           reversed = reversed + str[i]
       end for
       return reversed
   end function
   ```

10. **Question 10:**
    ```pseudocode
    function findSecondLargest(arr: array of integers)
        first = second = -infinity
        for i = 0 to length(arr)
            if arr[i] > first then
                second = first
                first = arr[i]
            else if arr[i] > second and arr[i] != first then
                second = arr[i]
        end for
        return second
    end function
    ```

11. **Question 11:**
    ```pseudocode
    function power(base: integer, exp: integer)
        result = 1
        for i = 0 to exp
            result = result * base
        end for
        return result
    end function
    ```

12. **Question 12:**
    ```pseudocode
    function removeDuplicates(arr: array of integers)
        unique = []
        for i = 0 to length(arr)
            if arr[i] not in unique then
                unique.append(arr[i])
        end for
        return unique
    end function
    ```

13. **Question 13:**
    ```pseudocode
    function countWords(str: string)
        words = split(str, " ")
        return length(words)
    end function
    ```

14. **Question 14:**
    ```pseudocode
    function maxDifference(arr: array of integers)
        minVal = arr[0]
        maxDiff = 0
        for i = 1 to length(arr)
            if arr[i] < minVal then
                minVal = arr[i]
            else
                diff = arr[i] - minVal
                if diff > maxDiff then
                    maxDiff = diff
        end for
        return maxDiff
    end function
    ```

15. **Question 15:**
    ```pseudocode
    function rotateArray(arr: array of integers, k: integer)
        k = k % length(arr)
        temp = []
        for i = 0 to length(arr)
            temp[(i + k) % length(arr)] = arr[i]
        end for
        return temp
    end function
    ```

16. **Question 16:**
    ```pseudocode
    function longestSubstring(str: string)
        maxLength = 0
        currentLength = 0
        for i = 0 to length(str)
            if str[i] not in str[0:i] then
                currentLength = currentLength + 1
            else
                maxLength = max(maxLength, currentLength)
                currentLength = 1
        end for
        return max(maxLength, currentLength)
    end function
    ```

17. **Question 17:**
    ```pseudocode
    function countOccurrences(arr: array of integers, target: integer)
        count = 0
        for i = 0 to length(arr)
            if arr[i] == target then
                count = count + 1
        end for
        return count
    end function
    ```

18. **Question 18:**
    ```pseudocode
    function areAnagrams(str1: string, str2: string)
        sort(str1)
        sort(str2)
        return str1 == str2
    end function
    ```

19. **Question 19:**
    ```pseudocode
    function flattenArray(arr: array of arrays)
        flat = []
        for subArray in arr
            for element in subArray
                flat.append(element)
        end for
        return flat
    end function
    ```

20. **Question 20:**
    ```pseudocode
    function findMissingNumber(arr: array of integers, n: integer)
        totalSum = n * (n + 1) / 2
        arrSum = 0
        for i = 0 to length(arr)
            arrSum = arrSum + arr[i]
        end for
        return totalSum - arrSum
    end function
    ```

21. **Question 21:**
    ```pseudocode
    function uniqueCharacters(str: string)
        charSet = {}
        for i = 0 to length(str)
            if str[i] in charSet then
                return false
            charSet.add(str[i])
        end for
        return true
    end function
    ```

22. **Question 22:**
    ```pseudocode
    function isValidParentheses(str: string)
        stack = []
        for char in str
            if char == "(" then
                stack.push(char)
            else if char == ")" then
                if stack is empty then
                    return false
                stack.pop()
        end for
        return stack is empty
    end function
    ```

23. **Question 23:**
    ```pseudocode
    function calculateGCD(a: integer, b: integer)
        while b != 0
            temp = b
            b = a % b
            a = temp
        end while
        return a
    end function
    ```

24. **Question 24:**
    ```pseudocode
    function flattenDictionary(dict: dictionary)
        flat = []
        for key, value in dict
            flat.append(key + ": " + value)
        end for
        return flat
    end function
    ```

25. **Question 25:**
    ```pseudocode
    function countPrimes(n: integer)
        count = 0
        for i = 2 to n
            isPrime = true
            for j = 2 to sqrt(i)
                if i % j == 0 then
                    isPrime = false
            end for
            if isPrime then
                count = count + 1
        end for
        return count
    end function
    ```

26. **Question 26:**
    ```pseudocode
    function longestCommonPrefix(strs: array of strings)
        if length(strs) == 0 then
            return ""
        prefix = strs[0]
        for i = 1 to length(strs)
            while strs[i].startsWith(prefix) is false
                prefix = prefix.substring(0, length(prefix) - 1)
        end for
        return prefix
    end function
    ```

27. **Question 27:**
    ```pseudocode
    function stringCompression(str: string)
        compressed = ""
        count = 1
        for i = 1 to length(str)
            if str[i] == str[i - 1] then
                count = count + 1
            else
                compressed = compressed + str[i - 1] + count
                count = 1
        end for
        return compressed + str[length(str) - 1] + count
    end function
    ```

28. **Question 28:**
    ```pseudocode
    function sumDigits(n: integer)
        sum = 0
        while n > 0
            sum = sum + (n % 10)
            n = n // 10
        end while
        return sum
    end function
    ```

29. **Question 29:**
    ```pseudocode
    function rotateMatrix(matrix: array of arrays)
        n = length(matrix)
        for i = 0 to n / 2
            for j = i to n - i - 1
                temp = matrix[i][j]
                matrix[i][j] = matrix[n - j - 1][i]
                matrix[n - j - 1][i] = matrix[n - i - 1][n - j - 1]
                matrix[n - i - 1][n - j - 1] = matrix[j][n - i - 1]
                matrix[j][n - i - 1] = temp
        end for
        return matrix
    end function
    ```

30. **Question 30:**
    ```pseudocode
    function binarySearch(arr: array of integers, target: integer)
        left = 0
        right = length(arr) - 1
        while left <= right
            mid = (left + right) / 2
            if arr[mid] == target then
                return mid
            else if arr[mid] < target then
                left = mid + 1
            else
                right = mid - 1
        end while
        return -1
    end function
    ```

31. **Question 31:**
    ```pseudocode
    function longestIncreasingSubsequence(arr: array of integers)
        n = length(arr)
        lis = array of size n filled with 1
        for i = 1 to n
            for j = 0 to i - 1
                if arr[i] > arr[j] then
                    lis[i] = max(lis[i], lis[j] + 1)
        end for
        return max(lis)
    end function
    ```

32. **Question 32:**
    ```pseudocode
    function getIntersection(arr1: array of integers, arr2: array of integers)
        set1 = {}
        intersection = []
        for num in arr1
            set1.add(num)
        end for
        for num in arr2
            if num in set1 then
                intersection.append(num)
        end for
        return intersection
    end function
    ```

33. **Question 33:**
    ```pseudocode
    function uniquePaths(m: integer, n: integer)
        dp = array of size m x n filled with 1
        for i = 1 to m
            for j = 1 to n
                dp[i][j] = dp[i - 1][j] + dp[i][j - 1]
        end for
        return dp[m - 1][n - 1]
    end function
    ```

34. **Question 34:**
    ```pseudocode
    function backtrackCombinations(n: integer, k: integer)
        result = []
        function backtrack(start: integer, path: array of integers)
            if length(path) == k then
                result.append(path)
                return
            for i = start to n
                path.append(i)
                backtrack(i + 1, path)
                path.pop()
        end function
        backtrack(1, [])
        return result
    end function
    ```

35. **Question 35:**
    ```pseudocode
    function isSubsetSum(arr: array of integers, sum: integer)
        n = length(arr)
        dp = array of size (n + 1) x (sum + 1) filled with false
        for i = 0 to n
            dp[i][0] = true
        end for
        for i = 1 to n
            for j = 1 to sum
                if arr[i - 1] <= j then
                    dp[i][j] = dp[i - 1][j] or dp[i - 1][j - arr[i - 1]]
                else
                    dp[i][j] = dp[i - 1][j]
        end for
        return dp[n][sum]
    end function
    ```

36. **Question 36:**
    ```pseudocode
    function isValidSudoku(board: array of arrays)
        rows = {}
        cols = {}
        boxes = {}
        for i = 0 to 9
            for j = 0 to 9
                if board[i][j] != "." then
                    num = board[i][j]
                    boxIndex = (i / 3) * 3 + (j / 3)
                    if (num in rows[i]) or (num in cols[j]) or (num in boxes[boxIndex]) then
                        return false
                    rows[i].add(num)
                    cols[j].add(num)
                    boxes[boxIndex].add(num)
        end for
        return true
    end function
    ```

37. **Question 37:**
    ```pseudocode
    function numberOfIslands(grid: array of arrays)
        if grid is empty then
            return 0
        count = 0
        for i = 0 to length(grid)
            for j = 0 to length(grid[0])
                if grid[i][j] == '1' then
                    count = count + 1
                    dfs(grid, i, j)
        end for
        return count
    end function

    function dfs(grid: array of arrays, i: integer, j: integer)
        if i < 0 or j < 0 or i >= length(grid) or j >= length(grid[0]) or grid[i][j] != '1' then
            return
        grid[i][j] = '0'
        dfs(grid, i - 1, j)
        dfs(grid, i + 1, j)
        dfs(grid, i, j - 1)
        dfs(grid, i, j + 1)
    end function
    ```

38. **Question 38:**
    ```pseudocode
    function stringRotation(str1: string, str2: string)
        if length(str1) != length(str2) then
            return false
        return str1 in (str2 + str2)
    end function
    ```

39. **Question 39:**
    ```pseudocode
    function minCoins(coins: array of integers, amount: integer)
        dp = array of size amount + 1 filled with infinity
        dp[0] = 0
        for coin in coins
            for j = coin to amount
                dp[j] = min(dp[j], dp[j - coin] + 1)
        end for
        return dp[amount] if dp[amount] != infinity else -1
    end function
    ```

40. **Question 40:**
    ```pseudocode
    function permutations(s: string)
        result = []
        backtrack(s, "", result)
        return result

    function backtrack(remaining: string, path: string, result: array of strings)
        if length(remaining) == 0 then
            result.append(path)
        for i = 0 to length(remaining)
            backtrack(remaining[0:i] + remaining[i + 1:], path + remaining[i], result)
    end function
    ```
