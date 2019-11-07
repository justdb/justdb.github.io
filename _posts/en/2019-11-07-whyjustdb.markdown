---
layout: post
title:  "Database Migration/Refactoring/Continue Integration Best Practices?"
ref: whyjustdb
date:   2019-11-07 17:38:44 +0800
categories: en justdb database
tags: justdb flywaydb liquibase
lang: en
---
What's the best practices for developers to manage database schemas and data changes?  
The answers are mostly referred to some db change scripts management solutions such flyway or liquibase. With these solutions, developers need to write database delta migration scripts and ordered them in certain orders. You should never ever touch any existing scripts otherwise you may meet some issue. You will not able to see the final database structure until you run these script. You may see the errors you made in your database scripts from the very beginning.  
Is there any solution which can help organize your database refactoring just like what you do with your code?  
We don't find such a solution. That's why we create this project JustDB.  
With JustDB, developers just need to write the final database schemas. They can make any changes to the database schemas, JustDB will do the left to make sure the databases are prepared as needed. What you see is what you get.  
We are working hard on JustDB to make it archived. Stay tuned.
