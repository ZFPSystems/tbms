# tbms
Tor-Browser Sandbox for macOS - security tool to reduce tor-browser access to macOS system

tbms is a script to allow macOS users to run TOR Browser inside Apple sandbox on Mac computers.
Sandboxing tor browser can help reduce risks related to exploits that can attack Firefox browser when browsing malicious sites.

NOTE (1): In no way tbms is going to secure tor browser from every possible exploit, it only helps to reduce tor browser access to your macOS resources, so it's just a marginal protection. However, sandboxing your browser does help to improve general security.

NOTE (2): New BROWSER release can break things up, if I find something not working I'll fix it, however if you find something not working after a browser update please try to fix and send me a pull I'll be happy to review your changes and add them to the master branch!

Please help me to improve this script with your suggestions and changes, thanks!

## Usage

1) Download torbrowser.sb on your Mac and replace all instances of < your-username > in torbrowser.sb with your username on your Mac, for example:

   Replace < your-username > with john

   Please Note: if the operation above results too difficult for you then it means you need to learn how to use your Mac and a text editor more before attempting to use projects like tbms.

2) Download latest tor browser bundle from this link: https://www.torproject.org/download/download

3) Run tor using the folowing syntax from your terminal window:

   sandbox-exec -f torbrowser.sb /Applications/TorBrowser.app/Contents/MacOS/firefox

   You can also put the sandbox-exec command in a script to be executed via Desktop Icon.

## More info

Please Note that each new release of the TOR Browser bundle may try to use different directory patch or resources and so you may get error messages that will require you to modify the torbrowser.sb script in order to address the specific issue.

In some cases it may be required also to change some configuration parameter on the browser itself. To access Browser configuration type about:config in the URL field and search for the specific parameter that is causing problems when the browser is executed inside a sandbox.

For more info check my original post on my blog here: https://paolozaino.wordpress.com/2015/10/20/maximum-security-and-privacy-using-mac-os-sandbox-and-tor-browser-bundle/

