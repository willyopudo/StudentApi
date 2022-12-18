# StudentApi
This is a repository for API lab exercise in ASP.NET Core Web API v5.0</br>

The API allows only POST and GET methods on Student entity repository. Other RESTful methods are disabled</br>
It is a simple example of a REST API a bank can use to verify details of a student making payment to a school account, 
such that the school can receive a payment notification with information about the student

To launch the app, clone the repo in the workspace root for Visual Studio 2019 or later, open, download any dependencies and run the app.

On successful build, the API endpoint is exposed at <strong>https://localhost:44308/api/students</strong></br>
This app uses an in-memory database. If the app is stopped and started, the preceding GET request will not return any data. </br>
If no data is returned, POST data to the app using postman as detailed below:

************************************************************************************************************************
Create a new request.

Set the HTTP method to POST.

Set the URI to https://localhost:44308/api/students. 

Select the Body tab.

Select the raw radio button.

Set the type to JSON (application/json).

In the request body enter JSON for a student object e.g:</br>
//</br>
{</br>
        "FirstName" : "Felix",</br>
        "LastName" : "Wazekwa",</br>
        "Email" : "wfelixd@yahoo.com",</br>
        "EnrollmentDate" : "2019-01-10",</br>
        "Course" : "Bachelor of Commerce",</br>
        "IsActive" : true</br>
}</br>
//</br>
Click Send
*****************************************************************************************************************

To test GET method with location URI, set the URI to: </br>

https://localhost:44308/api/students/>>ID<< where ID is the student id e.g 1,2 etc
