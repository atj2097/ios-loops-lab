# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**
//1
//for i in 1...150 {
//    print("\(i) ", separator: " " , terminator: " ")
//}
// print(" ")***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**
//2
//var anyNumber = 142...159
//var index = 142
//
//while anyNumber.contains(index) {
//    if index > 158 {
//             index += 1
//            continue
//           }
//          print(index)
//          index += 1
//   }***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**
var numberRange = 15...80
for i in numberRange where i%2 == 0{
print("\(i) is an even number")
}
***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**
var numberRange = 19...91
for i in numberRange where i%2 != 0{
print("\(i) is an odd number")
}
***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**
var rangeOfNumbers = 0...100
var index = 5

while rangeOfNumbers.contains(index) {
if index > 100 {
index += 5
continue
}
print(index)
index += 10
}
***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**
var rangeOfNumbers = 1...40
var index = 7

while rangeOfNumbers.contains(index) {
if index > 40 {
index += 7
continue
}
print(index)
index += 10
}
***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

var numberRange = 20...150
for i in numberRange where i%3 == 0{
print("\(i) is divisible by 3")
}

***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

var numberRange = 20...150
for i in numberRange where i%3 == 0 && i%2 == 0{
print("\(i) is divisible by 3 and 2")
}

***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:
var rangeOfNumbers = 20...150
var index = 24

while rangeOfNumbers.contains(index) {
if index > 150 {
index += 10
continue
}
print(index)
index += 10
}

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:
var numberRange = 20...150
var index = 20
for _ in numberRange
{
for i in numberRange where i == 31 && i == 35 {
print("\(i)")
}
for index in numberRange where index > 39 && index < 61 {
print("\(index)")
}
print("\(index)") }


***
## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

// Your explanation here
```
//infinite loop because 5 will always be greater than 3 therefore the loop is always true
***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
//var i = 5
//
//while (i < 9) {
//    i += 1
//    print("\(i)")
//}
***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
var i = 5

while (i < 5005) {
i += 5
print("\(i)")
}
***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i > 3) {
    i += 1
}
``` 
//var i = 5
//
//while (i < 5005) {
//    i += 5
//    print("\(i) ") }
//    if i%2 == 0 {
//        print("max number \(i) is even")
//    }
//    else {
//        print("btw, max is number \(i) is odd :(")
//    }

***
## Question 15

What's the difference in syntax between the following two while loops?  Will their outputs be different?  Explain why or why not.

```swift
var i = 1
//loop one
while i <= 10 {
    print("i = \(i)")
    i += 1
}

//loop two
var i = 1

repeat {
    print("i = \(i)")
    i += 1
} while i <= 10
```
//var i = 1
////loop one
//while i <= 10 {
//    print("i = \(i)")
//    i += 1
//}

//loop two
//var i = 1
//
//repeat {
//    print("i = \(i)")
//    i += 1
//} while i <= 10
//no difference because both loops have the same conditions
***
## Question 16

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.
//continue ends a certain part of the loop while break ends the whole thing***
## Question 17

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}
```

[]1
[]2
[]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10
//1, 2, 3, 8, 9 , 10
***
## Question 18

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```

[]1
[]2
[]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10
//1, 2, 3***
## Question 19

Without using Xcode, what will the loop below print?  Explain below.

```swift
outerloop: for x in 1...3 {
    innerloop: for y in 1...3 {
        if y == 2{
            continue outerloop
        }
        print("x = \(x), y = \(y)")
    }
}
```
//x = 1, y = 1
//x = 2, y = 1
//x = 3, y = 1
***
## Question 20

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.
xAxis: for xAxis in 0...10 {
yAxis: for yAxis in 0...10 {
if yAxis == 10{
continue xAxis
}
print("\(xAxis),  \(yAxis)")
}
}
***
## Question 21

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

***
## Question 22

Print the first `N` square numbers. A **square number**, also called perfect square, is an integer that is obtained by squaring some other integer; in other words, it is the product of some integer with itself (ex. 1 = 1*1, 4 = 2 * 2, 9 = 3* 3 …).



Example:
Input: `var N = 5`

Output:
```swift
1
4
9
16
25
```

*** 

//var N = 1...10
//var index = 1;
//for index in N {
//    index += index
//    print(index)
//}

## Question 23

Given an integer N draw a square of N x N asterisks. Look at the examples.

Example 1:
Input: `var N = 2`

Output:
```swift
**
**
```

Example 2:
Input: `var N = 3`

Output:
```swift
***
***
***
```

Hint 1
Try printing a single line of * first.

Hint 2
You can use print("") to print an empty line.

***
