# Caching

## What is cache?
Generally, cache in computer science is a small,fast storage device (or it could be a software component as well) that acts as a staging area for the data objects stored in larger, slower devives. Caching increases the read speed drastically. The using of cache is known as *caching*.

Cache is basically *SRAM* (Static Random Access Memory), which is a volatile memory. It means that the data is there as long as the device has power, or is turned on. 


When the data that need to be read is present in the cache, it is called as **cache hit**, else it is called as a **cache miss**.

## Cache Types
Caching has numerous applications, across many platforms and many domains.Some different types of cache are :
* Hardware Cache
    * CPU Cache
    * GPU Cache
* Network Cache
* Software Cache
    * Disk Cache
    * Web Cache

## Caching Matters!
Cache is one of the most effective strategies to improve the application performance. Caching can be applied to any type of relational databases like **NoSQL** or **Amazon RDS**.
By using caching the scale and the speed is significantly improved.\
\
The traditional _disk-based_ databases can decrease the peformance when our application requires scalability and low latency. Those include __slow processing speed__ , **non-optimal data access** etc.\
\
The way the caching improves performance is by supplementing the primary database by removing unnecessary pressure on it in the form of quite frequently accessed read data. The cache can live in a number of areas , including the database , application or as a standalone layer.


## Types Of Database Caches
* **Database Integrated Caches** :\
It is integrated cache that is managed within the database engine and has built in write-through capabilites. It updates its cache automatically , when the data changes on the database table




* **Local Cache**:\
It stores the frequently used data on the application itself.This removes the network traffic associated with retrieving data. But the downside is that when outage occures, the data in the local  cache is lost
 

* **Remote Cache**:\
These are caches stored on the servers and are built upon *key/value NOSQL* stores such as **Redis** and **Memcached**. They provide hundreds of thousands to up to a million requests persecond per cahce nodee.


## Redis
Redis, which stands for Remote Dictionary Server, is a fast ,open source , in-memory key-value data store for use as a database, cache ,message broker and queue. \
\
All Redis data is stored in-memory, unlike databases that store data on disk or SSDs.This avoids seek time delays due to not needing to access disks, and data can be accessed in microseconds. Redis uses versatile data structures and provides cluster support makin it simple to build real-time internet scale apps.

## Memcached
Memcached is yet another general purpose distributed memory-caching system. It is often used to speed up dynamic database-driven websites by caching data and objects in RAM to reduce the number of times an external data source (such as a database or API) must be read.

## Redis vs Memcached
When performance needs to be improved, caching is  the first step taken, and Memcached or Redis are typically the first places to turn. Both share a number of similarities , but also have many differences. Since the Redis is the new one and is more *versatile* of the two, it is usually preffered over the Memcached.  
  

**Memcached**, a *high-performance* distributed memory cache service, is designed for simplicity while **Redis** offers a rich set of features that make it effective for a wide range of use cases.  
___
### References:
* Computer Systems A Programmer's Perspective by Randal E.Bryant and David R Hallaron
* https://en.wikipedia.org/wiki/Cache_(computing)
* https://aws.amazon.com/caching/database-caching/
* https://en.wikipedia.org/wiki/Redis#Differences_from_other_database_systems
* https://en.wikipedia.org/wiki/Memcached
* https://aws.amazon.com/redis/
* https://www.infoworld.com/article/3063161/why-redis-beats-memcached-for-caching.html
* https://stackoverflow.com/questions/25802521/difference-between-in-memory-databases-and-disk-memory-database