# Node Ecosystem, TDD, CI/CD

## Array.map()

- The map() method will create a new array after calling the function that is invoked on each index of the array.

## Array.reduce()

- The reduce() method executes a 'reducer' function (which is provided by the developer) on each element of the array, and will result in a single value as output.

- The reducer function takes in four arguments:
* Accumulator
* Current Value
* Current Index
* Source Array

- The reducer functions returned value is then assigned to the accumlator, this value is remembered across each iteration through the array and lastly will become the final single resulting value.

## Superagent()
- How to fetch data from a URL

* Normal Promise .then() - 

- A request can be initiated by invoking the appropriate method on the request object, then calling .then() (or .end() or await) to send the request. For example a simple GET request:

 `request
   .get('/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });`

- The above code can be used to get (.get) information from an API or other source and after it receives said data it uses the (.then) to say what it will do with it.  The (.catch) is utilized for errors.

* Async/Await - 

`SuperAgent's request is a "thenable" object that's compatible with JavaScript promises and the async/await syntax.

const res = await request.get(url);
If you're using promises, do not call .end() or .pipe(). Any use of .then() or await disables all other ways of using the request.

Libraries like co or a web framework like koa can yield on any SuperAgent method:

const req = request
  .get('http://local')
  .auth('tobi', 'learnboost');
const res = yield req;`

* Async functions use implicit Promises to return results.  If a promise is not returned the async function ensures that our code is passed through the promise.

- Await blocks the code execution within an async function and only ensures that the next line is executed when the promise is resolved.


### Promises
- The Promise object represents the eventual completion or failure of an asynchronous operation, and the resulting value.

- A promise is like a real world promise in that after it is given it can be kept or broken.  When the promise is kept we can utilize that data usually followed by a .then or other options to say what to do with the promise we receive.  If the promise is broken we try to find out why and deal with it after understanding the underlying problem.

### Callback Functions

>"Callbacks are versatile — not only do they allow you to control the order in which functions are run and what data is passed between them, they also allow you to pass data to different functions depending on circumstance. So you could have different actions to run on the response downloaded, such as processJSON(), displayText(), etc.

>Note that not all callbacks are async — some run synchronously. An example is when we use Array.prototype.forEach() to loop through the items in an array".




References:

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map

https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reduce

https://medium.com/better-programming/should-i-use-promises-or-async-await-126ab5c98789

https://visionmedia.github.io/superagent/