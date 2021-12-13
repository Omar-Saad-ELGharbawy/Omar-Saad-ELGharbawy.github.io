# Const and Ampersand (&) Report 
## Usages of Const :
![const keyword](https://media.geeksforgeeks.org/wp-content/cdn-uploads/Constants-in-C.png)
1. When you don't want anyone to change or override values of a variable : Use `const` keyword in declaring this variable as constant(Read-only and unchangeable) Variable
- Code ex:
```
const int constNum = 15;  // constNum will always be 15
constNum = 10;  // error: assignment of read-only variable 'constNum'
```
2. To declare constant mathematical values
- Code ex:
```
const float PI = 3.14;
const int minutesPerHour = 60;
```
3. Use **pointer** to point to a const variable
- Code ex:
```
const int* K; //K is a pointer that can point to a const int type variable
char const* L; //L is a pointer to an char which is of const type
```
4. To make a ***constant pointer*** (put the `const` keyword to the right of the `*`) so we cannot change the pointer but can change the value that it points to.
- Code ex:
```
  int x = 1;
  int* const p = &x; //p is a constant pointer
 ```
5. const pointer pointing to a const variable.
- Code ex:
```
  const int* const x;
 ```
6. To make constant Function Arguments
- Code ex:
```
  void constantFunction (const int i)
{
    i++;    // error
}
 ```
## Usages of Ampersand operator :
1-Creating a **refrence variables** by the `&` operator
- Code ex:
```
  string name = "Omar";  // name variable
  string &nameRefrence = name;    // reference to name
 ```
2-To get the **memory address** of a variable
- Code ex:
```
  string name = "Omar";  
  cout << &name ;    // Outputs the memory location of the name variable
 ```
3-To declare a **pointer**
- Code ex:
```
  string name = "Omar";
  string* ptr = &name;   // A pointer variable, with the name ptr, that stores the address of name 
 ```
4-Use `&&` as ***logical operator*** (**AND**) :returns true if both operands are true and returns false otherwise
- Code ex:
```
 int x = 6;
    int y = 5;
    if((x > 0) && (y > 0))
    cout << "Both Numbers are postive";
```
- ![Logical Operators](https://www.javascripttutorial.net/wp-content/uploads/2016/11/JavaScript-Logical-Operator.png)