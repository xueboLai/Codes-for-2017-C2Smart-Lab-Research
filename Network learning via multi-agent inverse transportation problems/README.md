<h2># 2017SummerResearch</h2>
<h3>This is a python program developed for collecting realtime traffic data to prove the theory in Professor Chow’s paper, “Network learning via multi-agent inverse transportation problems”</h3>
<hr><
<p>
1,The program will randomly pick two directions every five minutes. After picking the directions, we will calculate the travel time of all routes from one direction to another in Queens. The travel times will be stored in regular.csv in output folder. The fastest route (least travel time route) will be saved in the file best.csv.
<br>
<br>
<br>
For example, if we have two directions (From) East and (to) West. “a, b, c, d” are four points in Queens. a,b are the two locations for East direction and c,d are the two locations for West direction. Then, in the regular.csv, we can have
<br><br>
iter num	&nbsp;c&nbsp&nbsp;&nbsp;d<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;a&nbsp;&nbsp;&nbsp	30&nbsp;&nbsp;60<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;b&nbsp;&nbsp;&nbsp	40&nbsp;&nbsp;70
<br>
The table illustrates that from a to c, it takes 30 seconds; from a to d, it takes 60 seconds; from b to c, it take 40 seconds; from b to d it takes 70 seconds.
Please notice that all the numbers have second as unit.
<br>
</p>
<br>
<p>
2, All the numbers of second generated by the program are the real time data from Google Map Distance Matrix API.
</p>
<br>
<p>
3, The log_file_saved is created to store all the intermediate value (printed in console) generated by the program for later debugging purpose.
</p>
<br>
<p>
4, Every five minutes, a screenshot of the fastest route described in 1 will be taken and stored in folder screenshotsOfRoutes
</p>
<br>
<p>
5, Based on the travel time extracted and maps of screenshots in screenShotsOfRoutes, I create a network serving as an integration of the real life traffic in the chosen part in Queens. The network system is in 2017SummerResearch/AssistanceForProfessorChow/TrafficNetworkCreation/new.
</p>