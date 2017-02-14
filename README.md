#Ionic2-benchmark

##1- Ionic 2 Project Structure:

<img src="Ionic-2-project-structure-2.png">
  
* **config.xml** : This contains configurations like the app name, and the package name, that will be used to install our app into an actual device.

* **cordova** :

* **hooks** : These scripts run as part of the Cordova build process. If you need to customize that in any way, then do it here.
  
* **ionic.config.json** : These are your project-specific settings. Primarily it’s just the app name and id along with any proxies you may need for your app.
  
* **node_modules** - Contains the npm packages listed in the package.json file. These are packages necessary for building the ionic app.

* **package.json** : If you are familiar with npm, you will recognize this immediately. If not, then this file describes your app’s production and development dependencies.

* **platforms** : This is where platform specific builds, build tools and packages/libraries are stored. You will find a folder for the platform your are building on. To add a platform, android for example, simply run ionic platform add android, and this will add the folder android folder to this folder.

* **plugins** : This is where cordova plugins will be stored when they are installed. Cordova plugins enables your app to have native functionality in the mobile device, e.g accessing the media storage of the device, or even the bluetooth API.
  
* **resources** : This also contains platform specific resources, such as icons and splash screens.
  
* **tsconfig.json**: N/A
  
* **tslint.json**: N/A

* **/webpack.config.js** : (optional) If you are using webpack for builds then you certainly will need this for adjusting your webpack build settings. If you are not using webpack then, please move on… nothing to see here.

* **/gulpfile.js** : Here you find hooks for modifying the Ionic gulp tasks. Use these to modify the Ionic build. There are a number of custom hooks you can take advantage of. You most likely will not need to modify this file.

* **/app** : Starting with folders, we can see that the bulk of our app lives here: pages, services, etc.

* **/app/app.js or app.ts** : Finally some code! This is where we bootstrap our application and where you will find your app’s @App decorator. There are a handful of global settings you’ll want to pass in. Most importantly, you’ll want to pass your app’s root template, config and list of providers.

* **www**: This is where your index.html file lives. However, don’t be fooled into thinking this is where your app should live. Put all of your application scripts in the ./app folder.

* **www/index.html**: This is obviously where you should update your meta tags and add in any required scripts (cordova, polyfills, vendor build, app build, etc.).
  
