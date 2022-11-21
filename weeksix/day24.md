# Day 24
We are starting to answer the team task.

<aside>
🔐 What is the difference between put in RestAPI and patch? In what circumstances do we use them?

</aside>

In the REST world, PUT and PATCH has different semantics. PUT means replacing the entire resource with given data (so null out fields if they are not provided in the request), while PATCH means replacing only specified fields. For the Table API, however, PUT and PATCH means the same thing. PUT and PATCH modify only the fields specified in the request.