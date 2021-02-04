# zoom-analytics #

Now, more than ever, meetings and conferences are happening virtually, primarily hosted by applications such as zoom. It is undeniable that this pattern will accelerate into the future, and businesses will have to adapt to this format, and learn how to capitalize on its unique advantages. One such advantage is that zoom provides complete logs for every meeting. However, these logs are difficult to understand and contain large amounts of useless information. Over the last 7 months I've been working on several ways to turn these logs into meaningful analytics for company meetings and larger events/conferences. The jupyter notebook contains code for 2 tables and 2 visualizations. The first table lists out the exact time that each participant joined and left the meeting. Note that Zoom seems to count clicking away from the meeting screen as leaving the meeting -- you will see several instances of a participant leaving and joining the meeting within one minute. These obviously do not accurately represent meeting attendance, so we find the earliest joining instance and latest leaving instance for each participant. EX: 

[Table 1](images/tab1.png)

The first visualization uses this table to determine how many participants were active during a specified time interval within the meeting. 

[Visualization 1](images/viz1.png)

The second table is an extension of the first, adding the total attendance time as a final column.

[Table 2](images/tab2.png)

The second visualization is exceptionally useful for smaller events, when you want to be able to visualize the participation of each individual in attendance.

[Visualization 2](images/viz2.png)
