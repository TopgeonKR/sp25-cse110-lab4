1. 3, because the loop ends when i turned into 3 as prices.length is 3. And var is function-scoped, which means it's still declared out of for loop.
2. 150, for the last iteration in loop, discountedPrice is 300*(1-0.5). and as it's var which is function-scoped, printing outside of for loop still works.
3. 150, in line 8, discountedPrice is rounded and store in finalPrice var.
4. [50, 100, 150]  / Input: prices = [100, 200, 300], discount = 0.5, for each price, discount rate is applied and stored in array discounted which results in [50, 100, 150] and it's returned.
5. Error, because i is declared by let which is block-scoped.
6. Error, because discountedPrice variable is declared by let which is block-scoped and the code is trying to print it outside of the for loop.
7. 150. finalprice is declared outside the loop using let. so it remains accessible.
8. [50, 100, 150] Same as problem 4.
9. Error. Trying to use i declared in the block by let.
10. 3, length is declard using const at outside of the loop. const is block scoped to the function and not reassigned. so it's alid and accessible at line 12
11. [50,100,150] const fix the variable, but for array, you can change the value inside the array even though the array is declared using const.
12. A: student.name
    B: student["Grad Year"]
    C: student.greeting()
    D: student["Favorite Teacher"].name
    E: student.courseLoad[0]
13. A: '32', + works as concatenation when there's string.
    B: 1, - is number operator
    C: 3, null turns into number 0
    D: '3null', + works as concatenation when there's string.
    E: 4, true turns into 1
    F: 0, false and null both turn into 0
    G:'3undefined', + works as concatenation when there's string.
    H: NaN, undefined can't be converted into number
14. A: true, '2' turns into 2
    B: false, comparison between string is comparing lexicrographical value 2 is greater than 1, which is the first letter of '12'
    C: true. because it's using weak comparison which convert types automatically.
    D: false. beause it's using strcit compartion which even compare types.
    E: false. true turns into number 1 and 1!=2
    F: true. Boolean(2) is true because Boolean return false only for 0. and comparing true and true which are the same => true
15. == compares values after type conversion, while === compares both value and type without converting them.
16. (part2-question16.js)
17. [2,4,6]
    We call modifyArray([1,2,3], doSomething)
    Inside modifyArray, newArr is intialized as an empty array.
    the for loop iterates over each element 1,2,3. On the first iteration array[i] us 1. It calls callback(1), which is doSomething(1), and this returns 2 and 2 is pushed int newArr. For next two more iteration, 2->4->pushed / 3->6->pushed.
    After the loop, newArr is [2,4,6] which is returned.
18. (part2-question18.js)
19. 1
    4
    3
    2