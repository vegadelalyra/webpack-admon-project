# webpack-admon project
## Tired of deal with <br> webpack.config.js file <br> writting code lines for each dependency, loader or plugin you install? <br><br> webpack-admon does it for you!
The idea is to create a npm package of CLI commands that automates the written of the webpack.configuration.js file just from terminal. <br><br>
This would be an example of the wished experience with this dependency: <br><br>
**npm i webpack-admon  :**   installs our package. <br><br>
**webpack-admon init   :**    automatically runs npm i "all typical dependencies for a typical website project (let's say @babel/core babel loader copy-webpack-plugin html-webpack-plugin webpack webpack-ci webpack-dev-server css-loader styles-loader, etc)" and creates || updates our webpack.config.js file with the typical configurations for each of these dependencies/loaders/plugins <br><br>
**webpack-admon custom :** user can define which dependencies are going to be executed at "webpack-admon init" command in a text editor <br><br>
**webpack-admon list :** will display the webpack-admon dependencies that will be installed with webpack-admon init, customizables with webpack-admon custom command.<br><br>
**webpack-admon config "dependency-name":** User can define the default settings **for any existing dependency** || installed dependency (if form is too hard to do). <br><br>
**webpack-admon update :** user new custom settings are added to his/her webpack.config.js file. <br> <br> 
**webpack-admon "dep name":** will install the indicated dependency with the default settings webpack-admon has or the custom settings the usar registered for that dependency with the "webpack-admon config 'anyDep'" command. If webpack-admon haven't registered default settings for any given dependency, it will just execute the npm i "non-registered dependency name" command and will prompt to the user something like "No default settings for "dependency name", set them up with webpack-admon config "namedep", so user can save time in futures projects. <br><br><br>
_____________________________________________________________________________________________________ <br> <br>

How hard can this be, right? 
