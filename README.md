# Fantasy-Cricket-Game
This project is about the working of the Fantasy Cricket Game where the user has to make a team of 11 players and earn points according to their performance.
It is made using Python, sqlite3, SQLite Studio and QtDesigner.


The project consists of 5 main files –
1) FantasyCricketGame.py : It is the main file which consists of all the information about 
the GUI of the game window along with all the methods and event listener code such 
as to make a team, save it, open an existing team, and evaluate team and lists to 
display the players name when a specific specialty is selected with the points 
remaining and used counter and the number of players selected of a particular 
speciality.
2)EvaluateTeam.py : It is the file which consists of all the information regarding the 
GUI of the dialog window which will appear when the user selects EVALUATE 
Team option in the main window along with all the methods and event listener code to 
select a particular team and match and calculate the final score a user has scored by 
his team.
3) FantasyCricketGame.ui : It contains information regarding the GUI of the game 
window and can be edited easily using QtDesigner.
4) EvaluateTeam.ui : It contains information regarding the GUI of the dialog window 
which will appear after the selection of EVALUATE Team option by the user.
5) TeamInfo.db : It is the database file which consists of 3 or more tables, out of them 2 
are Stats and Teams table and rest are Matches tables. The Stats table consists of 
players’ name, his speciality and all of his stats and records along with points value. 
The Teams table consists of information regarding the teams made by the user. The 
Match table consists of contribution made by players for a particular match.


Working of the Project
1) After specifying the name of the new team we want to make, as we are going to select 
any of the radio button specifying a player’s speciality, the data related to the category 
which is mentioned in ctg column will be fetched from the Stats table of the database 
and will display the list of those players belonging to that category under Players List 
section.
2) After double-clicking a player, the particular player will be added to another list and 
will be removed from the first list. Also the count of the player’s speciality will be 
incremented and the corresponding points will be decreased. The points value of a 
player is fetched from the Stats table under value column.
3) After clicking on OPEN team and specifying the name of the team, the list of players 
belonging to that team will be displayed and is fetched from the Teams table of the 
database. Similarly, SAVE team will store the players name in Teams table along with 
points and name of the team.
4) Clicking on EVALUATE Team will open a dialog window where the final score will 
be evaluated.
5) After specifying Team and Match, when we click on Evaluate Score, the data of the 
player’s contribution for a particular match will be fetched from the table name 
similar to the Match name and according to the conditions given, the individual scores 
will be evaluated. Example – if we select Match1 in dialog window, then the data will 
be fetched from Match1 table only. The match table consists of player name, runs 
scored, balls faced, fours, sixes, balls bowled, maidens, runs given, wickets taken, 
catches taken, stumpings and run outs.
