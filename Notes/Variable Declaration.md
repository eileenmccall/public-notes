- All variables are in one of two roles at any given time
    - They are being assigned a value
    - A value is being retrieved from them
    - It can only be in one position, so if it's not in one role, it must be in the other
- When running in "sloppy mode", if you assign a value to a variable that has not been declared, that variable is automatically declared in the global scope.
- When you try to reference a variable, JS will first check the current scope before moving up the scope chain. This is called **scope masking**
- Even if two variables have the same name, JS will use the one in the current scope before looking in the outer scope.
- When trying to locate a variable, a function will first look in its local variable environment, then in `[[scope]]`, **then** in the outer scope(s)