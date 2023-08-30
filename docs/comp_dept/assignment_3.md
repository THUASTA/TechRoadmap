# Assignment 3: Python Practices

## Goals

- Write simple python code

## Q1: Vector And Matrix Class

Write a vector and matrix operation class in python. Be careful not to use scientific computing libraries such as numpy. You need to use python `list` to complete, that is, one-dimensional lists represent vectors, and two-dimensional lists represent matrices.We assume that the input parameters meet the requirements and no format checking is required.And it is recommended that you write [Type Hint](https://zhuanlan.zhihu.com/p/464979921) after the parameters and write some necessary comments. 

In a vector class you need to implement the following class instance methods:

1. Constructor: The parameters are `self` and a list
2. Vector addition: the parameter is `self` and another vector
3. Vector inner product: The parameter is `self` and another vector, and returns a float value
4. Vector element-wise multiplication: The parameters are `self` and another vector, and a new vector is returned

In the Matrix class you need to implement the following class instance methods:

1. Constructor: The parameters are `self` and a list
2. Matrix addition: the parameters are `self` and another matrix
3. Matrix multiplication: The parameters are `self` and another matrix, and a new matrix is returned
4. Matrix element-wise multiplication: the parameters are `self` and another matrix, and a new matrix is returned
5. (Optional) Matrix determinant: the parameter is `self`, return a float value

You can write some other codes to check if the method in class is right.

You should finish your work by September 6th. Once you have completed all the questions, please submit your work to Tsinghua Cloud, uploading them to the folder named after their name in Tsinghua Cloud (e.g. `ASTA2023/部门/竞赛部/技术培训/作业三/张三/xxx.py`). If the folder does not exist, please create one.