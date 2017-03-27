# soot-docs
Javadoc from the nightly build of soot we use in jaam, as their server is down

# Building
First, clone the Soot git repository (https://github.com/Sable/soot.git). The directory where this git repository resides will be known as `<soot-dir>`. Next, check out the appropriate commit for the jar file. At the time of this writing, we're using a nightly build jar from 2016-10-21, so I found the last commit on or before that date (8912246ea434f9052e009ab5b7d30cd2c16a37f9).

Next, run the following line (in the directory of this repository, if updating):

`javadoc -classpath <soot-dir>/src -linksource -subpackages soot`
