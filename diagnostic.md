# Rails API Diagnostic

Place your responses inside the fenced code-blocks where indicated by comments.


What is the purpose of a backend?

```bash
The purpose of a backend is to comunicate from the client to the server/database
with information and requests(CRUD). Based what that request is different
actions are needed and it is the backends job to manage those requests
sucessfully and effectively. If the request is not successful that needs to be
communicated back to the server through the backend as well.
```

Which layer in the MVC pattern is used by the controller to fetch data?

```bash
the model
```

In which part of the MVC pattern can we find C.R.U.D actions?

```bash
in the routes. the routes recives the requests from the clients

```
List at least 5 standard actions that C.R.U.D corresponds to?

```bash
create-both creates and saves
update- patch request
destroy- deletes
index- displays all
show- lists one
new- creates but does not save
```

A user action fires a `PATCH` request for `pets/1`. Explain in detail each step
required for data to be returned to the client. (bullet points or ordered list,
please include information on dynamic segments, the params hash and seralizers).

```bash
-the client sents the patch request
-the routes takes that request to the controller
-the controller tells the model to update the information in the database
-the update happens
-the models relays the change back to the controller
-and the controller updates the server with the request sucessfuul
```

What is the command to scaffold a `medicalRecords` join table which holds
refrences to a `pets` and a `vets` table?

```bash
rails g scaffold medicalRecords references:pets references:vets
```

What is the point of having a join table?

```bash
being able to reference other tables that rely on each other rather than having
columns that repeat themselves
```

Give an example of a one-to-many relationship and a many-to-many relationship:

```bash
many to many:
students to teachers
both students have more than one teacher, and teachers have more than one
student

one to many:
cars
cars have one car-owner
car-owner
but car-owners can have many cars
```
