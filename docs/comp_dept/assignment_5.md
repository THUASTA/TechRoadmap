# Assignment 5: Hello, C\#

## Goals

This assignment can help you get started with C#. You can review the object-oriented programming concepts, learn how to use `event` in C#, which paves the way for the future development in the EDC and THUAI competition.


## Q1: Online Bookstore Management System


Imagine you are a C# developer tasked with building an online bookstore management system. This system should allow users to:

- Add, remove, and edit book information, including title, author, price, details and stock quantity.
- Search for books based on different criteria (e.g., title, author, price range).
- Display a shopping cart where users can add and remove books.
- Calculate the total price of items in the shopping cart.
- Implement events to notify when books are added or removed from the shopping cart.

Assignment Requirements:

- Create a C# console application to implement the online bookstore management system.

- Utilize object-oriented programming concepts to design and implement at least the following classes: (It's recommended that a C# file has one and only one class.)

    1. `Book`: Represents a book, including properties like title, author, price, details and stock quantity.

    2. `Bookstore`: Manages a collection of books and performs operations like adding, removing, searching, and editing book details.

    3. `ShoppingCart`: Represents a shopping cart where users can add or remove books and calculate the total price of items. Implement some events, such as BookAddedToCart and BookRemovedFromCart, to notify when books are added or removed from the shopping cart. 



- Utilize `List<T>` from the System.Collections.Generic namespace to manage collections of books and items in the shopping cart.

- Write the main function to test all your classes and methods.Please ensure your code is well-structured, **commented**.

Note that this assignment is just for practice. To save your time, please don't write too complicated or add extra features. 

You should finish your work by September 12th. Once you have completed all the questions, please submit your work to Tsinghua Cloud, uploading them to the folder named after their name in Tsinghua Cloud (e.g. `ASTA2023/部门/竞赛部/技术培训/作业五/张三/Book.cs`,`ASTA2023/部门/竞赛部/技术培训/作业五/张三/Bookstore.cs`,`ASTA2023/部门/竞赛部/技术培训/作业五/张三/ShoppingCart.cs`). If the folder does not exist, please create one.