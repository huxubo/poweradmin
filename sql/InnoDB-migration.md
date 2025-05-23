# InnoDB Migration

These are basic instructions on how to convert your poweradmin database to InnoDB.

## Introduction

This is intended to get you started. If you don't know how to change your MySQL Configuration or don't have basic
understanding on how MySQL works you should look for help.

## Important Notes

Converting the tables to InnoDB is not enough to enable you to enjoy better performance and ACID compliance. You must
configure the InnoDB storage engine appropriately too.

## Recommendations

I recommend you read through [The InnoDB Storage Engine](https://dev.mysql.com/doc/refman/5.6/en/innodb-storage-engine.html)
and set at least the `innodb_buffer_pool` variable to a reasonable value before you attempt to change the database tables.
