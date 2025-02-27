Rest Assured

Frond End Website (Java Technology) -> Back End Code (Java Technology) -> Database

API-Application programming interface

Front End (Angular - TypeScript) http request, http response API <-> Back EndCode(Java)<

> data Base

Testing API

Terminologies

End point/Base Url: Address where API is hosted on the server

HTTP methods which are commonly used to communicate with Rest API's are

GET, POST, PUT, DELETE

GET-Used to extract information from the server

POST-Used to send data to the server

PUT-Used to replace existing data that is already in the server

DELETE-Used to delete the already existing data in the server

Path Parameters - are variables parts of a URL path. They are typically used to point to a specific resource within a collection, such as a user identified by id.

Query Parameters-is used to sort/filter the resource.

BASEURL/Resource/(query/path) Parameters

Headers/Cookies - Headers represent the meta data associated with the api request and response. Additional details

REST ASSURED-java-based library that is used to test RESTful web Services/APIS

Install java, set path variables,

Maven-Build management tool-Automatic standard project skeleton creation, ease of adding project dependencies -> mvnrepository.com, seamless integration with CI/CD

Group id-parent (upper hitachy to project name)

Aritifact id-project name

<dependencies></dependencies>

Rest Assured-scope is removed

testNG

Hamcrest

I Created a basics class in src/test/java

Given-all input details

When submit the api,

Then-validate the response



Import ig.restassured RestAssured:

Import static ig,restured.BestAd.*;

BestAssured.baseURI="uri":

Given().log().all().queryParam("key", "qaclick123").header("Content-Type", "application/json")

body("")

when().post()

then().log().all().assertThat().statusCode(200);

QueryParam is the thing that adds after the endpoint with 2 in it. Here it will be ?key=qaclick123

Given when().get("/endpoint").then().statusCode(200);


given()-queryParam("", "")

when().get("/endpoint")

.then().log().all().assertThat().statusCode(200);

diff in using assertThat() or without using assertThat() at this point.

//I don't see any

That equalTg) in validation had that error because of not importing a static package in hamcrest

Import static org.hamcrest Matchers.*;

// auto suggestion doesn't work for static

Server response validation.

Header("server","Apache/blahblah")

String response.extract().response().asString():

JsenPath, js = new JsonPath(response);

String placeldis.getString("place..id");

Copilot Java Syntax-Setting up RestAssured:

import jo restassured. RestAssured:

import jo.restassured.response. Response:

public class RestAssured Example {

public static void main(String[] args) {

BestAssured.baseURI= "https://api.example.com";

}

}

GET Request:

import static jo restassured. RestAssured.":

import static org.hamcrest Matchers.*:

public class GetRequestExample {

public static void main(String[] args) {

given()

when()

get("/endpoint")

then()

.statusCode(200)

body("key", equalTo("value"));

}

}

POST Request:

public class PostRequestExample (

public static void main(String[] args) {

given()

header("Content-Type", "application/json")

.body("{\"name\": \"John\", \"age\": 30]")

when()

.post("/endpoint")

then()

statusCode(201)

body("id", notNullValue());

}

}


PUT Request:

public class PutRequestExample.{

public static void main(String[] args) {

given()

header("Content-Type", "application/json")

body("{\"name\": \"John\", \"age\": 31 }")

when()

.put("/endpoint/1")

.then()

statusCode(200)

body("name", equalTo("John"));

}

}


DELETE Request:

public class DeleteRequestExample {

public static void main(String[] args) {

given()

when()

.delete("/endpoint/1")

.then()

.statusCode(204);

}}


Body("msg", equalTo("blahblah"))

String getplaceresponse = Given().queryParam("key", "qaclick123").queryParam("place_id", placeldVariable)

when().get("maps/api/place/get/json")

.then().assertThat().statusCode(200).extract.response().asString()

JsonPath js1 New JsonPath(getplaceresponse);

String actualAdress = js1.getString("address");

Assert.assertEquals(actualAdress, responseAddress);


COMPLEX NEXTED JSON

JsonPath js = new JsonPath(string EinJsonformat);

Int count = js.getInt("courses.size()") //only use this on array that is In json format

Int totalAmount=js.getInt("Dashboard.purchaseAmount")

String title First - js.get("courses[0].title"); //get method at default will return string

Import org.testng.Assert;

Import org.testng.annotations.Test:

Public class SumValidation{

@Test

Public void sunOfCourses()

{

//run as testNG

I

}

}




ADVANCED PAYLOAD CREATION STRATERGIES

I

Dynamicall build json payload with external data inputs,

Parameterize the api tests with multiple data sets,

How to send static json files(payload) directyl into post method of rest assured,

Feed json payload from using excel using hashmap

TESTNG DATA PROVIDER FOR PARAMETERIZATION

@DataProvider(name = "dataProvider name")

public Object[][] getData()

{

return New Object[][] {{"1", "2"}, {"1", "3" } };

}

//

@Test(dataProvider = "dataProvider name")

public void test(String firstelement, String secondElement){

//use the variable in this method

}

STATIC JSON PAYLOAD, COVERTING JSON FILE INSIDE JAVA CLASS

New String (Files.readAllBytes(Paths.get("C:\\user"))) //add inside the body() //add throws

SEND FILES ATTACHMENTS THROUGH REST API CALLS

Jira-project management tool (collaboration tool).

Adding attachment to Jira bug issue using Jira API

When you want to send any file through rest API you can do it through form parameters.

Key format as file instead of text. (It should be in body)

THROUGH RESTASSURED JAVA JIRA ΑΡΙ

RestAssured.baseURI = "blahblah.atlassian.net"; given()

.header("Content-Type", "application/json") header("Authorization", "token")

.body("")

.post("rest/apj/3/issue")

.then().statusCode(201);

//extract id through jsonpath

given()

.pathParam("key", issueld)

//.header("Content-Type",

"application/json") not used

header("X-atalsadftoken", "nocheck") //refer documentation

.header("authorization", "token")

.multiPart("file", new File("path.jpeg"))
I .post("rest/api/3/issue/{key}/attachments").

Then.assertThat().statusCode(200);

OAUTH

Client credentials grant type- Client credentials -- client id, client secrets.

Client username - username, password.





