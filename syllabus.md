<!--
1. Syllabus - class grading overview
2. Database Overview (1) - history and choices
	- Network database - Cassandara -
	- Graph database - GraphQL -
	- Flat File database - git
	- Time Series database -
	- Persona (access)
	- Excel - 74% of structured data is in Excel
	- Immutable - Blockchain - Ethereum
3. Database Overview (2) - SQL - how to use
4. Database Overview (3) - bad choices - dead ends
4. Database Overview (4) - Research in DB
	- Distributed - Google F1/BigTable
	- Cockroach DB
	- 
5. Performance and SQL (1) - How queries work
5. Performance and SQL (2) - Local Turing of queries
5. Performance and SQL (3) - Collecting Statistics / Monetering
5. Performance and SQL (4) - Optimization
5. Performance and SQL (5) - Global Optimization
5. Graph QL
5. MongoDB - solution or a problem
6. 
-->
<style>
.pagebreak { page-break-before: always; }
.half { height: 200px; }
</style>

# Class Syllabus: 5825 CoSci Fall 2020.

## Instructor

- Prof Philip Schlump
- Office: Office hours will be on-line using zoom.
- Contact via email (pschlump@uwyo.edu) or (for emergencies only): 720-209-7888 (my cell)
and pschlump@gmail.com (personal email).
- Class Time:  Lectures are online and pre-recorded.  We will have a mix of discussion and one-on-one time during class.
If your schedule will not permit getting together during a discussion time then we will schedule individual one-on-one 
time. xyzzy M/W/F 1:10 PM to 2:00 PM.

If you want to call me to set up an appointment you will need to send me a SMS message
first so that I enter your name into my contact list.  I get 20+ robo-calls a day and
I will not answer a random number.  Text me with your name and that you are a student
in 5825 class.

## Required texts

*Important! I will bring the textbooks to class.*

PostgreSQL 10 High Performance: Expert techniques for query optimization, high availability, and efficient database maintenance Paperback – April 30, 2018
by Ibrar Ahmed (Author), Gregory Smith (Author), Enrico Pirozzi (Author).  

*Do not just go off an order a copy of the book for yourself!  I have copies of the book for you!  I will bring them to class.*

## Required Projects

Most of the class grade comes from the homework.

## Final Examination

Final is Friday, December 20 1:15 pm - 3:15 pm.   Location to be determined, but probably in the same room as class.

## Extra credit

No extra credit is planned at this time.

<div class="pagebreak"> </div>

## Office Hours 

From 12:30 to 1:30 Tu/Th - except the following dates:
Sep 12, Sep 26, Oct 10, Oct 24, Nov 7, Nov 21, Dec 5.  
Other times via an appointment.

I am planning on office hours at the convenience of this class.

## Grading

Your grade is from the Projects, 2 Tests (Midterm and Final) and the paper.

| Title                                         | Points  |
|-----------------------------------------------|---------|
|  HW 0 - Install PostgreSQL (Hello World)	    |         |
|         Sample data will be provided.  	    | 50 Pts  |
|                                               |         |
|  HW 1 - Benchmark System	                    | 100 Pts |
|  HW 2 - Disk Setup Tests	                    | 100 Pts | xyzzy
|  HW 3 - Storage Config / Disk Config	        | 100 Pts | xyzzy
|  HW 4 - Install MongoDB, Redis                | 50 Pts  |
|  HW 5 - Triggers / Proc / Views / Materialized	            | 200 Pts |
|  HW 6 - Blockchain in PG	                    | 200 Pts |
|  HW 7 - Query Performance Tuning                   | 300 Pts |
|  HW 8 - Implement No-SQL in PostreSQL                      | 300 Pts |
|                                               |         |
| Midterm                                       | 400 Pts |
| Final                                         | 400 Pts |

Total: 2200

| Points                                      | Letter Grade  |
|---------------------------------------------|---------------|
| From 1800 to 2200                           | A |
| From 1600 to 1800                           | B | 
| From 1400 to 1600                           | C | 
| From 1000 to 1400                           | D | 
| From 0 to 1400                              | F | 






