# NurseScheduler
Automated Nurse Schedule creator using google ortools api. A subset of the employee scheduling problem, an NP complete problem.

Constraints:
1. Only qualified staff with the right skill can take on a duty
2. Staff can be assigned at most one duty per day done; no overlapping duties
3. Avg working hours per week should not exceed 44 hours a week
4. Number of duties per day per skill must be done according to the specification
5. Staffs on Leave cannot work
6. The staff that work the longest hour cannot work more than 8 hours than the staff that work the shortest


Schedule_sample.JSON parameters:

1. Staff - id, name, designation
2. Skills - id, name
3. Staff_Skills - staff_id, skill_id
4. Duties - id, name, type, category, duration (hours), pattern
5. Shift_duties - id, name, shift_number (represent how many nurses need to be present for that duty on a 14 days period)


