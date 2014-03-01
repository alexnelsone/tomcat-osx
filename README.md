Installing Apache Tomact on OS X:


1. Download the tar.gz from the apache site.
2. Extract it to /usr/local/
3. (suggestion) create a link /usr/local/tomcat that points to the extracted files.
4. tomcat-launchd.sh should be put into /usr/local/apache-tomcat-<VERSION>/ and have executable bit s
5. org.apache.tomcat.plist should be put into /Library/LaunchDaemons and owned by root:wheel
6. load the script into launchd with 'sudo launchctl load /Libary/LaunchDaemons/org.apache.tomcat.plist
7. verify that launchd has the script locate with 'sudo launchctl list | grep tomcat'