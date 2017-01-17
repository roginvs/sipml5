# This is sipml5 library with some patches applied
- ICE Gathering timeout hack: This solves a problem when calls can delay up to 10 seconds. It happens when some of stun requests are dropped, for example if they are sent from interface without internet and etc. The patch reduced timeout from 10 seconds to 2.
- Failed to set local answer sdp: In some cases sipml5 can cause this error in Chrome. Workaround is taken from https://code.google.com/archive/p/sipml5/issues/209 with a simple change to make hold/resume working again.
- Fix for CallerId Name problems from https://github.com/DoubangoTelecom/sipml5/issues/163
- Indication for "Call completed elsewhere". Just simple lookup for such reason. This is useful in order to not to show such calls as missed

# Online test
Online demo is available [here](http://roginvs.github.io/sipml5/call.htm)

# Download
Download JS API: [SIPml-api.js](https://raw.githubusercontent.com/roginvs/sipml5/master/release/SIPml-api.js)
