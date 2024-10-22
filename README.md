# Brave Rats #
Authors: Abigail Barrientos, Sam Bryant, Ethan Wintill, Laiba Janat, Selah Boyle

## Overview
Brave Rats is a quick, 2 player card game similar to war that is all about reading your opponent. Each player starts with 8 cards and puts one of them down to face the opponent. The card with the highest power usually wins, however each card has a special ability that greatly affects the outcome of the game. The first player to reach 4 victories wins the game.
We have implemented this game in to an online browser card game. Users can play private matches with their friends, or play against a bot to hone their skills.

[![Screenshot 1](https://i.ibb.co/N1rMYk3/Screenshot-2024-10-21-at-8-58-40-PM.png)](https://ibb.co/6v8kspZ)
[![Screenshot 2](https://i.ibb.co/qjg8kSQ/Screenshot-2024-10-21-at-8-58-55-PM.png)](https://ibb.co/V9CG214)
[![Screenshot 3](https://i.ibb.co/D4g0Htr/Screenshot-2024-10-21-at-8-59-19-PM.png)](https://ibb.co/SN7F4Pf)



## Technologies used
- ** Flask **
- ** SocketIO **
- ** Gunicorn **
- ** JQuery **
- ** Bootstrap **

## Setup
- ** Install Dependencies **:
	- `Python`
		- Go to python.org
		- Choose the download for your hardware
		- Ensure download is complete by running "python --version" in your terminal
	- `Clone Project`
		- Create a new directory to install the project
		- Run "git clone https://bitbucket.org/cs3398s23cardassians/brave_rats/src/main/"
		- Ensure all files are cloned on your system
	- `Set Up Environment (optional)`
		- Run "pip install virtualenv"
		- Run "virtualenv venv" to create a new environment in your directory
		- Run "source venv/bin/activate" to enter your virtual environment
	- `Install Project Dependencies`
		- Run "pip install -r requirements.txt" in the root folder of the cloned project
		- After this is complete, you are ready to host a local server
- ** Run Server **:
	- `Using Gunicorn`
		- In your terminal, run the following command to start the server:
		- "gunicorn -k geventwebsocket.gunicorn.workers.GeventWebSocketWorker -w 1 app:app"
		- You should see in the console that the server is running with a url (usually localhost) to visit the site
	- ## Done! You are ready to play on you local machine!
	



## Sprint 1 (OLD PROJECT)
## Contributions
- ** Sam **: "Created UI elements for goal tracking and push notification features"
	- `Jira Task: Design and implement a UI for users to configure their push notification preferences.`
		- bitbucket reference: https://bitbucket.org/cs3398s23cardassians/mot/src/UI-for-push-notification-settings/
		- jira reference: https://cs3398s23cardassians.atlassian.net/browse/MOT-9
	- `Jira Task: Implement push notification functionality based on user preferences.`
		- reference: https://bitbucket.org/cs3398s23cardassians/mot/src/push-notification-functionality/
		- jira referece: https://cs3398s23cardassians.atlassian.net/browse/MOT-10
	- `Jira Task: Design and implement a UI for users to set and manage their goals.`
		- reference: https://bitbucket.org/cs3398s23cardassians/mot/src/UI-for-goals/
		- jira reference: https://cs3398s23cardassians.atlassian.net/browse/MOT-8
	- `Jira Task: Write unit tests to ensure that push notification and goal tracking functionality work as expected.`
		- reference: https://bitbucket.org/cs3398s23cardassians/mot/src/unit-tests-for-push-notifications/
		- jira reference: https://cs3398s23cardassians.atlassian.net/browse/MOT-12
	

## Sprint 2
## Contributions
- ** Sam **: "Designed and implemented backend architecture for seamless multiplayer gameplay"
	- `Jira Task: Add functionality to create a new game on server 
		- bitbucket reference: https://bitbucket.org/cs3398s23cardassians/brave_rats/pull-requests/3
		- jira referece: https://cs3398s23cardassians.atlassian.net/jira/software/projects/BR/boards/3/backlog?issueParent=10049&selectedIssue=BR-49
	- `Jira Task: Handle routes for home page and play page, with respective post requests aswell
		- bitbucket reference: https://bitbucket.org/cs3398s23cardassians/brave_rats/pull-requests/5
		- jira referece: https://cs3398s23cardassians.atlassian.net/jira/software/projects/BR/boards/3/backlog?issueParent=10049&selectedIssue=BR-53
	- `Jira Task: Create socket architecture to recieve input and send output to client
		- bitbucket reference: https://bitbucket.org/cs3398s23cardassians/brave_rats/pull-requests/10
		- jira referece: https://cs3398s23cardassians.atlassian.net/jira/software/projects/BR/boards/3/backlog?issueParent=10049&selectedIssue=BR-50
	- `Jira Task: Implement functionality to use client input in game logic
		- bitbucket reference: https://bitbucket.org/cs3398s23cardassians/brave_rats/pull-requests/8
		- jira referece: https://cs3398s23cardassians.atlassian.net/jira/software/projects/BR/boards/3/backlog?issueParent=10049&selectedIssue=BR-52
	- `Jira Task: Write unit tests to ensure server architecture works as intended
		- bitbucket reference: https://bitbucket.org/cs3398s23cardassians/brave_rats/pull-requests/23
		- jira referece: https://cs3398s23cardassians.atlassian.net/jira/software/projects/BR/boards/3/backlog?issueParent=10049&selectedIssue=BR-54
		

## Next Steps For Sprint 3

- ** Sam **:
	- For this next sprint I will add more features such as user logins and database functionality
	- I will work quickly to ensure that our goals are reached by the end of the sprint

## Sprint 3 
## Contributions
- ** Sam **: "Added database, user implementation, and spectator mode"
	- `Jira Task: Add spectator mode`
		- bitbucket reference: https://bitbucket.org/%7B%7D/%7B74c95d59-a787-4de7-ad93-16c74b62959a%7D/pull-requests/33
		- jira reference: https://cs3398s23cardassians.atlassian.net/jira/software/projects/BR/boards/3/roadmap?selectedIssue=BR-94
	- `Jira Task: Timer for game deletions`
		- bitbucket reference: https://bitbucket.org/%7B%7D/%7B74c95d59-a787-4de7-ad93-16c74b62959a%7D/pull-requests/38
		- jira referece: https://cs3398s23cardassians.atlassian.net/jira/software/projects/BR/boards/3/roadmap?selectedIssue=BR-86
	- `Jira Task: Create SQLite DB with models.py for storing users and previous games`
		- bitbucket reference: https://bitbucket.org/%7B%7D/%7B74c95d59-a787-4de7-ad93-16c74b62959a%7D/pull-requests/27
		- jira reference: https://cs3398s23cardassians.atlassian.net/jira/software/projects/BR/boards/3/roadmap?selectedIssue=BR-88
	- `Jira Task: Connect db to game`
		- bitbucket reference: https://bitbucket.org/%7B%7D/%7B74c95d59-a787-4de7-ad93-16c74b62959a%7D/pull-requests/35
		- jira reference: https://cs3398s23cardassians.atlassian.net/jira/software/projects/BR/boards/3/roadmap?selectedIssue=BR-89


## Next Steps For Sprint 4

- ** Sam **:
	- I want to add cool new features such as a chat box, play timer, and profile picture and username on the play page.
	- I would also want to make the visuals look nicer so it is more presentable to the average person
	- In the future I would like to monetize the game and sell things like skins, themes, profile pics, etc


## Acknowledgements
- This project is based on Brave Rats, by Seiji Kanai. [](https://blueorangegames.eu/en/games/braverats/)
- Brave Rats images and gameplay owned by respective copyright owners.
