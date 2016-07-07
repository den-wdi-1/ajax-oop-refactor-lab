# Ajax OOP Refactor Lab

| Objectives |
| :--- |
|By the end of this lab, developers will be able to...|
| Refactor Existing Front End JavaScript into OOP |
| Reinforce OOP JavaScript concepts |

## Where We Are

In the last lab, we did some test-driven development (TDD) to create a JSON api using Express.

For this lab we are going to take the *front-end* JavaScript we were given and refactor it into OOP.

#### Requirements

1. Inside of the document ready, we should declare

  ```js
      var app = new App();
  ```

2. Methods can be called on `app` from inside the document ready,

  ```
    app.render();
  ```
 but nothing should be defined in there!

3. Define all of your variables on App:
  ```js
    function App(){
      this.baseUrl = '/api/todos';
      ...
    };
  ```
>Think-pair-share: Look at the code and think of some other properties we would need in our ```App()``` constructor.

4. Attach all of your functions to App's prototype:
  ```js
    App.prototype.render = function() {
      this.$todosList.empty();
      ...
    };
  ```
>Think-pair-share: Look at the code and think of some other methods we would need in our ```App()``` prototype.

5. Try to set this up in small steps, and when in doubt (as often as possible), run the code and debug errors one by one.
6. When you are finished you should be able to create, read, update and destroy todos on your app!

## Resources
[OOP in JS: What you need to know](http://javascriptissexy.com/oop-in-javascript-what-you-need-to-know/)
