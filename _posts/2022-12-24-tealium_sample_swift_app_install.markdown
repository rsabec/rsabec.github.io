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
    cd Documents/mobile/ios/tealium-swift-master/samples/TealiumSwiftExample
	```
	7. Test what shell you are using . ( Apple set the default shell to the Z shell (zsh). )
```terminal
echo $0
```
	8. Run Cocopods install comman in this directory .
	```terminal
	pod install
	```  
pod install - returns below errors.<br>
Ignoring ffi-1.15.5 because its extensions are not built. Try: gem pristine ffi --version 1.15.5 <br>
Ignoring debug-1.4.0 because its extensions are not built. Try: gem pristine debug --version 1.4.0 <br>
Ignoring eventmachine-1.2.7 because its extensions are not built. Try: gem pristine eventmachine --version 1.2.7 <br>
Ignoring http_parser.rb-0.8.0 because its extensions are not built. Try: gem pristine http_parser.rb --version 0.8.0 <br>
Ignoring rbs-2.1.0 because its extensions are not built. Try: gem pristine rbs --version 2.1.0 <br>
Ignoring sassc-2.4.0 because its extensions are not built. Try: gem pristine sassc --version 2.4.0 <br>
Analyzing dependencies <br>
[!] Could not automatically select an Xcode project. Specify one in your Podfile like so: <br>
    project 'path/to/Project.xcodeproj'
	 <br>

	

