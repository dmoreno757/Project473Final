# taskyak
This application is designed to use emberjs and a firebase database to create and manage various tasks with a pinterest like layout
## Prerequisites
You will need the following things properly installed on your computer.

* [Git](https://git-scm.com/)
* [Node.js](https://nodejs.org/) (with npm)
* [Ember CLI](https://ember-cli.com/)
* [Google Chrome](https://google.com/chrome/)

## Installation..
* `git clone https://github.com/milesjmccloskey/Project-2-CPSC-473.git`
* `cd Project-2-CPSC-473`

## Running EmberFire and Torii..
* `ember install emberfire`
* `ember install torii`

Change the firebase environment variables within the app/config whereby the user
### Make sure these you have these dependencies
* `ember install ember-cli-bootstrap-4`
* `ember install ember-cli-babel@6.6`
* `npm i ember-easy-dropdown`

### If you have the wrong dependency installed...
you can run the command..
* `ember uninstall"dependency@version"`
then run...
* `ember install"dependency@version"`

###Once the correct dependecies are installed, run...
* `npm install`

## Setting up Firebase....
#### 1) Go to: https://console.firebase.google.com/
#### 2) Add a new project
#### 3) Pick a project name
#### 4) Create it the new Firebase instantiation by clicking 'Create'
#### 5) Click on the new Firebase project
#### 6) On the left.. Go to 'Authentication'
#### 7) Cick "SIGN-IN-METHOD"
#### 8) Set the Email/Password to Enabled
#### 9) Enable users to sign up using their email addresses
#### 10) Enable passwordless authentication with email link
#### Then on the left select Database make sure the rules are set to...
{
"rules": {
".read": true,
".write": true
   }
}
### Configure the Database to start up in Test Mode, then once
### the first data has been populated it shouldn't need rule changes

## Running / Development..
* `ember serve`
* Visit your app at [http://localhost:4200](http://localhost:4200).
* Visit your tests at [http://localhost:4200/tests](http://localhost:4200/tests).

## Running Tests..
* `ember test`
* `ember test --server`

## Linting..
* `npm run lint:js`
* `npm run lint:js -- --fix`

## Building..
* `ember build` (development)
* `ember build --environment production` (production)

## Code Generators..
Make use of the many generators for code, try `ember help generate/g` for more details
#### Routes:
```
* `ember g route about`
* `ember g rout application`
* `ember g route index`
* `ember g route messages`
* `ember g route navbar`
* `ember g route register`
* `ember g route signin`
* `ember g route task-listing`
* `ember g route taskforminput`
* `ember g route welcome`
```
#### Models:
```
* `ember g model user`
* `ember g model tasktaskforminput`
* `ember g model messageinput`
```
#### Controllers:
```
* `ember g controller application`
* `ember g controller index`
* `ember g controller messages`
* `ember g controller navbar`
* `ember g controller register`
* `ember g controller signin`
* `ember g controller taskforminput`
```

## Additional Git Commands
### How to add access and add from a remote branch
### Creates a new branch miles and switches to it...
* `git checkout -b <branch name>`
### Verify you're on the new branch
* `git status`
### Add any changes from the new remote branch to the master
* `git add .`
* `git commit -m "initiating changes from remote branch to master`
* `git remote add origin git@github.com:Razat94/Project-2-CPSC-473.git`
* `git push -u origin <remotebranchName>`
### Switch back to the master
* `git checkout master`
* `git merge <remotebranchName>`
* `git push -u origin master`

### Clone the new repo
* `git clone https://github.com/milesjmccloskey/Project-2-CPSC-473.git`
* `cd Project-2-CPSC-473`
* `npm install`
* `ember install emberfire && install torii`
* `ember test`
### If it doesn't have any compilation errors then..
* `ember serve`
### Also, if you want to clone from the remote branch you can
* `git clone -b <branch_name> git@github.com:Razat94/Project-2-CPSC-473.git`



* `module.exports = function(environment) {`
* ` let ENV = {`
* ` modulePrefix: 'p1',`
* ` environment,`
* ` rootURL: '/',`
* ` locationType: 'auto',`
* ` firebase: {`
* ` apiKey: "AIzaSyDVT8TDcFDZaf8oSWYVI8hbXXQeZbdup3I",`
* ` authDomain: "taskmanager-8f72.firebaseapp.com",`
* ` databaseURL: "https://taskmanager-8****.firebaseio.com",`
* ` projectId: "taskmanager-8****",`
* ` storageBucket: "taskmanager-8**02.appspot.com",`
* ` messagingSenderId: "***********"`
* ` },`
* ` torii: { sessionServiceName: 'session' },`
* ` EmberENV: {`
* ` FEATURES: {`
// Here you can enable experimental features on an ember canary build
// e.g. 'with-controller': true
},
* `EXTEND_PROTOTYPES: {* `
* `/ Prevent Ember Data from overriding Date.parse.`
* `/       Date: false* `

## If you accidently pushed the wrong repo, and need to revert to an old repository state or in other words to the previous commit...
### Enter the command...
* `git log`
### This will display a log of all the recent git commits with their
### corresponding commit SHA-1 ID's, which git uses as its version control
Choose the corresponding commit, and instead of using..
* `git fetch`
We can simply click on commits on the repository bar above the branch names..
Then click the commit  SHA-1 ID, and then click browse files...
Then simply download a zip, or..
* `git clone` from the correct corresponding commit repo

## Deploying the taskyak ember/firebase application
1) Create a heroku account
2) Create a new repo, and import the code from the github repository
3) Publish the heroku project instantiation...
4) Go to: https://<projectName>.herokuapp.com/

# LIVE DEMO:
## https://taskyak.herokuapp.com/
### * [taskyak](https://taskyak.herokuapp.com/)

## Further Reading / Useful Links
* [ember.js](https://emberjs.com/)
* [ember-cli](https://ember-cli.com/)
* Development Browser Extensions
  * [ember inspector for chrome](https://chrome.google.com/webstore/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi)
  * [ember inspector for firefox](https://addons.mozilla.org/en-US/firefox/addon/ember-inspector/)
