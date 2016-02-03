#CoreDevPrototypeEnv

Here are the steps to set up your dev environment.

Install [Eclipse Mars EE Edition](http://www.eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/marsr) if you have not already.

Set up an account on IBM Bluemix. If you dont have an invite ask from Patrick (patrick@cerebri.com).

Follow the instructions to install [IBM Eclipse Tools for Bluemix](https://marketplace.eclipse.org/content/ibm-eclipse-tools-bluemix)

Install [Visual Paradigm](http://www.visual-paradigm.com). Resources to learn Visual Paradigm are on the website. For now install the trial version valid ofr 30 days. If trial period expire contact Jay jay@cerebri.com.

Integrate Visual Paradigm with Eclipse. Go to the Window Tab on Visual Paradigm and select 'IDE Integration'. Select Eclipse. If Eclipse is not installed in the opt[linux] directory you may be unable to install the integration. Restart visual paradigm and try again.

Set up an account on [CircleCI](https://circleci.com/)

Go to IBM Bluemix Console and create app.

Clone the directory https://github.com/Cerebri/CoreDevPrototypeEnv.git

Edit the manifest.yml to add the app and host name.

Edit the circle.yml to add your Username and Password. I am trying to figure out how to use secret keys so you dont have to push your username and password.