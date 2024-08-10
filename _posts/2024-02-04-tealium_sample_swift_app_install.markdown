---
layout: post
title:  "Tealium Swift sample App Install"
date:   2024-02-04 08:50:00 -0800
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
	errors ********************************
robert.sabec@TEAL-LQ62V2YRWR TealiumSwiftExample % pod install
Ignoring ffi-1.15.5 because its extensions are not built. Try: gem pristine ffi --version 1.15.5
Ignoring debug-1.4.0 because its extensions are not built. Try: gem pristine debug --version 1.4.0
Ignoring eventmachine-1.2.7 because its extensions are not built. Try: gem pristine eventmachine --version 1.2.7
Ignoring http_parser.rb-0.8.0 because its extensions are not built. Try: gem pristine http_parser.rb --version 0.8.0
Ignoring rbs-2.1.0 because its extensions are not built. Try: gem pristine rbs --version 2.1.0
Ignoring sassc-2.4.0 because its extensions are not built. Try: gem pristine sassc --version 2.4.0
Analyzing dependencies
Adding spec repo `trunk` with CDN `https://cdn.cocoapods.org/`

[!] `<PBXSourcesBuildPhase UUID=`CF2E310D237622A9000CEDD3`>` attempted to initialize an object with an unknown UUID. `CFB6B54F26792F5C00D62D87` for attribute: `files`. This can be the result of a merge and the unknown UUID is being discarded.

[!] `<PBXSourcesBuildPhase UUID=`CF2E310D237622A9000CEDD3`>` attempted to initialize an object with an unknown UUID. `CFB6B55326792F5C00D62D87` for attribute: `files`. This can be the result of a merge and the unknown UUID is being discarded.

[!] `<PBXSourcesBuildPhase UUID=`CF2E310D237622A9000CEDD3`>` attempted to initialize an object with an unknown UUID. `CFB6B55026792F5C00D62D87` for attribute: `files`. This can be the result of a merge and the unknown UUID is being discarded.

[!] `<PBXFrameworksBuildPhase UUID=`CF2E310E237622A9000CEDD3`>` attempted to initialize an object with an unknown UUID. `CF665AA02673F6EB00742E9D` for attribute: `files`. This can be the result of a merge and the unknown UUID is being discarded.
<internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require': incompatible library version - /Users/robert.sabec/.gem/ruby/3.1.2/gems/ffi-1.15.5/lib/ffi_c.bundle (LoadError)
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /Users/robert.sabec/.gem/ruby/3.1.2/gems/ffi-1.15.5/lib/ffi.rb:5:in `rescue in <top (required)>'
	from /Users/robert.sabec/.gem/ruby/3.1.2/gems/ffi-1.15.5/lib/ffi.rb:2:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/ethon-0.15.0/lib/ethon.rb:3:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/typhoeus-1.4.0/lib/typhoeus.rb:2:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:440:in `download_typhoeus_impl_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:372:in `download_and_save_with_retries_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:365:in `download_file_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:338:in `download_file'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:53:in `refresh_metadata'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source.rb:31:in `initialize'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:30:in `initialize'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:315:in `new'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:315:in `block in source_from_path'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:322:in `source_from_path'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:331:in `block in aggregate_with_repos'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:331:in `map'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:331:in `aggregate_with_repos'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:26:in `aggregate'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:60:in `all'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface/error_report.rb:173:in `repo_information'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface/error_report.rb:77:in `stack'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface/error_report.rb:24:in `report'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command.rb:66:in `report_error'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/claide-1.1.0/lib/claide/command.rb:396:in `handle_exception'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/claide-1.1.0/lib/claide/command.rb:337:in `rescue in run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/claide-1.1.0/lib/claide/command.rb:324:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command.rb:52:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/bin/pod:55:in `<top (required)>'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/bin/pod:25:in `load'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/bin/pod:25:in `<main>'
<internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require': cannot load such file -- 3.1/ffi_c (LoadError)
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /Users/robert.sabec/.gem/ruby/3.1.2/gems/ffi-1.15.5/lib/ffi.rb:3:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/ethon-0.15.0/lib/ethon.rb:3:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/typhoeus-1.4.0/lib/typhoeus.rb:2:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:440:in `download_typhoeus_impl_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:372:in `download_and_save_with_retries_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:365:in `download_file_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:338:in `download_file'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:53:in `refresh_metadata'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source.rb:31:in `initialize'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:30:in `initialize'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:315:in `new'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:315:in `block in source_from_path'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:322:in `source_from_path'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:331:in `block in aggregate_with_repos'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:331:in `map'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:331:in `aggregate_with_repos'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:26:in `aggregate'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:60:in `all'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface/error_report.rb:173:in `repo_information'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface/error_report.rb:77:in `stack'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface/error_report.rb:24:in `report'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command.rb:66:in `report_error'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/claide-1.1.0/lib/claide/command.rb:396:in `handle_exception'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/claide-1.1.0/lib/claide/command.rb:337:in `rescue in run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/claide-1.1.0/lib/claide/command.rb:324:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command.rb:52:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/bin/pod:55:in `<top (required)>'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/bin/pod:25:in `load'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/bin/pod:25:in `<main>'
<internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require': incompatible library version - /Users/robert.sabec/.gem/ruby/3.1.2/gems/ffi-1.15.5/lib/ffi_c.bundle (LoadError)
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /Users/robert.sabec/.gem/ruby/3.1.2/gems/ffi-1.15.5/lib/ffi.rb:5:in `rescue in <top (required)>'
	from /Users/robert.sabec/.gem/ruby/3.1.2/gems/ffi-1.15.5/lib/ffi.rb:2:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/ethon-0.15.0/lib/ethon.rb:3:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/typhoeus-1.4.0/lib/typhoeus.rb:2:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:440:in `download_typhoeus_impl_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:372:in `download_and_save_with_retries_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:365:in `download_file_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:338:in `download_file'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:53:in `refresh_metadata'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source.rb:31:in `initialize'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:30:in `initialize'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:315:in `new'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:315:in `block in source_from_path'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:322:in `source_from_path'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:53:in `block in sources'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:53:in `map'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:53:in `sources'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command/repo/add_cdn.rb:38:in `block in run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface.rb:64:in `section'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command/repo/add_cdn.rb:36:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/sources_manager.rb:45:in `create_source_with_url'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/sources_manager.rb:22:in `find_or_create_source_with_url'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:178:in `block in sources'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:177:in `map'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:177:in `sources'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:1077:in `block in resolve_dependencies'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface.rb:64:in `section'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:1076:in `resolve_dependencies'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:124:in `analyze'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer.rb:416:in `analyze'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer.rb:241:in `block in resolve_dependencies'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface.rb:64:in `section'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer.rb:240:in `resolve_dependencies'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer.rb:161:in `install!'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command/install.rb:52:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/claide-1.1.0/lib/claide/command.rb:334:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command.rb:52:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/bin/pod:55:in `<top (required)>'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/bin/pod:25:in `load'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/bin/pod:25:in `<main>'
<internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require': cannot load such file -- 3.1/ffi_c (LoadError)
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /Users/robert.sabec/.gem/ruby/3.1.2/gems/ffi-1.15.5/lib/ffi.rb:3:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/ethon-0.15.0/lib/ethon.rb:3:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/typhoeus-1.4.0/lib/typhoeus.rb:2:in `<top (required)>'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from <internal:/opt/homebrew/Cellar/ruby/3.1.3/lib/ruby/3.1.0/rubygems/core_ext/kernel_require.rb>:85:in `require'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:440:in `download_typhoeus_impl_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:372:in `download_and_save_with_retries_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:365:in `download_file_async'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:338:in `download_file'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:53:in `refresh_metadata'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source.rb:31:in `initialize'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/cdn_source.rb:30:in `initialize'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:315:in `new'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:315:in `block in source_from_path'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:322:in `source_from_path'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:53:in `block in sources'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:53:in `map'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-core-1.11.3/lib/cocoapods-core/source/manager.rb:53:in `sources'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command/repo/add_cdn.rb:38:in `block in run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface.rb:64:in `section'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command/repo/add_cdn.rb:36:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/sources_manager.rb:45:in `create_source_with_url'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/sources_manager.rb:22:in `find_or_create_source_with_url'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:178:in `block in sources'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:177:in `map'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:177:in `sources'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:1077:in `block in resolve_dependencies'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface.rb:64:in `section'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:1076:in `resolve_dependencies'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer/analyzer.rb:124:in `analyze'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer.rb:416:in `analyze'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer.rb:241:in `block in resolve_dependencies'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/user_interface.rb:64:in `section'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer.rb:240:in `resolve_dependencies'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/installer.rb:161:in `install!'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command/install.rb:52:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/claide-1.1.0/lib/claide/command.rb:334:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/lib/cocoapods/command.rb:52:in `run'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/gems/cocoapods-1.11.3/bin/pod:55:in `<top (required)>'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/bin/pod:25:in `load'
	from /opt/homebrew/Cellar/cocoapods/1.11.3/libexec/bin/pod:25:in `<main>'
	 <br>

	

