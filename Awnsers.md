

1. **Scheduling -- Process Selection**
When discussing "When to Schedule" in class, it was mentioned that sometimes scheduling could be improved if an important process could play a role in selecting the next process to run when it blocks. Give a situation where this could be used and explain how.

Überlegen Sie eine Situation, in der das Scheduling eines Systems verbessert werden würde, wenn ein wichtiger Prozess, sobald dieser blockiert, eine Rolle bei der Auswahl des nächsten laufenden Prozesses spielen könnte.

Preemptive: Process runs without interruption for a maximum of some fixed time.

For example, any procces is in an endless loop, then the scheduler will call an other process after a certain time.

2. **Minimizing Turn Around Time**
Imagine the following list of processes in ready state:

| Process |A | B | C | D | E | F | G | H |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
Expected run time (msec) | 8 | 5 | 16 | 12 | 55 | 21 | 2 | 34

Average: 19,125

Turn Around Time: 72

---

How should a scheduler order these processes to minimize average turn around time? What is the minimal average turn around time in the optimal order you found?

| Process |G |B | A | D | C | F | H | E |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
Expected run time (msec) | 2 | 5 | 8 | 12 | 16 | 21 | 34 | 55

Average: 19,125

Turn Around Time: 51,12

You have to sort it, because it reduces the Turn Around Time.

---

3. **Round-Robin Scheduler --- Discussion**
Round-robin schedulers normally maintain a list of all runnable processes, with each process occurring exactly once in the list. What would happen if a process occurred twice in the list?
