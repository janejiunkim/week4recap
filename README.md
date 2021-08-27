# week4recap #

## AJAX - Asynchronous Javascript and XML 
- Ajax allows users on webpages to interact with servers through HTTP (protocol) -> Made even better with the Fetch API. 
- Async/ await functions 

``` 
async function getUserData() { 
    const url =  'https://google.com/gmail/users'; 
    let users = await fetch (url).then(res => res.json()); console.log(users); }
```

## FETCH ##
- make API requests using javascript -> get Data

```
fetch(requestURL)
     .then(function(responseData){
         return responseData.json();
     })
     .then(function(jsonData){

     })
```

## SQL ##
- Personal Favorite
- Store and access data efficiently in ~databases~
- Allows us to create and query for specific data
```
SELECT name, age FROM teachers;
```

## AJAX IN JQUERY ##
$.get() and $.post()
```
$.get('https://www.reddit.com/bio', {
    q: 'birthdays'
}).done(function(data) {
    console.log(data);
});
 
```

## PROMISES ##
- Because async functions can not run at the same time
- Makes promise to run before or later
```
$.get('https://www.google.com/fellofftherocks').done(function(data {

}).fail(function(error) {

}));
```