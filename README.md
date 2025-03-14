# Power-BI_Portfolio
Sample Dashboard to showcase the capabilities and expertise with Power BI

Given is the dataset of all IT tickets raised since 2012 December. The tickets can be categorized as P1- Critical, P2- Very High, P3- High and P4- Standard. P1 is given the highest priority whereas P4 is the lowest priority. A ticket could be high priority (P1 and P2) and still not be a major incident. Major incident means the incident could cause serious disruption to the service

-->The excel workbook contains two sheets (P1&P2 tickets) and (P3&P4 tickets). Please find description of the data in each excel sheet below-

-->P1&P2 tickets: The sheet contains data for all priority tickets. The column ‘Major incident’ indicates whether it is a major incident or not. The ‘Opened’ column indicates the date the ticket was created, the ‘Resolved’ column indicates when the ticket was marked as resolved by IT and the ‘Closed’ column indicates when the ticket was closed either by System based on when it was marked as resolved or closed by the user raising it. ‘Reassignment counter’ indicates how many times the ticket was reassigned to different people in IT before it was resolved and ‘Ticket state’ indicates the latest state of the ticket. ‘Region’ indicates the location of the user who raised the ticket

-->P3&P4 tickets: The sheet contains data for all tickets that are P3&P4 category. It also has tickets that could have reached P1 or P2 status in the lifecycle but were either downgraded to P3&P4 again or continue to stay at P1 or P2. Filter on INCxxx0104 or on INCxxx5443 to understand each situation, respectively. The column ‘Ticket Version’ indicates different versions of a single ticket. Value 0 indicates beginning of the lifecycle and it could go to any number depending on how many times the ticket was updated. With each update, the priority and state could change or remain the same. To see the lifecycle of the ticket, simply sort on ticket version- low to high. ‘Created’ and ‘Update’ are date fields indicating when the ticket was initially created and then contains the date for every time it was updated. ‘Priority New’ indicates the latest priority and ‘Priority Old’ indicates the n-1 priority. When Ticket version is 0, ‘Priority New’ will contain the priority assigned at the beginning of the ticket and ‘Priority Old’ will remain blank. Same applies to ‘Ticket State New’ and ‘Ticket State Old’. There is no expectation to join the two datasets.

-->Use your storytelling abilities to create a storyline and use any chart to visualize the dataset(P1&P2 tickets)
The two graphs however are a must in the page. Cumulative Incidents per region and Incidents per month by Business Service. The X axis should be based on Opened date. Fiscal Year starts in October and ends in September. For example: FY2023 runs from October 2022 to September 2023. I would also like to see the X axis show future date even if there is no data. See example below:
![image](https://github.com/user-attachments/assets/105c6c6e-d5de-4831-bb17-b6e29ce3ccf1)

  

Use the dataset( P3&P4 tickets) to create any interactive visualizations that would be apt to create a storyline
However, the below two charts are a must:
Create a chart to show tickets where the priority was 1 or 2 anytime during the lifecycle AND the final priority is P3 or P4.
Exclude all cases with final priority as P1 or P2.
Exclude all cases with final priority as P3 or P4 and the priority was never P1 or P2 during the lifecycle.
![image](https://github.com/user-attachments/assets/d0dc4195-4af8-47fc-a5fe-29250070bd9c)


-  Analyze the lifecycle of an incident in terms of the priority changes it goes through. For example, if the first status was P4 then it became a P3 ticket and finally   ended at P2 then P4>P3>P2 and plot it in a bar chart per incident. Color coding is as follows. P1- Red, P2- Light Red, P3- Pink, P4- Light pink. Maintain this color coding throughout. Sequence of appearance must also be followed
![image](https://github.com/user-attachments/assets/bbd5f22f-0739-44d3-bc9e-1aff9d1e938a)



