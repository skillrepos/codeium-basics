
# Codeium Basics - lab setup

These instructions will guide you through configuring a GitHub Codespaces environment that you can use to run the course labs. Because of issues with using Codeium directly through a codespace though, we will need to use VS Code as the front end. 
If you prefer and if you know one of the other IDEs supported by Codeium, you can use that. But the instructions will reference the codespace version.

These steps **must** be completed prior to starting the actual labs.

## Step 1. Install VS Code on your system from the link below:

<br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Install VS Code]
(https://github.com/skillrepos/codeium-basics/images/vscode.svg)](https://code.visualstudio.com/download)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Install VS Code](https://github.com/skillrepos/codeium-basics/blob/main/images/vscode.svg)](https://code.visualstudio.com/download)

## Step 2. To create your working environment for the labs, create a codespace by clicking on the button below:

Click on this button ⬇️
<br/><br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/skillrepos/codeium-basics?quickstart=1)

<br/><br/>
Then click on the option to create a new codespace.

![Creating new codespace from button](./images/helmfun20.png?raw=true "Creating new codespace from button")

**This will run for several minutes while it gets everything ready.**
  
![Starting codespace](./images/codeium-03.png?raw=true "Starting your codespace")

This will take a while to run.

## Step 2. Install the Codeium extension

See the figure below for numbered steps. 
(1) Click on the *Extensions* icon in the activity bar.
(2) Search for *codeium* in the search field.
(3) You can click on the item in the list to open up the larger page for the extension. Then click on *Install* to install the extension.

![Install Codeium extension](./images/codeium-11.png?raw=true "Install Codeium extension")


## Step 3. Follow the dialogs to sign in/sign up for Codeium.

You may be prompted to allow sigining in. Click on the *Allow* button in the first dialog and then the *Open* button in the second dialog.

![Authorizing...](./images/codeium-04.png?raw=true "Authorizing...")
![Authorizing...](./images/codeium-05.png?raw=true "Authorizing...")

Complete the forms to sign up/sign in to use Codeium.

![Authorizing...](./images/codeium-06.png?raw=true "Authorizing...")

Provide your name if signing up.

![Authorizing...](./images/codeium-07.png?raw=true "Authorizing...")

## Step 4. Copy the authentication token that Codeium provided.

Hightlight and copy or use the copy icon to capture the authentication token on the screen.

![Copying the token...](./images/codeium-08.png?raw=true "Copying the token...")

## Step 5. Provide the token to authorize Codeium use in the Codespace.

Switch back to your codespace. Use F1 to bring up the Command Palette. (Ignore any messages about *signin failed*.) In the Command Palette, search for Codeium: Provide Authentication Token. 

![Providing the token...](./images/codeium-09.png?raw=true "Providing the token...")

After you find that, hit *Enter* and then paste in the token.

![Providing the token...](./images/codeium-10.png?raw=true "Providing the token...")

![Labs doc preview in codespace](./images/cpho4.png?raw=true "Labs doc preview in codespace")

This will open it up in a tab above your terminal. Then you can follow along with the steps in the labs. 
Any command in the gray boxes is either code intended to be run in the console or code to be updated in a file.

Labs doc: [Copilot Hands-on Labs](labs.md)


