mfp-gitignore
=============

This is an unofficial repository providing an initial/template `.gitignore`
file for an [IBM MobileFirst Platform
Foundation](http://www-03.ibm.com/software/products/en/mobilefirstfoundation)
Project. *Note*: these templates are primarily intended for use with hybrid projects,
and it is likely they may not be directly suitable for native-first projects.
There is **no** official IBM support for these artifacts. 
We are attempting to follow the same principles as GitHub's own
[gitignore project](https://github.com/github/gitignore). We will gladly
accept any pull request with corrections or clarifications (especially
explanatory comments).

Usage
-----

1. Include the contents of the appropriate `<VERSION>.gitignore` file in your `.gitignore` file, located at the root of your MFP project (*Note*: not your Eclipse workspace).
1. MFP requires some directories to be present, but Git does not check in empty directories.  [`.gitkeep`](http://stackoverflow.com/a/7229996/27641) files ensure these directories are present when developers clone the Git repository.  `.gitkeep` files should be created in the following directories:
  1. `server/java`
  1. `server/lib`
  1. `apps`
  1. `adapters/ADAPTER_NAME/lib` (for all **Java** adapters)

Older Name - Worklight
----------------------

Prior to version 6.3, IBM MobileFirst Platform Foundation was known as
[IBM Worklight
Foundation](http://www-03.ibm.com/software/products/en/worklight-foundation),
so there are equivalent `.gitignore` files here for versions 6.1 and 6.2. This
repository was formerly known as `worklight-gitignore`.
