# AnyLogicSimulation
An IT Support Center for Customers 
The main objective of this activity was to create a simulation model of an IT Support Center using the Any Logic application. To demonstrate the behavior of customers entering the support center, queuing if any of the two technicians/service providers at the support center are busy attending to other customers and exiting the support center once they have been served. The metrics to keep track of are the average waiting time of customers while at the queue, average service time for each customer and the total number of customers served by the two technicians in one hour of simulation. In addition, a comparison was made in terms of the metrics, that is when there was one technician at the support center and while there were two technicians at the support center.



Measurements Taken/Tracked
Key Measurements taken in this simulation are the following:
a.	Average Waiting Time- measures average waiting time by customers at the queue before being served by the technicians.
b.	Average Service Time – measures the average service time for each customer at technicians.
c.	Number of customers served – real time measurement of the number of customers served by the technicians after one hour of simulation.
IT Support Center Simulation Results
Average Waiting Time
The Average Waiting Time of customers at the queue was tracked through the use of additional blocks at the process flow which are:
a.	TimeMeasureStart Block- a building block which is used to store the time when an agent is passed through it. I used it to model the time at which the customer entered the queue.
b.	TimeMeasureEnd Block – a building block that measures the time at which the agent spent inside the specified section of the process flowchart that is after passing the TimeMeasureStart Block. I used it to model the time at which the customer left the queue to be served by the teller. Named as totalWaiting
After which I used a histogram bar graph to model the average times at which customers stay in the queue while waiting for service at the teller. Using the “totalWaiting.distribution()” function. As shown below. With an average Waiting Time of 0 (with customers waiting in the queue between 0.02 minutes and 0.08 minutes from the histogram plot)
 
Average Service Time
The Average Service Time of customers by the technicians was tracked using additional blocks at the process flow which are:
a.	TimeMeasureStart Block- a building block which is used to store the time when an agent is passed through it. I used it to model the time at which the customer entered the technicians’ areas of service. Named as timeServiceStart.
b.	TimeMeasureEnd Block – a building block that measures the time at which the agent spent inside the specified section of the process flowchart that is after passing the TimeMeasureStart Block. I used it to model the time at which the customer left the technicians pool after being served by the technicians. Named as totalService.
After which I used a histogram bar graph to model the average times at which customers stay in the service block while receiving a service from the technician. Using the “totalService.distribution()” function. As shown below. With an average Service Time of 6 minutes per customer (with receiving a service between the times of 6.01 and 6.09 minutes from the histogram plot below)
 

Real Time Number of Customers Served
After one hour of simulation the total number of customers served by the two technicians was 13 customers as per the run window show below in anylogic.
 
Model Screenshots
The following are the screenshots of the process flowchart with the source, timemeasurestart, queue, totalWaiting, timeServiceStart, service, totalService, technicianPool, and sink.
 
And this is the simulation results screenshots after one-hour
![image](https://github.com/user-attachments/assets/6fbed96f-ba1c-4c4d-8502-8186f1479c6c)

 
Conclusion
The Any Logic simulation Application successfully modelled the IT Support center  as per the instructions with Graphical representation of the average waiting times of customers at the queue, real time count of customers being served by the technician and the queue length and the average service Time for each customer and with the comparisons when one technician is serving.

