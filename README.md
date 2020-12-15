# fingerprinting-and-panopticlick

### what is website trackers?
a tracker is a script on websites designed to derive data points about your preferences and who you are as you interact with their site. Sometimes these scripts are placed purposefully by the website you’re on, other times a script may be from a website you’ve never visited.

### what do trackers do?
And that's pretty much what Web trackers do. They keep tabs on your Internet activity. They may know your name (if you have opened an account online), or they may not know your name but simply "know" your interests.
Reference: whatismyipaddress.com/web-tracking

### what is cookies?
An HTTP cookie (also called web cookie, Internet cookie, browser cookie, or simply cookie) is a small piece of data sent from a website and stored on the user's computer by the user's web browser while the user is browsing.

### what is panopticlick?
research project
Panopticlick is a research project that was started by the Electronic Frontier Foundation (EFF) in 2010. They use a few of the older Browser Fingerprinting techniques to gather data about your system when you hit the big orange Test Me button on the Panopticlick home page.

### What is browser fingerprinting?
Device fingerprinting or browser fingerprinting is the systematic collection of information about a remote device, for identification purposes. Client-side scripting languages allow the development of procedures to collect very rich fingerprints: browser and operating system type and version, screen resolution, architecture type, lists of fonts, plugins, microphone, camera, etc.

On this website, we collect:

the User agent header
the Accept header
the Connection header
the Encoding headerwhat is panopticlick
the Language header
the Upgrade Insecure Requests header
the Referer header
the Cache-Control header
the BuildId of the browser
the list of plugins
the platform
the cookies preferences (allowed or not)
the Do Not Track preferences (yes, no or not communicated)
the timezone
the screen resolution and its color depth
the use of local storage
the use of session storage
a picture rendered with the HTML Canvas element
a picture rendered with WebGL
Supported Audio formats
Supported Video formats
the presence of AdBlock
the list of fonts 

### How is the fingerprint collected?
Browser fingerprints are also called cookieless monsters because it is not necessary to install any form of cookie to collect a fingerprint. This means that the act of fingerprinting a specific browser is stateless and transparent for the user. Any third-party interested in fingerprinting can exploit a set of different techniques to get a rich fingerprint:

the user agent and the accept headers are automatically sent to websites when a connection is initiated.
JavaScript gives access to many browser-populated features like the plugins installed on the user’s device.
If the Flash plugin is installed, its rich programming interface (API) provides access to many system-specific attributes: exact version of the operating system, list of fonts,screen resolution, timezone.
Through the display of an HTML5 Canvas element, it is possible to collect small differences in the hardware or in the software configurations, thanks to slight differences in the image rendering between devices. The smallest pixel difference can be detected. This is called canvas fingerprinting.
On this site, we use:

Plugin Detect for plugins detection.

### How are the fingerprints exploited?
Like all tracking technology, it is a double-edge sword.

Fingerprints can be used in a constructive way to combat fraud or credential hijacking, by checking that a user who logs into a specific site is likely the legitimate user.

Fingerprints can also be used in more questionable way, in order to track users across web sites and collect information about their habits and their tastes without the users knowing about it.

Fingerprints can even be used in a destructive way: if attackers know which software modules (specific browser version, plugins, etc.) are installed on a specific device, they can deliver exploits that are tailored for these specific modules or combination of modules.

### What is the difference between AmIUnique and panopticlick ?
AmIUnique shares some goals with panopticlick, but it provides a number of novelties:

AmIUnique implements the most recent techniques for fingerprinting, including webGL and canvas
AmIUnique provides more information to the users, including global statistics, as well as a concise summary of the main characteristics of a browser
We are going to open source the new version soon, the source code for the old version is available on Github
What is the difference between AmIUnique and other similar web sites?
There exist other sites that collect and / or inform users about the amount of information that can be collected through their website:

http://fingerprint.pet-portal.eu
http://browserspy.dk
AmIUnique is different from these sites, with respect to the following points. It implements state of the art fingerprinting techniques. In particular, this is the first web site that collects information through WebGL. It provides different levels of information to the user. Beyond the complete fingerprint, AmIUnique is the only site that provides a synthetic view, which gives few, easy to understand statistics about the degree of unicity of a device among the sample we have observed so far. We also centralize a number of different pointers about fingerprinting, which go from general pages that introduce the technique, to technical papers in the research literature and press articles that cover the topic.
