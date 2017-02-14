#Ionic2-benchmark

##1- Ionic 2 Project Structure:

<img src="Ionic-2-project-structure-2.png">
   
  -**config.xml** : This contains configurations like the app name, and the package name, that will be used to install our app into an actual device.
  
  -**hooks** : N/A
  
  -**ionic.config.json** : N/A
  
  -**node_modules** - Contains the npm packages listed in the package.json file. These are packages necessary for building the ionic app.
  -**package.json** : N/A
    
  -**platforms** : This is where platform specific builds, build tools and packages/libraries are stored. You will find a folder for the platform your are building on. To add a platform, android for example, simply run ionic platform add android, and this will add the folder android folder to this folder.

  -**plugins** : This is where cordova plugins will be stored when they are installed. Cordova plugins enables your app to have native functionality in the mobile device, e.g accessing the media storage of the device, or even the bluetooth API.
  
  -**resources** : This also contains platform specific resources, such as icons and splash screens.
  
  -**src** : This is where we'll spend the most of our time building our app. It contains the structured source code of our app.
  
  -**tsconfig.json**: N/A
  
  -**tslint.json**: N/A
  
