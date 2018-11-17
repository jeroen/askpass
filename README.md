# askpass

> Safe Password Entry for R, Git, and SSH

[![Build Status](https://travis-ci.org/jeroen/askpass.svg?branch=master)](https://travis-ci.org/jeroen/askpass)
[![AppVeyor Build Status](https://ci.appveyor.com/api/projects/status/github/jeroen/askpass?branch=master&svg=true)](https://ci.appveyor.com/project/jeroen/askpass)


Utilities for prompting the user for credentials or a passphrase, for
example to authenticate with a server or read a private key. Includes reliable
native programs for MacOS and Windows, no widgets are required. Password entry 
can be invoked in two different ways: either directly from R via the askpass()
function, but also indirectly as password-entry back-end via the SSH_ASKPASS 
and GIT_ASPKASS environment variables. Thereby the user can be prompted for 
credentials or a passphrase when R calls out to git or ssh-agent.

## Example

To invoke the password prompt manually use:

```r
askpass::askpass()
```

### Windows Credential Prompt

![askpass-rs](img/askpass-win.png)

### RStudio Desktop


![askpass-rs](img/askpass-rs.png)


