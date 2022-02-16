# Demo profile repository

The Demo profile repository is the place holder for the demo master and shared profiles.\
These profiles are compatible with the current Jeyzer project version.


Storage
---------------------------
The Jeyzer demo repository is a git repository maintained at :\
https://github.com/jeyzer-repo/demo


Shared profile access
---------------------------
The Jeyzer Analyzer is always accessing the **local** version first of the shared profiles in the demo repository, before accessing the remote one (the current one) at :\
https://raw.githubusercontent.com/jeyzer-repo/demo/master/shared \
Note that the "master" in this URL is the git branch (not to be confused with a Jeyzer "master" profile).

If you wish to execute the analysis against a constant version, set the desired \<version\> in the URL specified in the demo-repository.xml of your Jeyzer installation : \
https://raw.githubusercontent.com/jeyzer-repo/demo/demo-<version\>/shared

If you wish to load the shared profiles from the online repository, set the local_first=false in your demo-repository.xml.

As reminder, the demo-repository.xml is located in the profiles/shared-repositories directory of your Jeyzer installation.


Master profile access
---------------------------
The demo master profiles are loaded by the Jeyzer Web Analyzer.

If you wish to remove the demo master profiles from the Jeyzer Web Analyzer, remove the JEYZER_DEMO_MASTER_PROFILES_DIR reference from the JEYZER_MASTER_PROFILES_DIR_ROOTS environment variable.\
The JEYZER_MASTER_PROFILES_DIR_ROOTS variable is by default set in the web/apache-tomcat-9.0.41/bin/setenv.bat|sh file of your Jeyzer installation.


License
-------

Copyright 2022 Jeyzer.\
Licensed under the [Mozilla Public License, Version 2.0](https://www.mozilla.org/media/MPL/2.0/index.815ca599c9df.txt)
