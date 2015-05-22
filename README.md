# appium

Run: 
docker run -i -p 4723:4723 danielviorreta/appium:latest

Stop docker:
docker ps
docker stop CONTAINER_ID

Connect via ssh:
$(boot2docker shellinit 2> /dev/null)
docker run -i -t danielviorreta/appium:latest /bin/bash

Start appium:
/home/automator/appium/node_modules/.bin/appium

Appium needs one device to be ready and listening:
/home/automator/android-sdk-linux/platform-tools/adb-devices

Start emulator via command line:
/home/automator/android-sdk-linux/tools/platform-tools/emulator -avd ANDROID

Add tools, platform-tools and build tools to path:
export PATH=$PATH:$ANDROID_HOME/tools
export PATH=$PATH:$ANDROID_HOME/platform-tools/
export PATH=$PATH:$ANDROID_HOME/build-tools/19.1.0


