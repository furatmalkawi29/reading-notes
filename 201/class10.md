
# Error Handeling and debugging 

- You Need To Know The **order** in which statements are executed and variables scopes 


# Stack 


- call stack **manages execution contexts**

- execution contexts : 
1. Function execution context 

2. Global excution context 


- stack works based on the LIFO principle : **last-in-first-out.**

- it excute statements one by one 

- stack **starts with Global excution context** (code in global scope)

- then, if it needed to excute a code inside a function *(function call)* , it creats **new Function excution contexts**

- it **pauses the previous excution** context , adds the **new on the top** and works on it. 

![](https://cdn.javascripttutorial.net/wp-content/uploads/2019/12/JavaScript-Call-Stack.png)


![](https://miro.medium.com/max/1000/1*ACtBy8CIepVTOSYcVwZ34Q.png)


# Error objects 
Show in console messages to describe errors .

- 7 error object (syntax error is one of them)

# Dealing with Errors :

1. ## Debugging then fixing 

- tracing the error source using **Console** in browser 
- breakpoints 
2. ## handeling errors

- write error-handling code
- **try, catch, finally** statements. 



