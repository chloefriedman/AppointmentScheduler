# Appointment_Scheduler-Student
﻿SMART APPOINTMENT SCHEDULER - STUDENT STARTER
=============================================


CONTENTS (all in ONE folder when extracted)
  Appointment.java             - PROVIDED; do not edit
  AppointmentScheduler.java    - FIVE TODO methods to complete
  SchedulerMain.java           - PROVIDED console menu and startup/save I/O
  data/seed_schedule.txt       - starting schedule; do not edit
  BST_Appointment_Scheduler_Student_Directions.docx - assignment


SETUP
1. Extract this ZIP to a new folder.
2. In VS Code, File > Open Folder, and select THAT folder directly.
   The data folder must be in the same folder as the three .java files.
3. Run SchedulerMain.java (or in the terminal: javac *.java && java SchedulerMain).
4. Expected first message: Loaded 5 appointments from data/seed_schedule.txt


ONLY EDIT AppointmentScheduler.java.
The menu and initial file loading work before any TODO methods are completed.
Saving will not overwrite an earlier saved file until write() is implemented.
When working, save writes data/saved_schedule.txt; the next run loads that first.


ALL TIMES ARE 24-HOUR HH:MM. This is a single-day calendar, 08:00 to 17:00.

1) How does a TreeSet differ from an ArrayList in how it stores and organizes elements?
  A tree set stores them in an order by natural order and it is not linear. The tree set also only adds unique values. It is a self balancing binary search tree.
2) What does the floor() method return? What does floor() return if there is no appointment starting at or before the requested time?
The floor method returns the biggest value smaller than the requested element and null otherwise
3) What does the ceiling() method return? What does ceiling() return if there is no appointment starting at or after the requested time?
The smallest value greater than the requested element and null otherwise
4) Why might these methods be useful in an appointment scheduling program?
  In creating the order and making sure there is time for an appointment in between the values the methods return
      5. Suppose our calendar contains these appointments:
Start
End
9:00 AM
9:40 AM
10:15 AM
11:00 AM
11:30 AM
12:00 PM

  
If we attempt to schedule an appointment beginning at 10:00 AM, which existing appointments would floor() and ceiling() return, assuming appointments are ordered by start time?
Floor would return 9:40 and ceiling would return 10:15