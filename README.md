Lovely Professional University
Course code: INT404
Course Name:Artificial Intelligence
TOPIC: INTELLIGENT TIME TABLE GENERATOR
Registration No:11803306 Ansh Rao
11803351 Sishu Tiwari
11803331 Tanush Angural
Submitted to: Dr. V Devendran
Solution:
This project implements one of possible solutions for generating university schedule. The proposed
solution is based on methods of evolutionary computing, uses (1+1) evolutionary strategy and
simulated hardening. The success of solution is estimated on fulfillment of given constraints and
criteria. Results of testing the algorithm show that all hard constraints are satisfied, while additional
criteria are optimized to a certain extent.
Problem
The assignment is to find generic solution that will facilitate generating schedule for university.
Each class on faculty is represented as block (lasts arbitrary number of hours, mostly form 1 to 4).
For conducting every class required are: teacher, classroom, start time, duration and groups which
attend the class. It is also know in advance which groups attend which class and all classrooms are
the same size (each group can fit to a classroom).
Teaching is done on faculty from 9AM until 9PM on each work day.
Input data for each class are teachers’ name, subject, type, duration and list of allowed classrooms.
Output data are classroom and time for each class. Time is determined by day (Monday to Friday)
and start hour of the class.
Constraints
1. Resources can not overlap timewise
• No teacher can hold two classes at the same time
• No group can listen for two classes at the same time
• No classroom can receive two classes at the same time
Note: under the term "same time" is not meant only at the beginning of the class,
it should be taken into account the duration of the class. If the resource is busy at
the moment T1 and the class lasts t1, then the resource can only be re-occupied
at the moment T2 = T1 + t1.
2. Class should take place in one of the allowed classrooms
3. If the subject has several forms of teaching, the preferred order for each group is the
lectures, exercises, and laboratory exercises.
Constraints 1 and 2 must be met, while the 3rd limit is "soft" and allowed to be violated.
Additional criteria for estimating solution (used also for cost function):
• Fulfill hard constraints (1 & 2)
• Fulfill soft constraints (3)
• Minimize total "idle" for each group (eliminating pause between classes)
• Minimize total "idle time" for each teacher (elimination of pause between classes)
• Provide one hour on a teaching week where no one has classes
