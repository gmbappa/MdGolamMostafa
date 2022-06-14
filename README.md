# API service
## Description
Develop an API service for Get and Post date base n number of page-size. 

## Setup To Run Project
1. Need To Change DB Server Name at Model/DBAccessLayer.cs
2. Need To Create database

/****** 
    USE [Test]
         GO
		
		SET ANSI_NULLS ON
		GO
		SET QUOTED_IDENTIFIER ON
		GO
		CREATE TABLE [dbo].[Country](
			[Data] [nvarchar](max) NULL,
			[MaxCharacters] [varchar](10) NULL,
			[TotalLinePerPages] [varchar](10) NULL,
			[PageSize] [varchar](10) NULL
		) ON [PRIMARY] TEXTIMAGE_ON [PRIMARY]
		GO
		
		******/
3. Run The Application In visual studio 2019 
4. Using POST-Man For Testing Api Service.

 NEXT IN THIS COLLECTION
 
POST
http://localhost:51544/api/test

Request Headers:
PageSize like 15

GET
http://localhost:51544/api/test
GET
http://localhost:51544/api/test/15

Noted: Other Document and File can be find at Project MdGolamMostafa/Document folder.


### DB Server

* MSSQL


### Development Environment 

* Visual Studio 2019 


## Requirements 

Build and API service using .NET 5 where a user can send a list of words through a post 
request and a page size n using request header. The header name should be page-size. Now 
you have to construct line(s) using those words where each line can contain a maximum n 
number of characters. Return the constructed line through a get request.
