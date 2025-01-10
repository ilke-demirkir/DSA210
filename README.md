# DSA210
The Project Repository for DSA 210

Motivation of the project:
The motivation of this project is to see how well I perform as a third-year player on my ultimate frisbee team. I wish to use the data I collect here to correct my mistakes and further improve my game and my performance

Main research questions:

To explain these questions I would like to provide some definitions of ultimate:

Forehand and Backhand throws: There isn't an easy way to explain this other than to say these terms represent throwing motions much like the forehand and backhand in tennis or table tennis. Namely one of these throws is meant to be released from the right side of your body, and the other one is released from the left side of your body.


Aim of the game: The aim in ultimate is to catch the disc in your opponents endzone, you may throw the disc to your teammates any way you wish without foulling your defender. The disc may not touch the ground on offence unless it is within the control of an offensive player. The offense tries to pass the disc around to reach their opponents endzone whlist the defence tries to either catch the disc mid-air or make sure the disc touches the ground while it is in the air. The defence cannot indulge in non-minor contact with the offense and they may not touch the disc while it is in control of an offensive player.

Block: A block occurs when a defensive player intercepts the disc or makes contact with the disc so that it touches the ground. (For example smacking a disc into the ground mid-air is counted as a block)

Completion rate: The following ratio --> Caught passes of Player A / Passes thrown by Player A

Keeping these in mind here are the research questions:
1. How is my forehand pass completion rate compared to the team's?
2. How is my backhand pass completion rate compared to the team's?
3. How is my points+assits+block statistic compared to the team's?
4. How is my overall performance compared to the team's?

Data:
All the data used in this project is collected from the matches uploaded to youtube under the channel Sabancı Seahawks, I watched each game multiple times and collected the data by hand.
[Seahawks.xlsx](https://github.com/user-attachments/files/17933601/Seahawks.xlsx)

Findings: I've plotted the data gathered using polynomial regression, however pulling data from excel itself caused many issues during committing and runtime. The data even when cleaned multiple times proved difficult to gather. Therefore as an alternative Kmeans was used to separete the data across the 6 games data I've displayed. It should be noted that with the increasing number of data commiting the code took significantly longer. I am still working on alternatives methods in order to use the data. In the mean time it should be seen that my performence exceed the team's in every single match, maintain a performance level between 1.5-2.0. The perfomance was measure by the following formula:
Performance = Points + Assits*0.5 + (ForehandCompletion% + BackhandCompletion%) + (Blocks - Drops)*0.5
