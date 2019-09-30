# Loops Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link of your Fork on Canvas and submit


## Question 1

Write code that prints all the numbers from 1 to 150, **inclusive.**
```swift
for number in 1...150 {
    print(number)
}
```

***
## Question 2

Write code that prints all the numbers from 142 to 159, **exclusive.**

```swift
for number in 142..<159 {
    print(number)
}
```

***
## Question 3

Write code that prints only the even numbers from 15 to 80, **inclusive.**

```swift
for number in 15...80 {
    if(number%2==0){
        print(number)
    }
}
```

***
## Question 4

Write code that prints only the odd numbers from 19 to 51, **inclusive.**

```swift
for number in 19...51 {
    if(number%2!=0){
        print(number)
    }
}
```
***
## Question 5

Write code that prints all the numbers that end in a **5** from 1 to 100, **exclusive.**

```swift
for number in 1..<100{
    if(number%10==5){
        print(number)
    }
}
```

***
## Question 6

Write code that prints all the numbers that end in a 7 from 1 to 40, **inclusive.**

```swift
for number in 1...40{
    if(number%10==7){
        print(number)
    }
}
```

***
## Question 7

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 3`

```swift
for number in 20...150{
    if(number%3==0){
        print(number)
    }
}
```

***
## Question 8

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that are divisible by 2 and 3`

```swift
for number in 20...150{
    if(number%3==0 && number%2==0){
        print(number)
    }
}
```

***
## Question 9

Given a range of numbers from 20 to 150 inclusive, print out all the numbers that follows these conditions:

`Numbers that end with a 4`

```swift
for number in 20...150{
    if(number%10==4){
        print(number)
    }
}
```

***
## Question 10

Given a range of numbers from 20 to 150, print out all the numbers that follows these conditions:

`Print out numbers: 31, 35, 40 to 60.`

```swift

let selectedNum = (31, 35, 40...60)
for num in 20...150 {
    if selectedNum.0 == num || selectedNum.1 == num || selectedNum.2 ~= num {
        print(num)
    }
}
```

***
## Question 11

Without using Xcode, how many times will the loop below run?  Explain why.

```swift
var i = 5

while (i > 3) {
    i += 1
}

// Your explanation here
The loop will run indefinetly as there isn't a decrement toward the value of i that will make it eventually false or below 3 as the while loop will constantly increase the value of i by 1 above 5, making the look indefinitely true.
```

***
## Question 12

Change the code below to make the loop stop executing when i reaches 9.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
My code:
```swift
var i = 5

while (i < 9) {
    i += 1
}
```

***
## Question 13

Change the code below to make the loop stop executing after it has run 1,000 times.

```swift
var i = 5

while (i > 3) {
    i += 1
}
```
My code:
```swift
var i = 1

while (i < 1001) {
    i += 1
}
```
***
## Question 14

Change the code below to make the loop stop executing after it has run 1,000 times and also make it print out the current value of i **only if i is an even number.**

```swift
var i = 5

while (i < 1001) {
    if(i%2==0){
        print(i)
    }
    i += 1
}
```

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
The difference in syntax between the two loops is that the while loop will check the the condition of the loop before its iteration, where as the repeat while loop will execute the statements of the loop after a iteration of its loop. The outputs will be the same as although the second loop executes its loop first, the conditions for both of them will remain true.


# Bonus =)

***
## Question 1

What's the difference between `break` and `continue`?  Give an example that demonstrates their differences.<br/>

The difference between break and continue is that break will terminate a block of code, whereas continue will reiterate a block of code.<br/>
Ex of break:
```swift
for num in 1..10 {
    if num == 4 {
        break
    }
    print(num)
}
//prints numbers from 1 to 3
```
Ex of continue:
```swift
for num in 1..100 {
    if num%10 != 0 {
        continue
    }
    print(num)
}
//prints numbers evenly divisible by 10 from 1 to 100, ignoring all other numbers
```

***
## Question 2

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        continue
    }
    print(i)
}
```

[X]1
[X]2
[X]3
[]4
[]5
[]6
[]7
[X]8
[]X9
[X]10

***
## Question 3

Without using Xcode, what will the loop below print? Select all that apply.

```swift
for i in 1...10 {
    if (i >= 4 && i <= 7){
        break
    }
    print(i)
}
```

[X]1
[X]2
[X]3
[]4
[]5
[]6
[]7
[]8
[]9
[]10

***
## Question 4

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

The loop will print all possible combinations of x,y that exclude y values that equal to 2 and 3 as a continue statement is executed toward every y value that is 2, whereby it points it to the outerloop to ignore a y value of 2 and 3, and iterate to the next x interval or outerloop.

***
## Question 5

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** x and y are both integers.

***
## Question 6

Write code that prints out all the points in the area bounded by (0,0), (10,0), (0,10) and (10,10) **where** the difference of x and y is at least 5, and x and y are both integers.

***
## Question 7

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
## Question 8

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
