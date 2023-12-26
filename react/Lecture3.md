# scripts in package.json
scripts": {
    "start":"parcel index.html",
    "build":"parcel build index.html",
    "test": "jest"
} 
created shortcut for 
npx parcel index.html => npm run start

# jsx
1. jsx looks like html syntax or xml but both are not same
2. jsx is syntax and react element is an object

const heading=React.createElement('h1',
    {
      id:"heading",
    }
    "hello jsx"
)

# This above react code is equivalent to below jsx code.

const jsxHeading=<h1 id="heading">H1 element in jsx</h1>

# We code for both humans and machines
But first for human then fir machine 

# js engine understands only ECMA script i.e. es6 browser understands ecma
so how jsx code is showing on browser so here comes parcel which transpile the code parcel is just the manager actual work is done by babel

# Transpilation with Babel:
JSX needs to be transformed into standard JavaScript (ECMAScript) that browsers can understand. This process is called transpilation. Babel is a popular JavaScript compiler that can perform this transpilation. It converts JSX code into standard JavaScript code.
 
# When you use Parcel to build a React project, it automatically configures Babel to transpile JSX into standard JavaScript.

# on babel website u can get the conversion of jsx code into es6 (can see live demmo)

# in html we use class and in jsx we use className i.e why both html and jsx are       different.

# jsx is camelcase 

1. single line jsx
   const jsxHeading=<h1 id="heading">singleline jsx</h1>

2. Multiline jsx
   const jsxHeading=(
                    <h1 
                       id="heading">
                            singleline jsx
                    </h1>
                    ) 
While writing codes in multiline it is nescessary to put the brackets so that babel can understand from where the code is starting and where it is ending.

# jsx code => babel transpiles it to React.createElement => react element -> js object ->HTMl element(render)

# REACT COMPONENTS
1. CLASS-BASED
2. FUNCTIONAL-BASED

CLASS-BASED 
-old way of writing code 
-uses javascript classes to create components

FUNCTIONAL-BASED
-uses javascript functions to create components
-javascript function that returns jsx piece of code 

Whenever creating a component its starting letter should be capital in the name 
# How to render a component
root.render(<component/>)

# What is component composition
Composing two components into one another




