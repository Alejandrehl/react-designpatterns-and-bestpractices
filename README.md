# React Design Patterns And Best Practices

## Babel
- Babel is a popular JavaScript compiler widely adopted within the React Community.

Babel can compile ES2015 into ES5 JavaScript, as well as compile JSX into JavaScript functions. The process is called transpilation, because it compiles the source into a new source rather than into an executable.

## ESLint
1. yarn global add eslint
2. create .eslintrc in root folder
3. Try this code (Disable semicolon)

        {
          "rules": {
            "semi": [2, "never"]
          }
        }

**semi** is the name of the rule and **[2, "never"]** is the value.

ESLint rules have three levels, which determine the severity of the problem.
* off or 0: The rule is disabled
* warn or 1: The rule is warning
* error or 2: The rule throws an error

The second parameter tells ESLint that we want the semicolon never to be used (the opposite is always).

We can enable and disable every single rule manually, or we can enable the recommended configuration in one go by putting the following code into our .eslintrc:
    
    {
       "extends": "eslint:recommended"
    }
