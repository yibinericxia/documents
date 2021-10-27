1. Schedule consideration

The time factor plays an important role in project delivery. If the schedule is tight, you may have to consider to share the common database as it is instead of having your own, so that you can move your data access layer (jpa/jdbc) from the monolith to the microservice easily without much efforts.

2. Boundary consideration

How to divide the domains into different service components are critical.

3. Database consideration

Ideally each microservice should have its own database.

4. Deployment consideration

Good for both production deployment and local debugging. 
