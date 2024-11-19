System Requirements for Cypress Windows
You will need to download and run Cypress as a desktop application on your computer. Here is a rundown of the OSes that are compatible with Cypress.

macOS 10.9 and above (64-bit only)
Linux Ubuntu 12.04 and above
Fedora 21 and Debian 8 (64-bit only)
Windows 7 and above
If you install Cypress with npm, Cypress supports Node.js 8 and above

Installing Node.js
Before proceeding with the Cypress installation, you must have Node.js installed. Node.js is a JavaScript runtime environment. An IDE (Integrated Development Environment) and a code editor, such as Microsoft’s Visual Studio Code, are also required for programming and managing project directories.

Download NodeJS for Windows 

Running the installer

Installing NodeJS

You can get the Windows installer here. Just run the .msi file to set up Node.js. 
Installing and Setting up NodeJS

Continue to Next and approve the license.
Verifying the installation

The ‘npm package manager‘ is also installed, as shown below.
Verifying Installation of NodeJS

This completes the implementation of Node.js. Once installed, you can validate the version with the command node -version or node -v, as well as the installation of the Node package manager with the command npm -version.

Installing Cypress
Here are two different methods used below to install Cypress in the Windows desktop.

Read More: Cypress Installation for Test Automation: Tutorial

Installing Cypress via npm
Installing Cypress using NPM

You can use npm to install Cypress; to do so, cd into your project directory and run the below command

npm install cypress -save-dev

When you run this, Cypress will be installed for your project as a dev dependency.

Make sure your project directory contains a package.json file or a node_modules folder. By doing this, the proper directory for Cypress’ installation is created.
The Cypress documentation advises using npm to run Cypress because:
In the same way that you would track the version of any other dependency, Cypress also has versions.
Installing npm made it easier to use continuous Integration with Cypress.
Installing Cypress via yarn
To use yarn to install Cypress, cd into your project directory, and then enter the command shown below:

yarn add cypress --dev

Verifying the installation

In addition to downloading Cypress immediately, npm install cypress also adds an entry to the package.json file. When you run -save-dev, the cypress entry in package.json will be saved. As a development dependency, Cypress will be downloaded and installed on your project.

The package.json will still have an entry for cypress even after you move the project cypress test to a different place. Therefore, you only need to run the npm install cypress command, not the full npm install cypress -save-dev command, which only needs to be run once.

Once you open the package.json in the cypress folder, you will see an entry for the cypress software that you have loaded.

Verifying Installation of Cypress


Updating Cypress
Use one of the commands below to launch the Cypress application.

$ ./node_modules/.bin/cypress open

Or

$(npm bin)/cypress open

#Using npx, note: npm > v5.2

$npx cypress open

Updating Cypress

You can see the notice for the updated version (10.8.0), the link for the changelog, and the current version (8.4.1) at the bottom. You can review the changelog for the most recent version if you are not receiving notifications. To see every version, click Changelog.

To view the change logs, click Changelog at the bottom of the runner or go to this link. You can see the features, performance fixes, and bug fixes here, among other things.

The most recent version with the release date will be at the head of the list. You can quickly access the relevant version by clicking on the links on this page’s right side under the section.

 Update Cypress using NPM

npm install --save-dev cypress@10.8.0

Additionally, you can switch the Cypress version to the most recent upgraded version in the package.json

Setting up your first Cypress test
Now that you have Cypress installed, you can run it by

npx cypress open

Select Cypress Testing type

To start, click the “E2E Testing” button on the left.
Next, Cypress will tell you about the different files it will make for you so that everything is set up right for e2e testing. Click on “Continue”.
Next, you’ll see a screen that says “Choose a Browser.” Depending on which browsers you have on your computer, you may have different choices.
Select Browser for Cypress Testing

As you don’t yet have any test files created, Cypress will then launch and prompt you to create your first specification.
Select “Create a new empty spec”: which could be home.cy.ts.

