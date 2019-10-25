This is README.md

Install MongoDb

https://www.mongodb.com/download-center/community?jmp=docs

While Installing check the checkbox of Install Compass community server should be checked


After Installing Mongo db
open the Mongo db server

1) Create the Db
2) Create the Collection
3) Import the File speedReportsStructure.json which is attached
4) if you want to import the File from Console 
  :- mongoimport --db speed --collection reports --drop --file reports.json
  
5)  query to get the result from the collection which we use in sqlite database
:- db.test.find({date : "2019-10-06" ,customerno : 549,"data.lastupdated" : {"$gte" : "2019-10-06 00:00:00", "$lte" : "2019-10-06 23:59:59" }}).pretty();

6) Structure Schema
  {
	"customerno" : 549,
	"date" : "2019-10-06",
	"uid" : "9597",
	"vehicleid" : 11296,
	"data" : [
		{
		"deviceid":9613,
		"customerno":549,
		"devicelat":"18.460135",
		"devicelong":"74.346433",
		"lastupdated":"2019-10-06 00:00:46",
		"altitude":555,
		"directionchange":"319",
		"inbatt":"4089",
		"hwv":"1.1",
		"swv":"3.9CHT4_6.23",
		"msgid":"197",
		"status":"E",
		"ignition":0,
		"powercut":1,
		"tamper":1,
		"gpsfixed":"A",
		"online_offline":0,
		"gsmstrength":11,
		"gsmregister":5,
		"gprsregister":13,
		"satv":"9",
		"uid":9597,
		"unitno":"1813010018484",
		"analog1":"0",
		"analog2":"2693",
		"analog3":"0",
		"analog4":"0",
		"digitalio":0,
		"commandkey":"0",
		"commandkeyval":"",
		"vehicleid":11296,
		"vehicleno":"KA52A5079",
		"extbatt":"1149",
		"odometer":115193435,
		"curspeed":0,
		"driverid":21717
		}
	]}