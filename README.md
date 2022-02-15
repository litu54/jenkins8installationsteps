# jenkins8installationsteps

Installing Jenkins on Ubuntu

On Debian-based distributions, such as Ubuntu, you can install Jenkins through apt-get.

You need to have a JDK and JRE installed. openjdk-8-jre and openjdk-8-jdk are suggested.

Command to be executed:
sudo apt-get update -y && sudo apt-get install openjdk-8-jdk openjdk-8-jre -y

Once Java is installed set the JAVA_HOME path.
Command to be executed:
export JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
export PATH=$PATH:$JAVA_HOME/bin

Add the above two lines at the end of /etc/environment 
source /etc/environment

Usually most linux systems source /etc/environment by default. If your system doesn't do that add the following line to ~/.bashrc 

Follow the remaining instructions available at the official site:
https://wiki.jenkins.io/display/JENKI...
