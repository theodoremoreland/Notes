# "Amazon CloudFront is a fast content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to customers globally with low latency, high transfer speeds, all within a developer-friendly environment."

# CDN Networks

## Edge locations
where content is cached. you CAN write and read to/from them

## Origin
the origin of all the files that the cdn will distribute.

## Distributions
the name of the cdn which consists of a collection of edge locations.

### Web distribution
typically for websites

### RTMP
used for media streaming


Objects are timed to TTL (time to live)
Cached content can be cleared (a.k.a. "invalidating the cache), but you will be charged!
Invalidating works must like .gitignore files.
Can take up to an hour to initialize.