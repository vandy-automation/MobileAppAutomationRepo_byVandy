# MobileAppAutomationRepo_byVandy
Mobile Application automation 


List of softwares needed to install app automation tool

Below is the list of all softwares needed in order to install and setup App mobile automation.
Appium Desktop
IDE- IntelliJ
Maven
Java
Android studio
Xcode
How to Install:

Steps:

Install home brew by command terminal on Mac
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

To check if home brew is installed or not - Type ‘brew’ in Terminal it will show the options

********************************JAVA Setup on Mac**********************************************

Using SDKMAN:  Type below command on terminal of Mac
1. curl -s "https://get.sdkman.io" | bash

2. Check if above command ran successfully or not:
Sdk help (open new terminal and enter this command)

3. Run command: source "$HOME/.sdkman/bin/sdkman-init.sh"

4. Check the version to be installed by entering below command on terminal:
    sdk version

    sdk list java  (check available java version)

   	    sdk install java 14.0.2-zulu  (enter the version and install through terminal)

	    Verify the Java version installed:
    Check java version: java -version

****************************************Intellij Set Up on Mac**********************************

Below is the reference link to install intelliJ
https://www.jetbrains.com/idea/download/#section=mac

Once downloaded move to applications folder under Mac

Install maven using brew: Enter below command in terminal
brew install maven

Check version installed: mvn -version

Download Appium desktop .dmg file from below link
https://github.com/appium/appium-desktop/releases/tag/v1.18.2
Move .dmg file to applications folder by dragging under Mac

*********************Download and install android studio : refer below link******************
https://developer.android.com/studio?gclid=Cj0KCQiA5vb-BRCRARIsAJBKc6JFEoVfCZ-dKDtlwZI_72VG7OyttJuJZicttEkqNOkY8-ScSbJ3F_kaAuefEALw_wcB&gclsrc=aw.ds

Drag the downloaded file to Applications folder in MAC

**********************Install and download Xcode from Apple app store*************************
Search and get install
Check Git is installed or not in command line
Enter git



**************************How to Setup ~/.bash_profile and ~/.zshrc****************************

Below is the keypoints on which we need to work
Add Java home
Add maven home
Add Npm home
	
Open Terminal enter 
whoami
Which maven
/usr/local/bin/mvn
Which java
/Users/user/.sdkman/candidates/java/current/bin/java
env | grep M2_HOME
cd /usr/local/bin/
vi ~/.bash_profile
Press shift +i
Now amend the copied path in the below Java_home and Mr_Home

#set JAVA_HOME
JAVA_HOME=/Users/user/.sdkman/candidates/java/current/bin/java
export JAVA_HOME

M2_HOME=/usr/local/bin/mvn
export M2_HOME

PATH=$PATH:$JAVA_HOME/bin:$M2_HOME/bin
export PATH

Save and close : :qw
Enter Source ~/.bash_profile

How To Set up /Export project from a Git Repo 

First check whether your have git or not 
Enter below command under terminal
Git

Now create a workspace 
Mkdir Workspace
Cd WorkSpace/
Ls   (It should be empty)
Git clone https://github.com/ashutoshsaxena06/DETestEngine.gi
Above path you have to take from someones repository
Ls (This time you should see the project name which you cloned)
For me it is DETestEngine
Cd DETestEngine/
Ls  (will show all the directories / files)
Git pull 
It will show you if you have any changes which needs to be pulled from the server repo
Otherwise it will say “Already up to date.”











