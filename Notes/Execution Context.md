- When you call a function, you create a new execution context comprised of:
    - The thread of execution
    - A local memory environment where things defined in the function are stored (**variable environment**)
- Global execution context
    - As soon as you start running your code, you create a **global execution context**
    - Consists of
        - The thread of execution (parsing and executing code line by line)
        - Live memory of variables with data (**Global Variable Environment**)