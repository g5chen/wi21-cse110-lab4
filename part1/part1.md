Name: Guo Chen

1. line 11 prints out the number of prices.length to the console, because Javascript does not have block scope until const and let were introduced, just var which is function scoped.

2. line 12 prints out [Function: discountPrices] to the console. In javascript, we can call console.log(Function) inside the function. 

3. line 13 prints out the last item's price after discount. Since the declaration of var finalPrice made declares a function-scoped variable.

4.
3
150
150
i = 3, variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before and after they are declared. 
150, variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before and after they are declared. 
150 is the finalPrice, the original price is 300 and the discount is 0.5. variables declared with var keyword are hoisted (initialized with undefined before the code is run) which means they are accessible in their enclosing scope even before and after they are declared. 

5.line 11 caused error, since let is block scoped to the statement, or expression within which it is used. We call variable i outside the for loop, so the system cannot see it.

6. line 12 caused error, since let is block scoped to the statement, or expression within which it is used. We call variable discountedPrice outside the for loop, so the system cannot see it.

7. line 13 output the discounted price of the last item in the prices, since let is block scoped to the statement, or expression within which it is used. We defined and called variable finalPrice within the function discountedPrices, so the system can see it.

8. the function return error, since line 11 and line 12 called variables that didn't defined in the correct space.

9. line 11 is an error, since let i is defined block-scope inside the for loop function.

10. line 12 output the discountedPrice, since it is defined as const, the scope is global.

11. line 13 would output 0, since it is defined as const, it is global, and the later code cannot change it's number.

12. the function call caused error, console shows TypeError: Assignment to constant variable. Because in line 7, it tries to assign finalPrice a new value, which cannot, since finalPrice is defined as const, it cannot be changed value.

13.
A: student.name
B: student["Grad Year"]
C: student.greeting()
D: student["Favorite Teacher"].name
E: student.courseLoad[0]

14.
A: '32'
B: 1
C: 3
D: '3null'
E: 4
F: 0
G: '3undefined'
H: NaN

15.
A: true
B: false
C: true
D: false
E: false
F: true

16. == in Javascript is used to comparing two variables, and ignores the datatype. === is used for comparing two variables but the operator also checks the datatype and the values.

17. the console output 'How are you?' since (2 == true) is false, and it checks (2), which is true since if you pass a number, that always evaluates to true unless it's 0. 

18. see part1-question18.js file

19. output [6, 8, 10]. steps: after we called modifyArray([1,2,3], doSomething), it goes to the function modifyArray first, run the first for loop when i = 0, and then go to the function doSomething, then go back to the newArr.push(callback(array[i], function(x){ line, then go to the for loop of the function modifyArray as i incremeneted by 1, then jump to function doSomething, then go back to the newArr.push(callback(array[i], function(x){ line, it iterate 3 times when i = 0, i = 1, i = 2, it stops when i = 3 since the array.length = 3. Finally output [6, 8, 10].
