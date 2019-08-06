How to Get PhoneGap to Work

##basic testing

0. Update npm with "sudo npm install -g npm"
1. Update phonegap with "sudo npm install -g phonegap"
2. Try running the app locally in a browser with "sudo phonegap serve --autoreload"
3. Change some code and verify that it's updating
4. Open phonegap tester app and connect to served URL (see if it continues to work) - note that some plugins might not work on this mode

##deploying changes
1. Git should be configured with a REMOTE that PhoneGap Build knows about (phonegap build only seems to work with Github)
2. run "git add *"
3. run "git commit -m 'commit message'"
4. run "git push deploy" - where deploy is the name of the REMOTE

##running from PG BUILD
1. open build.phonegap.com
2. click "update code", which should pull from the configured repo (must be public)
3. deploy the APK to Android and test it
