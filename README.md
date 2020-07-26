# MSA-2020Phase1-backend

URLs of the APIs that have been hosted on Azure: https://msa-backend-app.azurewebsites.net

### Screenshots for Database and APIs

##### 1. Database
Add Address table. In the Address and Student class, add the table relationship. Also, need to add two tables in the data context class.

![alt text](https://github.com/Helena-li/MSA-2020Phase1-backend/blob/master/Images/database.PNG?raw=true)

##### 2. APIs

Basic CRUD requests for the Student and Address table. When adds/update new address, use StudentId to judge the existing Student in the database.
Use automapper to map the classes.
```
public DataAutoMapper()
        {
            CreateMap<Student, StudentViewModel>();
            CreateMap<StudentViewModel, Student>(); 
            CreateMap<Address, AdressViewModel>();
            CreateMap<AdressViewModel, Address>();
        }
 ```

![alt text](https://github.com/Helena-li/MSA-2020Phase1-backend/blob/master/Images/APIs.PNG?raw=true)
