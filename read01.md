## Map() Method:
  - is a Method used for looping over an array and allow to store a result of loop inside it usinng `return` statment without changing the value of the originoal array.

## Reduce() Method:
  - it is similar to **array.map() method** but it has three parameters one for index, one for value of index, and the last one is used as a variable instead of defining a variable for it and that variable should be returned using `return` statment.

## Superagent:
  - it is a library used to produce an HTTP request to the API to bring data from it .
* superagent using *.then()*:
`
let url='https://api.covid19api.com/summary';
superagent.get(url)
.then(result=>{
    res.send(result.body);
})
`
* This is an example of using async/await with super agent:
`  .post('/api/pet')
   .send({ name: 'Manny', species: 'cat' })
   .set('X-API-Key', 'foobar')
   .set('Accept', 'application/json')
   .end(function(err, res){
     if (err || !res.ok) {
       alert('Oh no! error');
     } else {
       alert('yay got ' + JSON.stringify(res.body));
     }
   });
`
#### Promise Function:
  - is a function that needs time so to avoid causing a long period of time we use it and it works by complete excuting the code after it then when it reach the *fullfulled* status the interpretter goes back to that function and take the result from it.

#### Are all callback functions considered to be Asynchronous? Why or Why Not?
- no they don't considred as a call back functions because it depends on the argument is being passed to to outer function which is the callback function itself + excution time of it + the dependency on other activity from the user like clicking or writting..etc .



## Which 3 things had you heard about previously and now have better clarity on?
1. Node.js
2. v8.
3. Require function.

## Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
1. Modules.
2. Packages.
3. Asynchronous Functions.

## What are you most excited about trying to implement or see how it works?
- npm packages that I didn't use before.