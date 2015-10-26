A very basic [Ionic](http://ionicframework.com) project with a (non-working) Android implementation of [Parse](https://parse.com/docs/android/guide#push-notifications)'s Push service and [Phonegap's Push plugin](https://github.com/phonegap/phonegap-plugin-push)

Steps taken to create this projects:
- create an ionic project `ionic start myApp`
- ran 'npm install && bower install' to install all the dependencies
- added [Phonegap's Push plugin](https://github.com/phonegap/phonegap-plugin-push) 'ionic plugin add https://github.com/phonegap/phonegap-plugin-push'
- added the Android platform `ionic platform add android`
- implemented the Push plugin as illustrated in the [readme](https://github.com/phonegap/phonegap-plugin-push#quick-example)
- build and ran it on an android device 'ionic run android'
- debugged the webapp using [Chrome's remote debugging](https://developer.chrome.com/devtools/docs/remote-debugging)

The problem is that the device somehow can't register with GCM as it keeps returning an empty registrationId. I also tried replacing Parse's GCM Push Credentials with credentials I made in the Google Developers Console, but to no avail... 
