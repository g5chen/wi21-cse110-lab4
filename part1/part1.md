Name: Guo Chen

1. line 11 prints out the number of prices.length to the console, it prints 3 if prices = [100,200,300]. since var i is declared inside the function, the variable i is function scoped, so we can access it later.

2. line 12 prints out the price after discount. output 150 if prices = [100, 200, 300] and discount = 0.5. since var discountedPrice is declared inside the function, the variable discountedPrice is function scoped, so we can access it later.

3. line 13 prints out the last item's price after discount. output 150 if prices = [100, 200, 300] and discount = 0.5. Since the declaration of variable finalPrice is var and defined inside the function, the variable finalPrice is function scoped and we can access it later.

4.
output is 
3
150
150
when i = 3 the for loop ends, variables i, discountedPrice and finalPrice are declared with var keyword are accessible in their enclosing scope even before and after they are declared. that is, three of them are defined inside the function, so they are accessible inside the whole function.
150 is the finalPrice since the last original price inside prices is 300 and the discount is 0.5. 

5.line 11 caused error, since let i is block scoped. We call variable i outside the for loop, so we cannot access it after the for loop.

6. line 12 caused error, since let discountedPrice is block scoped defined inside the for loop. We call variable discountedPrice outside the for loop, so we cannot access it after the for loop.

7. line 13 output the finalPrice of the last item in the prices, output 150 if prices = [100,200,300] and discount = 0.5. since let is block scoped to the statement, and let finalPrice was defined inside the function(outside/before the for loop), we can regard the whole function as a block. so we can still access it inside the function after declaration.

8. the function return error, since line 11 and line 12 called variables that didn't defined in the correct space. If we change let in line 11 and 12 to var, the output should be 3, 150, 150.

9. line 11 caused an error, since let i is defined block-scope inside the for loop function. we cannot access it after the for loop ends.

10. line 12 wants to print out discountedPrice to the console, discountedPrice was defined as const and assigned calculated number into it. and even though it was defined inside the for loop, it should be accessible after the loop since it is global scoped. However, we cannot change its value once defined it, so when the for loop iterate i when i = 1 and wants to update discountedPrice, it would cause error.

11. line 13 wants to print out finalPrice to the console, finalPrice was defined as const and assigned value 0 to it inside the function. const means it is global scoped, but it cannot be changed value afterwards. since line 3 already assigned 0 to it, line 7 would cause error since it wants to assign it a new value.

12. the function call caused error, console shows TypeError: Assignment to constant variable. Because in line 7, it tries to assign finalPrice a new value, which cannot, since finalPrice is defined as const, it cannot be changed value. and also there are errors I explained in question 9, 10, 11.

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

19. output [6, 8, 10]. steps: after we called modifyArray([1,2,3], doSomething), it goes to the function modifyArray first, step into the first for loop when i = 0, and then step into the function doSomething before the for loop ends, then go back to the newArr.push(callback(array[i], function(x){ line, then step into the for loop of the function modifyArray as i incremeneted by 1, then step to function doSomething before the for loop ends, then go back to the newArr.push(callback(array[i], function(x){ line, it iterate 3 times when i = 0, i = 1, i = 2, it stops when i = 3 since the array.length = 3, the condition false. Then finally output [6, 8, 10].

20. see part1-question20.js file

21. the output is 
1
4
3
2

End.
