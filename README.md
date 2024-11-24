# OpenPNGStudio-Factory
Automated binary builds and releases of OpenPNGStudio

## Current Platforms
- Linux
- Windows
- FreeBSD
- OpenBSD
> Note 1: *BSD have binary builds for their latest release version<br>
> Note 2: I couldn't get NetBSD to install deps, I have no idea why but pkg_add wasn't shoving any signs of life - it was stuck

What about Macos? No, I am NOT going to spend money to buy Mac just to test build it on there, other BSDs didn't require any patches so I'm sure you can
just as easily build it yourself. MacOS uses stuff from FreeBSD so you can be in luck. However MacOS has their own ABI so you won't run FreeBSD biniares :p

### *BSD and ports
Since it's possible by each *BSD release some things may change in their ABI, you'll have to manually build it using ports tree.<br>
> Thanks again [Bryan Steele](https://brynet.ca/) for the [heads up](https://bsky.app/profile/canadianbryan.bsky.social/post/3lbnukw7uvk2i)! Go and help him out by buying him a pizza! https://brynet.ca/wallofpizza.html<br>

You're in luck, OpenPNGStudio will contain a directory `ports` (unless I think of something else) with `README.txt` file with instructions how to
1. install the port into ports tree
2. build OpenPNGStudio within ports tree
3. install it from ports tree
