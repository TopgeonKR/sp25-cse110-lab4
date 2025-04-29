1. 20
2. 20
3. Because "var" is function-scoped declaration. It's not block scope, which can cause unexpected behavior in conditions or loops.
4. 20
5. error. Because let is block-scoped, it can't be used out of the if block. as 13 line is after if block is closed, result variable does not exist at that moment.
6. Error. Before line 9, code returns an error because line 7 is trying to reassign new value but const variable doesn't allow it.
7. error. same reason as problem 6.
8. 