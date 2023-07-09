# Lockout-Tournament Discord Bot
<img src="https://github.com/Ayush-721/Lockout-Tourney-Bot/assets/95296019/348642b7-22b7-44d8-afbc-d37b685ee12b" alt="Image" width="60%">

This is a [Python](https://www.python.org/) based Discord bot which helps to organise tournaments and conduct 1v1 programming matches. The bot can handle scheduling and organisation of the fixtures.</br>
We used the [Codeforces](https://codeforces.com/apiHelp) API for fetching questions and also check for submissions in real time while conducting the matches itself. We used  [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/) for web scraping to get the support of  [AtCoder](https://atcoder.jp/)  judge.
We tried to create user-friendly interface, allowing participants get to validated and compete in tournaments. All of these features were integrated with the help of [discord.py](https://discordpy.readthedocs.io/en/stable/) library.

# Features
* <b>Competitive Programming Judges supported: </b>[Codeforces](https://codeforces.com/) and [Atcoder](https://atcoder.jp/).
* <b>Validation of Handles: </b> Validate a handle by making a request to the <b>"user.info"</b> method of the Codeforces API and checking the response for user information for Codeforces Handle Verification. Also no. of permissible accounts for a particular judge is limited by <b>1</b>.
* <b>Show ongoing Matches: </b> Provide user with the list of all ongoing matches in the particular tournament.
* <b>Start Match:</b> Starts a lockout based match between the users(if both are <b>registered</b>) and asks for a time in minutes in [10-180) for that round, and presents the users with a set of <b>5</b> questions which neither of them have previously attempted.
* <b>Match Updates:</b> Shows the status of problems solved and remaining time for the particular round.
* <b>Problems Presented:</b> Takes in an input value for the rating of the first problem for the user, and the problems presented are of rating <b>x, x+100, x+200, x+300, x+400</b> where <b>x</b> is the value input by the user.
* <b>Show Participants: </b> Gives the list of participants in a particular tournament along with their [Codeforces](https://codeforces.com/) and [Atcoder](https://atcoder.jp/) profile's max ratings.
* <b> Show Matches: </b> Provides user with the fixture of matches to be played in the ongoing tournament. This fixture is built by using the method of <b>Single Elimination Tournament</b> with byes given in case of an unsymetric number of participants in the particular round.

The commands for all these features and their usage can be retrieved by executing the command !help in the server.
