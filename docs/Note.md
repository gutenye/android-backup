Profile Configuration
---------------------

for example, a 'guten' profile

	/sdcard/.abrt/
		conf       # global settings 
		guten/
			conf     # profile settings
			files    # used in `rsync --files-from=files`
			excludes # optional.  used in `rsync --exclude-from=excludes`

also see SOURCE/conf/examples

Android File System Layout
--------------------------

	/system/app  # system apps, come with device
	/data/app    # user apps, install from market by user
	/data/data   # system + user settings

more details in /data/data

	/data/data
		com.android.providers.telephony/databases/mmssms.db  # SMS messages
		com.android.browser/databases/browser.db  # Bookmarks
		com.android.alarmclock
		com.google.android.providers.settings
		com.android.launcher
		com.android.providers.userdictionary
