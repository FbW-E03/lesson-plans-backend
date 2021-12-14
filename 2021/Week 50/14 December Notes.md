## Problems with the application we built

1. Application does not give much feedback - we have no idea if we are logged in or not

2. We would like the option to logout

3. We would like to hide some navigational elements where appropriate (for example, no "Logout" button when we are not logged in)

4. A future improvement - add notifications

##### What we know of our application so far...

- Storing the JWT token in a httpOnly cookie
- We need to call the backend to tell it to remove the token, if the user decides to logout

## Conventions when building an application

- Consistency is key
- Follow the conventions as setup within the application
- Change the way you code to match the style as setup by the team

## Running a React application

- `npm start` or `npm run start` - development (not optimised, but better for debugging)
- `npm run build` - production (how you want to deploy your project for pubic consumption)

## IIFE - Immediately invoked function expressions

Fancy way of saying "make a function as an expression and run it"

An expression is a piece of code which resolves to a value

```javascript
const string = getString(); //expression = "some string"
const string2 = "dfjd"; // "dfjd"
const numbers = 2 + 2; // 4
```

## React Context API

##### Prop drilling

**anti-pattern**
If we consider that a pattern is an established, "best" practise which you are encouraged to follow - an anti-pattern is the opposite, in the sense that it goes against convention and is recognised as being counter-productive in the long term / can cause problems in terms of maintenance and readability.

## Storing data within our web application

- cookies
- localStorage - (reliable) permanent, until user manually deletes
- sessionStorage - (less reliable) - as soon as your session is over, it is removed