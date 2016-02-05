#CoreDevPrototypeEnv

Here are the steps to set up your dev environment.

Install [Eclipse Mars EE Edition](http://www.eclipse.org/downloads/packages/eclipse-ide-java-ee-developers/marsr) if you have not already.

Set up an account on IBM Bluemix. If you dont have an invite ask from Patrick (patrick@cerebri.com).

Follow the instructions to install [IBM Eclipse Tools for Bluemix](https://marketplace.eclipse.org/content/ibm-eclipse-tools-bluemix)

Install [Visual Paradigm](http://www.visual-paradigm.com). Resources to learn Visual Paradigm are on the website. For now install the trial version valid ofr 30 days. If trial period expire contact Jay jay@cerebri.com.

Integrate Visual Paradigm with Eclipse. Go to the Window Tab on Visual Paradigm and select 'IDE Integration'. Select Eclipse. If Eclipse is not installed in the opt[linux] directory you may be unable to install the integration. Restart visual paradigm and try again.

Set up an account on [CircleCI](https://circleci.com/)

Go to IBM Bluemix Console and create app. Select .mybluemix.net as domain.

Clone the directory https://github.com/Cerebri/CoreDevPrototypeEnv.git

Edit the manifest.yml to add the app and host name. This hostname is the same as what you chose for *.mybluemix.net E.g, haad-java.mybluemix.net haad-java is the app and hostname.

If you choose you can rename this directory and PUSH it.

Now in the circleCI account select `ADD PROJECTS` and navigate to the github repo and select it. This forms a tab on your console. Click the repo name and it will direct you to Project Page for your repo. On top right corner select `Project Settings`. In the left panel select `Environment Variables`. Now add two values for USER (ibm Id) and PASSWORD (ibm password). In case you dont like the variable names USER and PASSWORD you can edit the circle.yml file in your directory to reflect the new variable names. After adding variables you can make a change and PUSH again or in the project page select REBUILD.

Once the rebuild is complete you will see "Hello World" on <hostname>.mybluemix.net

