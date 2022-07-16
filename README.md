# Sum The Strings
Create a function that takes 2 integers in form of a string as an input, and outputs the sum (also as a string):

Example: (Input1, Input2 -->Output)

![image](https://user-images.githubusercontent.com/72622378/179363067-0c5c1f53-294c-46b8-b749-21de34fdc6c7.png)

Notes:
If either input is an empty string, consider it as zero.
Inputs and the expected output will never exceed the signed 32-bit integer limit (2^31 - 1)


# 1

    def sum_str(a, b):
        return str(int(a or 0) + int(b or 0))


# 2

    def sum_str(a, b):
        return str(int('0' + a) + int('0' + b))
        
        
# 3
    
    def sum_str(a, b):
        print(a, b)
        if a == "" or a == None: a = "0"
        if b == "" or b == None: b = "0"
        return str(int(a)+int(b))
