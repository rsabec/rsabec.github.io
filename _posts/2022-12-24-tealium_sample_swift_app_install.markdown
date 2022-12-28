---
layout: post
title:  "Tealium Swift sample App Install"
date:   2022-12-24 08:50:00 -0800
categories: ios code tealium swift
---

 links for Tealium Swift sample app and Dependencies.
* Github [Tealium/tealium-swift](https://github.com/Tealium/tealium-swift.git) 
* [Homebrew](https://brew.sh/) - used to install Cocopods.
* [Xcode and Xcode Command Line Tools](https://developer.apple.com/download/all/) - available behind your apple develpper login -
* [Cocopods](https://formulae.brew.sh/formula/cocoapods#default)

	Sample App Setup - Swift

	1. Have Xcode and Xcode tools downloaded and ready to go.
	2. Follow the link to Homebrew and follow instructions to install on your mac.
	3. Download the Sample app from Tealium's repo, unzip and place in a uncomplicated directory path such as directly in your 'Documents' directory.
	4. Check Homebrew installed on your mac or [install it](https://brew.sh/). 
	>
	```terminal
	/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
	``` 
	5. [Install Cocopds](https://formulae.brew.sh/formula/cocoapods#default)
	>
	```terminal
	/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
	``` 
	6. Open Terminal app and change directories to location of Swift project. If you placed the download into your 'Documents' folder then  example below- 
	```terminal
    cd /Users/robert.sabec/Documents/tealium-swift-main/samples/TealiumSwiftExample
	```
	7. Test what shell you are using . ( Apple set the default shell to the Z shell (zsh). )
```terminal
echo $0
```
   8. Run Cocopods install comman in this directory .
	```terminal
	pod install
	```  

	 <br>

	

