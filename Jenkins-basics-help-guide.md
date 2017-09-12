# Jenkins Guide Mac

## Getting Started
These instructions will help you install Jenkins on your Mac.


## Install Jenkins
- [Click here to download latest version of Jenkins.](https://jenkins.io/download/)
- Click pkg to install Jenkins
- By Default Jenkins should be running on port 8080
- Access link - [http://localhost:8080]

## Change Jenkins Port

```bash
# Set Port

$ sudo defaults write /Library/Preferences/org.jenkins-ci httpsPort <any port number>


# Read Port

sudo defaults read /Library/Preferences/org.jenkins-ci httpsPort
```

```bash
# Usage

sudo defaults write /Library/Preferences/org.jenkins-ci httpsPort 8443
```

## Start Jenkins

```bash
$ sudo launchctl load /Library/LaunchDaemons/org.jenkins-ci.plist
```
## Stop Jenkins

```bash
$ sudo launchctl load /Library/LaunchDaemons/org.jenkins-ci.plist
```

## Start Jenkins using war file
- Open terminal and locate **jenkins.war** file.
```bash
# Run Jenkins war on any port 

java -jar jenkins.war --httpPort=8080
```
- Follow [Documentation](https://jenkins.io/doc/)

## License

Copyright © 2017 Sato Global Solutions, LLC. All rights reserved.
