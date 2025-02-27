API Testing

URL-Uniform Reformed Locator

Postman - API testing

API documentation is really required

Request - {Address, request method, headers, body} -> <-Response (Status code, header, body}

Collection-is a collection of request.

Variable - {{baseUrl}}

Initial Value -is the value that is shared (public), while Current value will not be shared (private).

Get request - HTTP request method.

Williams, Stephen

url/endpoint

endpoint-is/product in this get product request, /status is also another endpoint.

Resouce - is the body that we get back from

JSON - API usually give back json as body.

Query params

{{baseUrl}}/products?category=dairy

Key-category, value-diary. (Keys and values - are usually case sensitive)

{{baseUrl}}/products?category=dairy&results=20

Path Variable

{{baseUrl}}products/:productid - ":porductid" will be replaced with the given value by postman

Path param doesn't have a question mark.

{{baseUrl}}/products/:productid?product-label=true

Path variable are madetory based on API doc, while query parameters je which comes after "?"

& - delimiter

Path variables are only value, mandatory, part of the endpoint/path

Query parameter are key-value pair, mandatory or optional, starts after the question mark

Business process & rules

Business rules for this API-1. Create, 2. Create a new, 3. add product to cart, 4. Place an order

I

Post Request - HTTP request method.

POST/carts

Creates a card and gives back an id

Use the cart id and use it to get the products in that cart.

POST - {{BaseUrl}}/

Json-transfer data, from one system to another system like from programming language to another system.

JSON SYNTAX- Double quotes is used not single quotes.

{

"FirstName":

"John",

I

"age":

22,

"isMarried":

false,

bool and number doesn't need in double quotes

"Hobbies": ["Netflix","nountain biking"]

}

[

{"firstname":"a" },

{" firstname":"b"}

]

When using POST we write the body in Json format

Postman's body also needs to specify with what type of text is in the body like json or just text.

API AUTHENTICATION

API client - client server communication, postman is the client probably

Headers

API authorization is done by accessToken

Bearer token

HTTP Status code

200-Ok

400-bad request


Using random data



Using random data

{{$randomFullName}}

HTTP headers

Key value pairs

PATCH - HTTP request method.

PUT - HTTP REQUEST METHOD

DELETE - HTTP REQUEST METHOD

GET, POST, PUT, PATCH, DELETE - which to use - look at the API documentation.

HEAD - HTTP REQUEST METHOD - To check where that api endpoint is working or not without

INTRODUCTION TO API TESTING N JAVASCRIPT

First postman script

Scripts-pre request & post response

Pre Script:

console.log('Before the request');

Test

console.log('After the request');

console.clear(): - clear request in postman console

pm.test("Status code is 200", function() {pm.response.to.have.status(200);})

am.test("Status should be up", funtion() {

var json Data pm.response.json():

am.expect(isonData.status).to.egl("UP");

})

JavaScript Basics

Variables

var firstName = 'Jamie';

let firstName 'Jamie';

let lastName 'Doe';

Let fullName1firstName ++ lastName:

let lastName2 = ${firstName} ${lastName)

//back ticks not single quotes

//template literals

const url = 'http://example.com';

//we can't reassign const variables

DATA TYPES

Strings, numbers, boolean, undefined - Primitive data types

Arrays, Non Primitive data types

Object-collection of related items

Mathematical Operations

garaeint("4"); parseFloat('2.5');

VARIABLE SCOPE

{

//code block "{}"

FUNCTIONS IN IS

function sayHello(name)

console.log('Hello from post melon');

sayHello('Jamie');

BUILT IN FUNCTION

Math.random()

Math.floor() //rounds down integer

Function without name is called ananomous function

Const hello() => {

Console.log('Hello')

}

Const add = (a,b) => a + b;

Const add = function add(a,b) =>

{

Let c = atb:

return c;

}


Call Back Function

setTimeoutlannounceBreakfast, 5000);

setTimeout(()=> {console.log("staring to making breakfast")}, 5000); Use Case? - asynchronous Execution

Rm.test("name of test", () => { pm.response.to.have.status(200); });

OBJECTS IN JAVASCRIPT

Const person = {

firstName: "Jamie', "last Name": 'Done', age: 29, isMarried: false,

/saytiello: () => "Hello";

sayHello: function() {return 'hello' +this.firstName;}

Console.log(person.firstName);

//again object properties are case sensitive.

person.email = 'email@gmail.com':

//for const in object, you can add but cannot change already added properties

this.firstName

MANGING OBJECT PROPERTIES

Person['last Name'];

Let jsonString = JSON.stringify(person);

Console.log(isonString); //only data is strogd in stringify not any function like the sayHello

Let newPerson - JSON.parselisonString);

Console.log(newPerson.firstName):

PARSING JSON IN POSTMAN

Console.log(pm.response.text());

Let response = pm.esponse.json();

Response.status

ASSERSTION IN POSTMAN

Em.test('status is be up', () => {

})

//Rm.expect(1).to.eal(1);

Em.expect(response.status.to.egl('UP'));

Console.log(response.status):

ARRAYS

Let number [2, 4, 5, 91;

Let names = ['jamie', 'mary'l

Let employee = [{

En: 'jame'

En: 'jamas

}];

Let anything [3, 'hello', (), []];

NAVIGATING ARRAYS

Number[3];

NAVIGATING COMPLEX DATA STRUCTURE IN POSTMAN

Const response-pm.response.json();

Console.log(response.)response.data[0]

BUILT IN ARRAYS IN JS

numbers.push(15);

numbers.length

numbers.per();

number.shift(); //print and remove that in that array

and there are many more

VERYFIY THE RESPONSE STATUS CODES

TESTING THE RESPONSE BODY

Rm.test("response body test", () => {

cont response = Rm.response.jsion):

pm.expect(response.name).to.eal('nameintheresponsefeild")

Different type of assertion

Em.xpect(respose.price) to be a('number');

Em.expect(response.price).to.be.above(0);

Em.expect(respose.price).to.be.an('object');

REFRACTORING TEST

ERROR HANDLING

Happy path testing-correct path of working with api by user

Negative testing-ensureing correct error is shown when user gives wrong details

(use folder in postman to organize)

REUSING TESTS

Collection level or Folder level -> Edit -> tests -> all the HTTP request in the folder will be tested with this script.

BOUNDARY TESTING

\'in string to use'

Pm.expectiresponse.error).to.have,string("invalid value for query parameter 'caasd'") //contains type

SETTING POSTMAN VARIABLES FROM SCRIPT

Em.collectionVariable.set('firstName', 'Jamie');


