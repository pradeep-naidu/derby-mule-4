# derby-mule-4
Repository on how to use derby with mule 4

In this code base we will see the use of Derby database (https://db.apache.org/derby/)  as temporary data store solution or can also be considered for use as database, until the actual database is provisioned.

For the use case, let’s consider having a mule flow which has to provide endpoints so that any field device (mobile) can send the data, the flow then publish the data to a JMS queue.

Another flow in the mule application consumes the JMS message and insert into the database for future use, At this point we can use the Derby as database solution till we get the actual database.

Let’s have another flow which will pull the data from Derby database on demand.

Below is a diagram to give you an understanding of the data flow.


![alt Use Case](https://raw.githubusercontent.com/pradeep-naidu/derby-mule-4/master/use-case.png)
