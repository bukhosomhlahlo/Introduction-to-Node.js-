# Introduction-to-Node.js-
## Introduction to Node.js
ECMA Script- Refers to the standard language
Javascript- is what we use in practice and builds on top of EMCA script
#### Java runtime Engines
<ol><li>V8- it is the open source engine developved by google for chrome</li>
    <li>Spider Monkey- is a Javascript engine powering Firefox Browswer
    <li>Javascript Core- is a Javascript engine developed by Apple and Safari
    <li>Chakra- was the Javascript engine created for the original Microsoft Edge, but the latest Microsoft Edge uses the V8</li></ol>
<b>NB</b>: We can embedd the V8 engine into the C++ program and it will run the users Javascript code.
C++ program is the <b>NodeJS</b>

##### Node.JS
Node.js is for sharing code and data structures seamlessly between the front-end and back-end
For example where an attack algorithm is executed on the front end and validated on the back end to prevent cheating, maintaining identical algorithms is imperative.
The use of code sharing and the unification of the front-end and back-end in a common language yield significant advantages in terms of overall development efficiency and maintainability.
    <ul><li>File Handling
        <li>Database Connection
        <li>Network Operations
        <li>Shared library
        <li>Custom function or algprithms
        <li>Data Structures or object defination</li></ul>

##### Advantages of JavaScript
 Unlike other languages in different environments, JavaScript simplifies data transfer from the back end to the front end without requiring intricate conversions.

  <ul><li>Front-end and back-end share language
          <li>Front-end and Back-end share code
          <li>Dynamic
          <li>Works well with JSON
          <li>Custom function or algprithms</li></ul>

###### Callbacks and Asynchronous Tasks

Synchronous and asynchronous callbacks are both programming concepts related to how functions or tasks are executed in a program, particularly in environments where operations may take varying amounts of time to complete, such as network requests, file I/O, or database queries.
<ul><li>Synchronous- In synchronous callbacks, the callback function is executed immediately after the completion of a certain operation or task.
                     These callbacks are executed in a blocking manner, meaning the program waits for the callback function to finish executing before proceeding to the next line of code.


<code>function synchronousTask(callback) {
    *Perform some operation*
    let result = doSomethingSynchronous();

*Call the callback function*
callback(result);
}

synchronousTask(function(result) {
    console.log("Result:", result);
});</code>
                        
 <li>Asynchronous- In asynchronous callbacks, the callback function is not executed immediately after the completion of the operation. Instead, it's scheduled to run at some later time, typically when the operation completes or a certain event occurs.
Asynchronous callbacks are commonly used in scenarios where operations may take a significant amount of time to complete, such as network requests, file I/O, or user input.

<code>function asynchronousTask(callback) {
    // Perform some asynchronous operation, like an AJAX request
    doSomethingAsynchronous(function(result) {
        // Call the callback function when the operation is complete
        callback(result);
    });
}

asynchronousTask(function(result) {
    console.log("Result:", result);
});</code></ul>



