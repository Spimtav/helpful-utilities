# helpful-utilities
It is hereby decreed: 

This repo shall house a set of scripts and such that i've written to solve (generally) one-off problems.  May they serve you as well as they have me, weary traveller.

### on-the-fly
In my work on VMware's Tanzu, there came a time in which i had to constantly switch between maintaining two projects: one very new and one very old.  Each of them were running vastly different Concourse versions, which necessitated switching back and forth between two versions of the fly-cli every few minutes.

This got old real fast.

This script uses the magic of symlinks to quickly toggle between fly-cli versions, so that you don't have to redownload and install things a bunch of times.

Dependencies:
- old fly, named fly_<old_major>
- new fly, named fly_<new_major>
- FLY_DIRECTORY set in the script to some bin directory on your PATH

