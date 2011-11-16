abt, Android backup tool
========================

| Homepage:      |  https://github.com/GutenYe/abt       |
|----------------|------------------------------------------------------       |
| Author:	       | Guten                                                 |
| License:       | MIT-LICENSE                                                |
| Documentation: | http://rubydoc.info/gems/abt/frames                |
| Issue Tracker: | https://github.com/GutenYe/abt/issues |


Overview
--------

It uses rsync backend, wihch is very powerful. And it's client(Android) side app.

Features
--------

* Use Open Source Technologies: rsync
* Fast: behind rsync
* Flexible: you can configure which files need to be backup in a plan text. 

Usage
-----

Setup Configuration

	# cp /sdcard/.abrt/examples/system to /sdcard/.abrt and change the settings.

see [Configuration](http://github.com/GutenYe/abt/docs/Note.md)

Backup

	# start ssh daemon in Linux
	# adb shell with root
	$ abt backup system

Restore

	# start ssh daemon in Linux
	# adb shell with root
	$ abt restore system

Install
----------

Requiments

	* ssh and rsync in both android and linux side.
	* current need `adb shell` returns root.
	* tested in Linux

1. install rsync, ssh into android, you can get it from [android-utils](https://github.com/GutenYe/android-utils)

2. download source

3. auto install: run `$ ./install`

3. manual install: see install source code.


Contributing
-------------

* Feel free to join the project and make contributions (by submitting a pull request)
* Submit any bugs/features/ideas to issue tracker

Credits
--------

* [Contributors](https://github.com/GutenYe/abt/contributors)

Resources
---------

	* [abrtool](http://code.google.com/p/abrtool/) Simple backup and restore tool for android devices on linux based machines 

Copyright
---------

(the MIT License)

Copyright (c) 2011 Guten

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
