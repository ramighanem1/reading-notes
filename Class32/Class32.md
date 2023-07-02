# Django Rest Framework permissions

DRF permissions consist of built-in permission classes that define access rules for API views, determining whether a user has permission to perform actions like retrieving, creating, updating, or deleting a resource. Permission checks are performed based on these classes when a request is made, verifying the user's authentication status and applying additional rules. Authentication, integrated with Django's system, identifies and verifies user identities using various methods. Authorization is handled by DRF permissions, checking user permissions or group membership to grant or deny access to specific actions on resources. By leveraging these components, developers can enforce secure access control, authenticate users, and determine authorization privileges for API operations.

# SELECT statement SQL

In SQL, the SELECT statement is used to retrieve data from a database table or multiple tables. It allows you to specify the columns you want to retrieve, apply filtering conditions, perform calculations, and perform various other operations on the data.

# Django Rest Framework Generic Views 

pre-built views provided by DRF that help simplify the process of building RESTful APIs. They abstract away common patterns and provide default behavior for common API operations, reducing the amount of code you need to write.

Example :

Let's say we have a model called 'Employee' with fields such as 'name', 'email', and 'designation'. We want to build an API that supports listing all employees, retrieving a specific employee by their ID, creating a new employee, updating an existing employee, and deleting an employee.

To achieve this, we can use DRF Generic Views as follows:

```
from rest_framework.generics import ListAPIView, RetrieveAPIView, CreateAPIView, UpdateAPIView, DestroyAPIView
from .serializers import EmployeeSerializer
from .models import Employee

class EmployeeListView(ListAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer

class EmployeeDetailView(RetrieveAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer

class EmployeeCreateView(CreateAPIView):
    serializer_class = EmployeeSerializer

class EmployeeUpdateView(UpdateAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer

class EmployeeDeleteView(DestroyAPIView):
    queryset = Employee.objects.all()
    serializer_class = EmployeeSerializer
    
```



