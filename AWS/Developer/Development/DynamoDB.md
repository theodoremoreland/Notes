## Sections
- Components
- Data Consistency
- Throughput
- DynamoDB Streams
- DynamoDB Accelerator
- Global Tables
- Auto Scaling Triggers
- Keys

## Links

https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/HowItWorks.CoreComponents.html

# Components

In DynamoDB, tables, items, and attributes are the core components that you work with. A table is a collection of items, and each item is a collection of attributes. DynamoDB uses primary keys to uniquely identify each item in a table and secondary indexes to provide more querying flexibility. You can use DynamoDB Streams to capture data modification events in DynamoDB tables.

### Tables
### Items
### Attributes

# Data Consistency

### Can specify eventually consistent vs strongly consistent

* runs exclusively on SSD

* secondary keys?

# Throughput

### Read Capacity Units (RCU)
Number of strongly consistent reads per second or two eventually consistent
reads per second, for items up to 4kb in size (eventually consistent reads use half the the provisioned read capacity)

### Write Capacity Units (WCU)
Number of writes per second, up to 1kb in size.

### Pages, Scan Operations

# Dynamo DB Streams

# DynamoDB Accelerator

# Global Tables

Stores 3 geograhically distributed replicas of each table to enable high availablity and performance.

