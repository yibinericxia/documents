1. Schedule consideration

The time factor plays an important role in project delivery. If the schedule is tight, you may have to consider to share the common database as it is instead of having your own, so that you can move your data access layer (jpa/jdbc) from the monolith to the microservice easily without much efforts.

2. Boundary consideration

How to divide the domains into different service components are critical.

3. Database consideration

Ideally each microservice should have its own database so that its database schema or schemas out of the microservice can be changed independently. If the databasee is shared with other microservices or applicatons, it is recommended to use low level database operation, such as jdbc instead of jpa for relational database.

If the binary content is stored in database, it can be a good time to move it to the cloud blobs storage and store its URI in database.

4. Deployment consideration

Good for both production deployment and local debugging. 
