python

下載python
安裝Python 2.7==>裝在D:\python2
 
使用gedit寫程式   檔名aaa.py

輸入:input        函數從標準輸入讀取一個行，並返回一個字串
但是 input 可以接收一個Python運算式作為輸入，並將運算結果返回。

#!/usr/bin/env python
#coding=utf-8

 radius = 20 # radius is now 20
 Prompt the user to enter a radius
radius = eval(input("Enter a number for radius: "))

 Compute area
area = radius * radius * 3.14159

 Display results
print("The area for the circle of radius", radius, "is", area)



同時指定(Simultaneous Assignment )
!/usr/bin/env python
coding=utf-8
 Prompt the user to enter three numbers
number1, number2, number3 = eval(input(
  "Enter three numbers separated by commas: "))

 Compute average
average = (number1 + number2 + number3) / 3

 Display result
print("The average of", number1, number2, number3,
    "is", average)
    
輸出:print
>>> q = 259
>>> p = 0.038
>>> print(q, p, p * q)
>>> print(q, p, p * q, sep=",")
>>> print(q, p, p * q, sep=" :-) ")
>>> print(str(q) + " " + str(p) + " " + str(p * q))

格式化輸出:使用format()

符  號	
%c	 格式化字元及其ASCII碼
      %s	 格式化字串
      %d	 格式化整數
      %u	 格式化無符號整型
      %o	 格式化無符號八進位數
      %x	 格式化無符號十六進位數
      %X	 格式化無符號十六進位數（大寫）
      %f	 格式化浮點數字，可指定小數點後的精度
      %e	 用科學計數法格式化浮點數
      %E	 作用同%e，用科學計數法格式化浮點數
      %g	 %f和%e的簡寫
      %G	 %f 和 %E 的簡寫
      %p	 用十六進位數格式化變數的位址

運算子
#!/usr/bin/env python
#coding=utf-8

seconds = eval(input("Enter an integer for seconds: "))

minutes = seconds // 60     # Find minutes in seconds
remainingSeconds = seconds % 60   # Seconds remaining
print(seconds, "seconds is", minutes,  
  "minutes and", remainingSeconds, "seconds")
  
  各種資料型態:
  數字型   字串   列表   辭典
  
  餘數運算子
  ```
  #!/usr/bin/env python
coding=utf-8

seconds = eval(input("Enter an integer for seconds: "))
minutes = seconds // 60      Find minutes in seconds
remainingSeconds = seconds % 60   # Seconds remaining
print(seconds, "seconds is", minutes,  
"minutes and", remainingSeconds, "seconds")
------------------------------------------------
```
