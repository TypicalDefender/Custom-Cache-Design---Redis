# Design Cache From Scratch - (Redis, Memcached)

LLD designs are of two types: Machine coding where you actually build something. And 'Design' where you mention the classes and inheritance/composition relations.

Machine coding is similar to HLD where you clarify requirements of the object you are building, and then move on to code it. It requires some show to executable code.

![sequence diagram cache](https://s3.amazonaws.com/thinkific-import-development/305173/sequencediagramcache-201021-164202.png)

###### Readability

First draw the interaction diagram, and make sure the requirements are clear. You first tell what you'll do, then code it.

Clarify requirements as you go along.

Don't refrain from using the board. It's better to invest 2 minutes for a smooth flow.

###### Correctness

Before you write a major function, define what it does. 

Set 1-2 tests for every major function. This makes you confident of correctness. Try to make the tests runnable (even some examples running in the main function help).

Is concurrency an issue? Most of these cases can't be tested in the limited time, so try to remove such issues. Can you use ordering? Code locks? Data Locks?

Pick one feature at a time. Write a test to confirm.

###### Performance

Look for bottlenecks in your code. You need to be very familiar with time complexities. Code with O(n^2) time complexity is not acceptable.

Most performance problems related to search can be solved using inverse mapping or priority queues. Look at how a map and queue can work together.

###### Tips:

a) Clarify requirements

b) Code in a structured manner and talk them through the process

c) Attack the most critical parts first.

![task scheduler](https://s3.amazonaws.com/thinkific-import-development/305173/Taskschedulerforthreads-201021-164202.png)
![task scheduler](https://s3.amazonaws.com/thinkific-import-development/305173/threadexecutiononmultiplecores-201021-164202.png)
