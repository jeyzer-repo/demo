# Demo profile repository

The Demo profile repository is the place holder for the demo shared profiles.\
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

If you wish to execute the analysis against a constant version, set the desired <version> in the URL specified in the demo.xml of your Jeyzer installation : \
https://raw.githubusercontent.com/jeyzer-repo/demo/demo-<version\>/shared

If you wish to load the shared profiles from the online repository, set the local_first=false in your demo.xml.

As reminder, the demo.xml is located in the profiles/shared-repositories directory of your Jeyzer installation.


License
-------

Copyright 2020 Jeyzer.\
Licensed under the [Mozilla Public License, Version 2.0](https://www.mozilla.org/media/MPL/2.0/index.815ca599c9df.txt)
