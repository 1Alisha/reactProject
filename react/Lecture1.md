# Lecture 1 
1. Print hello world using html
2. Print hello world using javascript
3. CDN links  
      # Content delivery networks are the websites on which complete react code is hoisted and
      we fetch react code from there to use it in our projects. 

      CDN aims to reduce latency(Latency is the delay or waiting time for things to happen)
      
      They host various types of content, including JavaScript libraries, CSS files,
      images, and more. 

4. # Purpose of crossorigin in the CDN links
      It's a security feature that ensures that scripts fetched from trusted sources only.

5. React is a javascript library for building user interface and was created by FACEBOOK developers.

6. Why there are 2 links in the REACT CDN?
   1st for core react 
   2nd acts as a bridge b/w react and browser
   to create mobile applications like react native

7. # React.createElement('h1',{props},"hello") 
   ReactDOM.createRoot(getElementById('root'));
   root.render();

   props are children and attributes that we pass
   React.createElement(
      'h1',
       {                 ]
          id:heading,    ]attributes of h1(In HTML, attributes are used to modify or provide extra details about elements.)
          xyz:abc,       ]
       },
       "hello"           ]children of h1
    ) 

8.  How to create nested divs in react

  <div id='parent'>
      <div id='child'>
          <h1>heading tag created</h1>
      </div>
  </div>  

React.createElement
    (
        'div',
        {
            id:'parent'
        },
        React.createElement
        (
            'div',
            {
                id:'child'
            },React.createElement('h1',{},"H1 created")
        )
    )


9. IMPORTANT POINT
   React.createElement(object)=> HTML(browser understands)
   While rendering the DOM it converts the object into html code which is understood by the browser.

10. How to create siblings in nested loop
   
  <div id='parent'>
      <div id='child'>
          <h1>heading tag created</h1>
          <h2>heading tag created</h2>
      </div>
  </div>  

React.createElement
    (
        'div',
        {
            id:'parent'
        },
        React.createElement
        (
            'div',
            {
                id:'child'
            },
            [
                React.createElement('h1',{},"H1 created"),
                React.createElement('h1',{},"H1 created")
            ]
        )
    )
just pass the siblings into an array as shown above
This is called ARRAY OF 

11. Does order of file matters in react
    Yes, app.js file should always be below the react cdn links.

12. Render will replace the code inside html with the react code

13. What is the difference between library and framework
    Library: You use a library when you need specific tools or functions.
             You call the library's functions in your code.
    Example: You borrow a book (library) and use the recipes (functions) you need.

    Framework: A framework is like a set of rules that helps you build an entire house.
               You follow the framework's guidelines, and it does a lot of work for you.
    Example:   You get a construction framework that tells you where to put walls, doors, and windows.
               You fill in the details.
    

