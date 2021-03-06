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

##Integration Testing Via Selenium
- Perform the development setup above
- You must have a selenium-stand-alone server running in order to run these tests.
- You may start this server by running these 3 commands in succession in a separate terminal:
  - npm install -g selenium-standalone
  - selenium-standalone install
  - selenium-standalone start
- If selenium-standalone-server is not running, the test will stall after printing "Running integration tests now"
- You must also have firefox installed in order to run these tests.
- Run 'npm test' from within the 'src' directory.
- A firefox browser should open, and run through/report results of tests for registering, logging in/out, and selecting a playlist
