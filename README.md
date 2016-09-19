
![](https://github.com/jenjwong/Read-With-Me/tree/master/documentation/screenshot.png)
## Team
* **Ashwini Jogwar** - Product Owner
* **Cathy Lee** - Scrum Master
* **David Doan** - Software Engineer
* **Jen Wong** - Software Engineer

### Deployed MVP:
http://159.203.213.49:8000

### Requirements
* node.js - v6.2.0
* mongodb
* Go to Twilio's site and follow directions at (https://www.twilio.com/docs/api/ip-messaging/guides/quickstart-js) to create a Twilio account to get SID and API keys

### Description
*Read With Me* is a remote reading app, that allows parents who are away from their kids to interactively read and webcam with them online. Both parties can draw on the storybook, navigate pages, and make each page image animate.

### Installing Dependencies

From the root directory run:
```
npm install
npm install -g nodemon webpack
webpack --watch
mongod
nodemon server.js

//visit localhost:8000 in the browser.

```
### Seeding the Database
```
1. go to postman
2. make a post request ONLY ONCE to http://localhost:8000/api/books
3. comment all the stuff that you just uncommented.
4. save the bookController.js


```
### Testing
Client side testing is implemented with Karma and Airbnb's Enzyme framework. Developers can pinpoint the source of their errors's using Enzyme's shallow rendering and Karma's sourcemap. Server side testing is implement with Supertest and Chai.


From the root directory run:
```
npm test
