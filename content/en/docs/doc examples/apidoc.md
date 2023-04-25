---
linkTitle: "API Documentation"
# Display h2 to h5 headings
toc_min_heading_level: 2
toc_max_heading_level: 6
---
# API Documentation

## What is an API?

API are application programming interfaces that communicate with two or more products or services or comoputers using a set of definitions and protocols. Applications are software with set of pre-defined functions resulting in outputs. Interfaces are ways or methods by which two or more applications or services communicate with each other using requests and responses.

In most cases, client and server are used to describe API architecture. A request is sent by an application known as a client, and a response is sent by an application known as a server. In the case of the weather, the mobile app is the client and the bureau's weather database is the server in this scenario. 

### What are REST APIs?

These are the most popular and flexible APIs found on the web today. The client sends requests to the server as data. The server uses this client input to start internal functions and returns output data back to the client. 

### What is API Documentation?

Connecting software and/or online services to your platform is made easier by API documentation for partners and consumers. It has every bit of data needed to interact and integrate with an API. The documentation for the API offers users a clever means of information exchange, information transfer, and process support.

#### API Documentation Example

##### Sample API Name

Resource Description - Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

###### Endpoint Name and Method

> **GET** EndpointName/{PathParameter}

Brief Endpoint Description - Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod.

###### Parameters

***Path Parameters***

| Path Paramter      | Description |
| ----------- | ----------- |
| {PathParameter}      | Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.       |


***Query String Parameters***

| Query string parameter      | Required / Optional | Description | Type
| ----------- | ----------- |  ----------- | ----------- |
| ParameterName      | Required or Optional       |  Short Description        |  String Type

###### Sample Request

```
curl -I -X GET "https://api.samplename.org/data/2.5/endpointname?zip=95050&appid=APIKEY&units=imperial&days=2"
```
(In the above code, replace `APIKEY` with your actual API key.)

###### Sample Response

The following is a sample response from the EndpointName/{PathParameter} endpoint:

```ruby
{
    "EndpointName": [
        {
            "PathParameter": "Bangalore",
            "ParameterName": {
                "ParaStatus": {
                    "Height": 9,
                    "Weight": 150,
                    "Age": 40,
                    "recommendation": "Go Running!"
                },
                "ParaStatus": {
                    "Height": 8,
                    "Weight": 90,
                    "Age": 27,
                    "recommendation": "Go Cycling!"
                },
                "ParaStatus": {
                    "Height": 9.5,
                    "Weight": 60,
                    "Age": 32,
                    "recommendation": "Keep it up!!!"
                }
                ...
            }
        }
    ]
}
```

**Response definitions**

The following table describes each item in the response.

| Response item      | Description | Data type
| ----------- | ----------- |  ----------- |
| PathParameter     | Item Description       |  String or Object or Integer       
| {ParameterName}   | Item Description       |  String or Object or Integer    
| {ParaStatus}     | Item Description       |  String     
| {ParaStatus/Height}    | Item Description       |  Integer    
| {ParaStatus/Weight}    | Item Description       |  Integer    
| {ParaStatus/Age}    | Item Description       |  Integer    
| {ParaStatus/Recommendation}    | Item Description       |  String    






