---
layout: post
title:   "Databases"
date:   2016-11-17
categories:   "161"
---

This week's project was overwhelming.  I'm pretty sure we didn't do it 
correctly,but we did our best.  Our biggest problem was that we took a really
long time to figure out how to load data into the database so we weren't able to
ask questions when we actually got stuck.  We ended up working outside of class
until the point where we just couldn't troubleshoot anymore.

I served as the "Database Master" for our group project.  That meant
that I created the database in mysql, using the 'CREATE TABLE' command.  I also
figured out how to set the random ID number as the primary key and found the
command to load all the data into the database. When I found that last command, 
I was so relieved!  We never figured out if we could load the data into the 
mysql database from Todd's or Grace's development environments.

While I was Googling, I found a command that would have allowed me to add users
to my mysql, but there was apparently an error in my syntax that I couldn't
find.  I also found commands that identified my hostname and port.  I thought
that I might have been able to use those to give Todd and Grace access to the 
mysql database, but I didn't find any commands that would let me do that.  
Since Elliott explained that we would have to load the data one-by-one, we
decided that I was barking up the wrong tree.  Still...could it have worked if
I found the right command?

Toward the end, we had a minor crisis when the script in my repository got
deleted.  We were able to restore it, but not without some panicking.  Also,
Todd was denied access to the script for awhile, but he somehow straightened
that out.  In the end, we put directions to manually load the data from Todd and
Grace into the mysql database.  I'm now wondering if we could have used 
mysqlimport and connected to my mysql somehow.  

Unfortunately, it's nearly midnight and I'm going to turn into a pumpkin.

<https://github.com/gma96/braid-assignment-5>

We wrote two scripts.  Everyone who isn't me runs braid0.sh. This script simply 
prompts the user to answer the questions and prints the answers to a .sql file. 
I run braid2.sh, which prompts for the answers, inserts the data into the
mysql database script, then dumps the data into braid0.sql.  Then, I do the 
LOAD DATA command and it loads the data (ignoring any duplicate).  Not so 
simple, but we have a database.