<div class="pagebreak"> </div>

## Overview

This is an approximate schedule.  Updates will be noted in class.  
Most Fridays we will be comparing database choices. 

| Date     | No | Description                                                                       |
|----------|----|-----------------------------------------------------------------------------------|
| Sep 4    | 01 | Introduction to class.                                                            |
| Sep 6    | 02 | My background in database performance.                                            |
|          |    |                                                                                   |
| Sep 9    | 03 | The Database *Landscape*  (Ch 1 & 2 from book) Homework 0 - Install.              |
| Sep 11   | 04 | Life cycle of database systems - where you come into the picture.                 |
| Sep 13   | 05 | To ORM or not to ORM / Existing Packages / Reports                                |
|          |    |                                                                                   |
| Sep 16   | 06 | (Ch 3 - Disk Benchmarking)  Homework 1 - Benchmark Your System.  Hw 0 Due.        |
| Sep 18   | 07 | Database Design  - Tables ERD - Modeling                                          |
| Sep 20   | 08 | System Design - Multiple Caching Layers                                           |
|          |    |                                                                                   |
| Sep 23   | 09 | (Ch 4 - Disk Setup) - Homework 2 - Testing Disk Setup. Hw 1 Due.                  |
| Sep 25   | 10 | Testing Setup                                                                     |
| Sep 27   | 11 | AWS / Azure / GCP performance and Database                                        |
|          |    |                                                                                   |
| Sep 30   | 12 | (Ch 5 & 6 - Memory - Server Config) - Homework 3 - Disk Config Hw 2 Due.          |
| Oct  2   | 13 | Alternatives to SQL Database Storage.                                             |
| Oct  4   | 14 | Install Mongo DB, Redis - Homework 4.                                             |
|          |    |                                                                                   |
| Oct  7   | 13 | Homework 5 - Triggers / Stored Proc. / Views etc.  Hw 4 Due.                      |
| Oct  9   | 14 | Denormalization for Performance / Triggers and Materialized Views.                |
| Oct 11   | 15 | Midterm Review (Topics from Ch 1..6 of book) Hw 5 Due.                            |
|          |    |                                                                                   |
| Oct 14   | 16 | Midterm                                                                           |
| Oct 16   | 17 | Query Performance / Explain Plans / Tuning Queries                                |
| Oct 18   | 18 | Automating in PG Query Tuning (Oracle, etc)                                       |
|          |    |                                                                                   |
| Oct 21   | 19 | Docker and Database                                                               |
| Oct 23   | 20 | Database Fragmentation and Vacuum.                                                |
| Oct 25   | 21 | Comparison of PostgreSQL to MongoDB.                                             |
|          |    |                                                                                   |
| Oct 28   | 22 | Blockchain as a Database (Homework 6)                                             |
| Oct 30   | 23 | Connection Pooling.                                                               |
| Nov  1   | 24 | Comparison of PostgreSQL to Redis                                                 |
|          |    |                                                                                   |
| Nov  4   | 25 | Hw 6 Due.  Homework 7 - Find the slow query.                                      |
| Nov  6   | 26 | Overview of Real Applications                                                    |
| Nov  8   | 27 | Comparison of PostgreSQL to Oracle.                                               |
|          |    |                                                                                   |
| Nov 11   | 28 | Caching Layers. ( From Client to Storage and Back )                               |
| Nov 13   | 29 | Hw 7 Due.   Homework 8 - Redis Based Caching.                                     |
| Nov 15   | 30 | Comparison of PostgreSQL to DB 2 Universal.                                       |
|          |    |                                                                                   |
| Nov 18   | 31 | Applying a Learning System to Query Performance.                                  |
| Nov 20   | 32 | Applying a Learning System to Query Performance.                                  |
| Nov 22   | 33 | Comparison of PostgreSQL to MySQL.                                                |
|          |    |                                                                                   |
| Nov 25   | 34 | Comparison of PostgreSQL to Microsoft SQL Server.                                 |
|          |    |                                                                                   |
| Dec  2   | 35 | Hw 8 - Due.                                                                       |
| Dec  4   | 36 | Overview of where database is headed.                                             |
| Dec  6   | 37 | Comparison of PostgreSQL to Cassandra.                                            |
|          |    |                                                                                   |
| Dec  9   | 38 | Catch up Lecture 1.                                                               |
| Dec 11   | 39 | Catch up Lecture 2.                                                               |
| Dec 13   | 40 | Final Review.                                                                     |










