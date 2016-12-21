# tbms
Tor-Browser Sandbox for macOS - security tool to reduce tor-browser access to macOS system

tbms is a script to allow macOS users to run TOR Browser inside Apple sandbox on Mac computers.
Sandboxing tor browser can help reduce risks related to exploits that can attack Firefox browser when browsing malicious sites.

NOTE: In no way tbms is going to secure tor browser from every possible exploit, it only helps to reduce tor browser access to your macOS resources, so it's just a marginal protection. However, sandboxing your browser does help to improve general security.

Please help me to improve this script with your suggestions and changes, thanks!

## Usage

Download torbrowser.sb on your Mac and replace all instances of <your-username> with your username on your Mac.

Download latest tor browser bundle from this link: https://www.torproject.org/download/download

Run tor using the folowing syntax from your terminal window:

sandbox-exec -f torbrowser.sb /Applications/TorBrowser.app/Contents/MacOS/firefox

You can also put the sandbox-exec command in a script to be executed via Desktop Icon.
