https://www.meteor.com/tutorials/angular/creating-an-app

To create the app, open your terminal and type:

meteor create simple-todos
This will create a new folder called simple-todos with all of the files that a Meteor app needs:

client/main.js        # a JavaScript entry point loaded on the client
client/main.html      # an HTML file that defines view templates
client/main.css       # a CSS file to define your app's styles
server/main.js        # a JavaScript entry point loaded on the server
package.json          # a control file for installing NPM packages
package-lock.json     # Describes the NPM dependency tree
.meteor               # internal Meteor files
.gitignore            # a control file for git
To run the newly created app:

cd simple-todos
meteor

To open the app, simply open your web browser and go to http://localhost:3000 to see the app running.

To use Angular in our app, we first need to remove the default UI package of Meteor, called Blaze.

We remove it by running:

meteor remove blaze-html-templates
Now we need to replace it with UI package for angular:

meteor add angular-templates
To start working with angular-meteor, let's add some NPM packages.

meteor npm install --save angular angular-meteor
Note: meteor npm supports the same features as npm, though the difference can be important. Consult the meteor npm documentation for more information.
