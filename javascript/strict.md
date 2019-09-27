# Benifits of using ‘use strict’ 

Strict mode makes several changes to normal JavaScript semantics. 

- Strict mode eliminates some JavaScript silent errors by changing them to throw errors.

- Strict mode fixes mistakes that make it difficult for JavaScript engines to perform optimizations: strict mode code can sometimes be made to run 
faster than identical code that’s not strict mode.

- Strict mode prohibits some syntax likely to be defined in future versions of ECMAScript.

- It prevents, or throws errors, when relatively “unsafe” actions are taken (such as gaining access to the global object). 

- It disables features that are confusing or poorly thought out.

- Strict mode makes it easier to write “secure” JavaScript.


## React also has a strict mode
https://reactjs.org/docs/strict-mode.html

- will detect legacy code and tell you to update it
- can be passed down to wrapped children and bypassed with the others

```js

    <div>
      <Header />
      <React.StrictMode> // this wrap around the components
        <div>
          <ComponentOne />
          <ComponentTwo />
        </div>
      </React.StrictMode>
      <Footer />
    </div>
```