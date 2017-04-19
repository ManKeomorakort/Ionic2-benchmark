
How to create a module

1.	Run : npm init
	This command will generate your module package.json file

2.	Create a typescript file, put your classes and methods in it
	You can have several typescript files and import classes and methods from 	one to another
	IMPORTANT : make sure to mention export to the class/method you want to 	use elsewhere (ex : export class TestingClass)

3.	Compile your typescript file by running�: tsc filename.ts -d -sourceMap
	It will generate filename.js (javascript)
	-d will generate filename.d.ts
	-sourceMap will generate filename.js.map
	! To run the tsc command, you must have installed npm install -g 	typescript�!

Once you have finished with your module, you have to install it in your application

If you want to compile a package, you must create a tsconfig.json file (run�: tsc --init) at the root of your package, set the compilerOptions (declaration, sourceMap set to true, and inculde/exclude the folders you want to compile). Then compile the package by running�: tsc -w


How to install a module from a local file =

=>	In your project, run : npm install <path>
	Where <path> is the path to your module (ex : "../Test_module")
	Use double quotes (does not work with single quotes)

For more info : https://docs.npmjs.com/cli/install
Your module will be added to node_modules but if you want to add it to the dependencies of your application package.json file you have to run  npm install <path> --save


How to use your module 

=>	Go to the file where you want to use your module and import it (ex : 	import { Restaurant } from 'testmod0/test-module')

You can now use freely your module in your Ionic 2 application