## Late work.

Generally it is a good idea to get the homework done one time.
 

                         

## Title IX – Duty to Report
 
The University of Wyoming faculty are committed to helping create a safe learning environment for all students and for
the university as a whole. If you have experienced any form of gender or sex-based discrimination or harassment,
including sexual assault, sexual harassment, relationship violence, or stalking, know that help and support are
available. The University has staff members trained to support survivors in navigating campus life, accessing health and
counseling services, providing academic and housing accommodations, and more. The University strongly encourages all
students to report any such incidents to the University. Please be aware that all University of Wyoming employees,
including student staff, are required to report all Title IX related concerns to the Title IX Coordinator or their
supervisor. This means that if you tell a faculty member about a situation of sexual harassment or sexual violence, or
other related misconduct, the faculty member must share that information with the University’s Title IX Coordinator.
UW’s Title IX Coordinator is Jim Osborn (Manager of Investigations, Equal Opportunity Report and Response). He is
located in Room 320 of the Bureau of Mines Building, and can be reached via email at report-it@uwyo.edu or via phone at
766-5200 or 766-5228. For more information, go to:
[http://www.uwyo.edu/reportit/learn-more/faqs.html](http://www.uwyo.edu/reportit/learn-more/faqs.html) .

## Attendance and Absence policies

Attendance is critical.  The only way to know what you need to know is by
attending class. If you have an excused absence that is fine, try to get notes from the day you missed from one of your
classmates. Just don't skip!

## Classroom Behavior Policy

At all times, treat your presence in the classroom and your enrollment in this course as you would a job. Act
professionally, arrive on time, pay attention, complete your work in a timely and professional manner. You will be
respectful towards your classmates and instructor. Spirited debate and disagreement are to be expected in any classroom
and all views will be heard fully, but at all times we will behave civilly and with respect towards one another.
Personal attacks, offensive language, name-calling, and dismissive gestures are not warranted in a learning atmosphere.
As the instructor, I have the right to dismiss you from the classroom.

## Classroom Statement on Diversity

The University of Wyoming values an educational environment that is diverse, equitable, and inclusive. The diversity
that students and faculty bring to class, including age, country of origin, culture, disability, economic class,
ethnicity, gender identity, immigration status, linguistic, political affiliation, race, religion, sexual orientation,
veteran status, worldview, and other social and cultural diversity is valued, respected, and considered a resource for
learning. 

## Disability Support

If you have a physical, learning, sensory or psychological disability and require accommodations, please register as
soon as possible and provide documentation of your disability to Disability Support Services (DSS), Room 109 Knight
Hall. You may also contact DSS at (307) 766-3073 or udss@uwyo.edu. Visit their website for more
information: www.uwyo.edu/udss

## Academic Dishonesty Policies

Don't cheat on the exams. I expect you to take full advantage of all the online resources you can get your hands on.
That includes Stack Overflow, Github etc. If you do use someone else's code, put in a link to where you found it.
Don't cheat on the projects - do you own work.  Most of the learning in the class is from *doing* the projects.

## Substantive changes to syllabus

All deadlines, requirements, and course structure are subject to change if deemed necessary by the instructor. Students
will be notified verbally in class, on our WyoCourses page announcement, and via email of these changes. I do travel
during the semester. Class could be canceled or assignments due dates changed.

# Copyright

Copyright (C) University of Wyoming, 2020.
