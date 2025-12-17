1. Write a program in javascript to display the first 100 natural numbers.
Expected Output :
1 2 3 4 5 6 7 8 9 10 . . .

2. Write a javascript program to find the sum of first 10 natural numbers.
Expected Output :
The first 10 natural number is :
1 2 3 4 5 6 7 8 9 10
The Sum is : 55

3. Write a program in javascript to display n terms of natural number and their sum.
Test Data : 7
Expected Output :
The first 7 natural number is :
1 2 3 4 5 6 7
The Sum of Natural Number upto 7 terms : 28

4. Write a program in javascript to read 10 numbers from keyboard and find their sum and average.
Test Data :
Input the 10 numbers :
Number-1 :2
...
Number-10 :2
Expected Output :
The sum of 10 no is : 55
The Average is : 5.500000

5. Write a program in javascript to display the cube of the number upto given an integer.
Test Data :
Input number of terms : 5
Expected Output :
Number is : 1 and cube of the 1 is :1
Number is : 2 and cube of the 2 is :8
Number is : 3 and cube of the 3 is :27
Number is : 4 and cube of the 4 is :64
Number is : 5 and cube of the 5 is :125

6. Write a program in javascript to display the multiplication table of a given integer.
Test Data :
Input the number (Table to be calculated) : 15
Expected Output :
15 X 1 = 15
...
...
15 X 10 = 150

7. Write a program in javascript to display the multipliaction table vertically from 1 to 8.
Test Data :
Input upto the table number starting from 1 : 8
Expected Output :
Multiplication table from 1 to 8
1x1 = 1, 2x1 = 2, 3x1 = 3, 4x1 = 4, 5x1 = 5, 6x1 = 6, 7x1 = 7, 8x1 = 8
...
1x10 = 10, 2x10 = 20, 3x10 = 30, 4x10 = 40, 5x10 = 50, 6x10 = 60, 7x10 = 70, 8x10 = 80

8. Write a program in javascript to display the n terms of odd natural number and their sum .
Test Data
Input number of terms : 10
Expected Output :
The odd numbers are :1 3 5 7 9 11 13 15 17 19
The Sum of odd Natural Number upto 10 terms : 100


Good Questions of Loops Below:

1. take a number from user and find factorial of that
let num=5 -> 5*4*3*2*1 = 120
2. print fibonnaci series let n=10
0 1 1 2 3 5 8 13 21 34
3.check whether a no. is 3 digit armstrong or not i.e
153 = 1*1*1 + 5*5*5 + 3*3*3 => 153
4. take a number from user and count how many digits are in that number eg.4589 -> 4
5. take a number from user and count how many odd digits are in that number eg.45897 -> 3
6. take a number from user and count how many even digits are in that number eg.4589 -> 2
7. take a number from user and sum of the even digits in that number eg.4589 -> 12
8. take a number from user and sum of the odd digits in that number eg.4589 -> 14
9. take a ,n,d from user and print the A.P (arithematic progression)
let a=10 n=6 d=3
a a+d a+2d a+3d a+4d a+5d . .
10 13 16 19 22 25 Ans.
10. take a number from user and check whether it is a prime number or not.
11.Take a number from user and count it's length and the sum of odd and even numbers
present in that number then let these 2 results as first and second term
and make fibonnaci series from them till n(the length of that number) term.
let num=321578 OddSum=16 evenSum=10 digitLen=6
16 10 26 36 62 98 Ans.
12. reverse a number 1234 -> 4321
13. check whether a no. is palindrome or not
i.e 12321 -> after reverse -> 12321

---

## Star Patterns (using loops) ⭐

Below are concise star-pattern questions to practice nested loops. Each includes a sample input and expected output plus a short JavaScript solution using loops.

1) Right triangle
Test Data: n = 5
Expected Output:
```
*
**
***
****
*****
```
Sample JS (nested loops):
```js
for (let i = 1; i <= n; i++) {
	let line = '';
	for (let j = 1; j <= i; j++) line += '*';
	console.log(line);
}
```

2) Inverted right triangle
Test Data: n = 5
Expected Output:
```
*****
****
***
**
*
```
Sample JS:
```js
for (let i = n; i >= 1; i--) {
	console.log('*'.repeat(i));
}
```

3) Centered pyramid
Test Data: n = 5 (rows)
Expected Output:
```
		*
	 ***
	*****
 *******
*********
```
Sample JS:
```js
for (let i = 1; i <= n; i++) {
	const spaces = ' '.repeat(n - i);
	const stars = '*'.repeat(2 * i - 1);
	console.log(spaces + stars);
}
```

4) Diamond (odd rows)
Test Data: n = 5 (half height)
Expected Output:
```
	*
 ***
*****
 ***
	*
```
Sample JS (combine pyramid + inverted pyramid):
```js
// top (including middle)
for (let i = 1; i <= n; i++) console.log(' '.repeat(n - i) + '*'.repeat(2 * i - 1));
// bottom
for (let i = n - 1; i >= 1; i--) console.log(' '.repeat(n - i) + '*'.repeat(2 * i - 1));
```

5) Hollow square
Test Data: n = 5
Expected Output:
```
*****
*   *
*   *
*   *
*****
```
Sample JS:
```js
for (let i = 1; i <= n; i++) {
	let line = '';
	for (let j = 1; j <= n; j++) {
		line += (i === 1 || i === n || j === 1 || j === n) ? '*' : ' ';
	}
	console.log(line);
}
```

6) Pyramid of numbers (bonus) — Floyd style using stars optional
Test Data: n = 4
Expected Output:
```
1
2 3
4 5 6
7 8 9 10
```
Sample JS:
```js
let val = 1;
for (let i = 1; i <= n; i++) {
	let line = '';
	for (let j = 1; j <= i; j++) {
		line += (val++) + (j === i ? '' : ' ');
	}
	console.log(line);
}
```

----

Want these converted into interactive HTML/JS examples or more patterns (e.g., hollow pyramid, mirrored triangles)? 🔧