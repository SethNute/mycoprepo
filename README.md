﻿#Collaborative Music Player

###Authors
- Andrew
- Tony
- Seth
- Amit

##Functional Requirements (Need >= 16 of these)
- Users need to be able to create accounts
- Users need to be able to login to their accounts
- User spends a coin to add a song to the playlist 
- User spends a coin to add a song to the playlist from recommended songs
- User starts tuning into the playlist (listening to whatever is playing)
- User stops tuning into the playlist
- Song user added just played and user gets 1 coin added to their account
- User can adjust volume
- User can choose the genre of the playlist they are listening to
- User can report a song or user for not following proper songs or etiquette
- User votes on top 4 songs in the queue to increase their chance of being played
- Songs that do not get voted on after 10 cycles are removed from the playlist and user is refunded a coin
- Users can type messages to others listening to the same playlist
- Users can look at other users profiles and statistics
- Users can look at leaderboards for top statistics amongst users
- Users can filter the leaderboards 
- Users can click another user's name from chat or leaderboard to go to their profile


##Non-Functional Requirements (Need >= 4 of these)
- Web app that runs smoothly on all modern browsers
- Users data must be secure (usernames and passwords)
- Song playlist should buffer smoothly for >90% of users
- Song playback should be concurrent across all tuned in users
- Chat is updated as messages come in

##Development
- Clone the repository
- Change directories to src
- run the command, 'npm install'
- start mongo on your machine by using the command, 'mongod --fork --syslog'
- run the command, 'npm start'
- head to localhost:8080 to view the web app

##Use Case Testing
- Perform the development setup above
- Navigate to the src directory
- Run the command, 'npm install -g mocha'
- Run the command, 'mocha'

##System Testing
- Perform the development setup above
- You must download selenium-server-standalone-2.x.x.jar from http://docs.seleniumhq.org/download/
- Run the selenium-server-standalone jar you have downloaded.
- You must also have firefox installed in order to run these tests.
- From the 'src' directory, type 'node systemTests.js'