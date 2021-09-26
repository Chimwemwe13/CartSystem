itemsDB is the database for ms mssql
Programes used 

Postman
Ms sql
Visual Studio   for the  uniqiue API.controller


Packages used 
System.Data.SqlClient
Microsoft.Asp.net.Core.NewtonsoftJson



step 1> i created a database in ms sql to be  able to use it in asp.net

datbase Items included is 
ProductId
ProductName
PriceOfProduct

if you want me to add more information in  i will be able to add

step 2> i then created the api.net controller to create the web api to be able to GET,UPDATE,DELETE

step 3> i then went to app settings to add the function to link the data base 

Conntections String 
step 4> I then went to start up 

TO enable the cores and Json Serializer 

if you want to add in the json Serializer 
 you would then need to add
using Newtonsoft.Json.Serialization;

added a method to Configure   to configure the HTTP request

app.UseCore


step 5> i then added the models  Cartsystem the following Fields 
        public int ProductId { get; set; }
        public string ProductName { get; set; }
        public string PriceOfProduct { get; set; }
step 6> i then created Cat controller 

Added items
using Microsoft.Extensions.Configuration;
using System.Data.SqlClient;
using System.Data;
using WebApi.Models;

then added configuration on public CartController


then used [HttpGet] Json result to add in the get function to get information from the database

then used  [HttpPost]Json result  to insert  information that you want to add in  the data base
 
then usd [HttpPut] jsonResult to update the cart so that any order is made from the front end it will be able to recive it 

then used   [HttpDelete("{id}")] json result  to  delete the unique id number in the database








