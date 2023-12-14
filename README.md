![GitHub Repo stars](https://img.shields.io/github/stars/djacidfx/djacidfx.github.io)
![Website](https://img.shields.io/website?url=https%3A%2F%2Fwildcatproductions.biz%2F&up_message=Online&up_color=blue&down_message=Offline&down_color=red)
![GitHub Discussions](https://img.shields.io/github/discussions/djacidfx/Rust-Server-Installer)
<span class="badge-githubsponsors"><a href="https://github.com/sponsors/djacidfx" title="Donate to this project using GitHub Sponsors"><img src="https://img.shields.io/badge/github-donate-yellow.svg" alt="GitHub Sponsors donate button" /></a></span>
<span class="badge-buymeacoffee"><a href="https://buymeacoffee.com/wildcatprod" title="Donate to this project using Buy Me A Coffee"><img src="https://img.shields.io/badge/buy%20me%20a%20coffee-donate-yellow.svg" alt="Buy Me A Coffee donate button" /></a></span>
<span class="badge-patreon"><a href="https://patreon.com/wildcatstudio" title="Donate to this project using Patreon"><img src="https://img.shields.io/badge/patreon-donate-yellow.svg" alt="Patreon donate button" /></a></span>
<span class="badge-paypal"><a href="https://paypal.me/WildCatProductions" title="Donate to this project using Paypal"><img src="https://img.shields.io/badge/paypal-donate-yellow.svg" alt="PayPal donate button" /></a></span>

![GitHub repo size](https://img.shields.io/github/repo-size/djacidfx/Rust-Server-Installer)
![GitHub release (with filter)](https://img.shields.io/github/v/release/djacidfx/Rust-Server-Installer)
[![Awesome Content - Click Here](https://img.shields.io/badge/Awesome_Content-Click_Here-2ea44f)](https://mywild.work/)
[![Awesome](https://awesome.re/badge.svg)](https://mywild.work/)

## Issues
If you find a bug or run into any issues please submit them on our [Issue Tracker](https://github.com/djacidfx/Rust-Server-Installer/issues)

Rust is a multiplayer-only survival sandbox game developed by Facepunch Studios. It was released in early access in 2013 and fully released in 2018. In Rust, players must gather resources, build structures, and craft weapons and tools in order to survive in a harsh and unforgiving world. Rust is known for its challenging gameplay, its emphasis on PvP combat, and its unique world-building system.

![Rust Server](https://mywild.work/uploads/images/202310/image_750x_652c5126de5ab.jpg)

[Click Here to view full blog post](https://mywild.work/rust-server-installing-a-rust-server-the-easy-way)

<h2 data-sourcepos="5:1-5:65">How to Build Your Own Local Rust Server Easy</h2>
<div class="sqs-block html-block sqs-block-html" data-block-type="2" id="block-yui_3_17_2_3_1427555213965_11319">
<div class="sqs-block-content">
<div class="sqs-html-content">
<h2 style="white-space: pre-wrap;">System Requirements</h2>
<p class="" style="white-space: pre-wrap;">The Rust server can be taxing on your host/local machine but maybe not as much as you might think. As a baseline a 3 square km (default gen size) map freshly generated will run at close to 2 gigabytes of ram. After some stress testing and 150k entities later, can use 6+ gigabytes of memory easily. So I would suggest having at least 8 gigs allocated per server so you don't encounter as much lag during peek times.</p>
</div>
</div>
</div>
<h2 data-sourcepos="52:1-52:183">100% Automated Install and Setup:</h2>
<p>Using the attached batch script at the bottom of this post (".bat" file - windows only) you can automate the entire install process including the option to install oxide or Carbon, setup owner/Moderator ID's and create batch scripts to start, update and wipe your server or if you want to review the code and see what's all in it, you can <a href="https://github.com/djacidfx/Rust-Server-Installer/blob/main/Setup.bat" title="batch script" target="_blank" rel="noopener">click here</a> and also download the batch script from there.</p>
<p></p>
<p data-sourcepos="7:1-7:88"><strong>To build a Rust server the manual way, you will need the following:</strong></p>
<ul data-sourcepos="9:1-12:0">
<li data-sourcepos="9:1-9:20">A copy of SteamCMD</li>
<li data-sourcepos="10:1-10:43">A copy of the Rust Server installed (using SteamCMD)</li>
<li data-sourcepos="11:1-12:0">A batch file (text) editor to make and edit your batch script</li>
</ul>
<p data-sourcepos="13:1-13:66">Once you have all of the necessary components, follow these steps:</p>
<ul data-sourcepos="15:1-21:0">
<li>
<p class="" style="white-space: pre-wrap;">Create a folder for SteamCMD, such as c:\steamcmd</p>
</li>
<li>
<p class="" style="white-space: pre-wrap;">Create a folder for the server, such as c:\rustserver</p>
</li>
<li>
<p class="" style="white-space: pre-wrap;"><a href="https://steamcdn-a.akamaihd.net/client/installer/steamcmd.zip" target="_blank" rel="noopener">Download </a>SteamCMD for Windows.</p>
</li>
<li>
<p class="" style="white-space: pre-wrap;">Extract the contents of the zip file to the folder you created for steamcmd.</p>
</li>
<li>
<p class="" style="white-space: pre-wrap;">Execute the steamcmd.exe program for the first time so it can install updates. (Your computer may ask you to confirm that you want to run it.) Once updated, type Exit and press enter.</p>
</li>
<li>Open a Terminal window and change directory (cd C:/SteamCMD) into where you installed SteamCMD and run the following command:</li>
</ul>
<div _ngcontent-ng-c285113196="" class="code-block ng-star-inserted">
<div _ngcontent-ng-c285113196="" class="code-block-decoration header gmat-subhead-2 ng-star-inserted"><span _ngcontent-ng-c285113196=""><span style="color: rgb(35, 111, 161);">DOS Command Line to install the Rust Server</span><br></span></div>
<pre _ngcontent-ng-c285113196=""><code _ngcontent-ng-c285113196="" role="text" class="code-container"><span class="hljs-function"><span class="hljs-title">steamcmd.exe</span> +<span class="hljs-title">login</span> <span class="hljs-title">anonymous</span> +<span class="hljs-title">force_install_dir</span> <span class="hljs-title">C</span>:\<span class="hljs-title">rustserver</span> +<span class="hljs-title">app_update</span> 258550 +<span class="hljs-title">quit</span>
</span></code></pre>
</div>
<p><span class="citation-5 contradictory citation-end-5" role="button" tabindex="0"><strong>You should see something like this (SteamCMD being updated):</strong></span></p>
<p><img src="https://mywild.work/uploads/images/202310/image_750x_653c21c2b8035.jpg" alt=""></p>
<p></p>
<div class="sqs-block html-block sqs-block-html" data-block-type="2" id="block-yui_3_17_2_4_1485807572147_60324">
<div class="sqs-block-content">
<div class="sqs-html-content">
<h2 style="white-space: pre-wrap;">Changing to a different branch</h2>
<p class="" style="white-space: pre-wrap;">If you want to download the staging branch of Rust that receives the most recent updates, modify the app_update command as follows: </p>
<pre><code>app_update 258550 -beta staging</code></pre>
<p class="" style="white-space: pre-wrap;">If you want to download the prerelease branch of Rust that receives the future/work-in-progress updates, modify the app_update command as follows: </p>
<pre><code>app_update 258550 -beta prerelease</code></pre>
</div>
</div>
</div>
<h2 data-sourcepos="38:1-38:15">Post Install and Configure</h2>
<p><strong>Installing Oxide:</strong></p>
<div _ngcontent-ng-c1415017246="" class="markdown markdown-main-panel" style="--animation-duration: 600ms;" dir="ltr">
<p data-sourcepos="1:1-1:52">you will need to:</p>
<ol data-sourcepos="3:1-8:0">
<li data-sourcepos="3:1-3:62"><span class="citation-0 entailed citation-end-0" role="button" tabindex="0">Download the latest version of <a href="https://umod.org/games/rust" title="Oxide" target="_blank" rel="noopener">Oxide for Rust</a>.</span></li>
<li data-sourcepos="4:1-4:38"><span class="citation-1 entailed citation-end-1" role="button" tabindex="0">Stop your Rust server.</span></li>
<li data-sourcepos="5:1-5:69">Extract the Oxide files to the root directory of your Rust server.</li>
<li data-sourcepos="6:1-6:55">Replace any existing files with the new Oxide files.</li>
<li data-sourcepos="7:1-8:0">Start your Rust server.</li>
</ol>
<p data-sourcepos="9:1-9:155">To verify that Oxide is installed correctly, open the Rust console and type <code>oxide.version</code>. You should see the version number of Oxide that you installed.</p>
<p data-sourcepos="11:1-11:178"><strong>Note:</strong> If you are using a Rust server hosting provider, they may have a different process for installing Oxide. Please consult with your hosting provider for more information.</p>
<p data-sourcepos="13:1-13:51">Here are some additional tips for installing Oxide:</p>
<ul data-sourcepos="15:1-18:0">
<li data-sourcepos="15:1-15:98"><span class="citation-2 contradictory citation-end-2" role="button" tabindex="0">Make sure that you download the correct version of Oxide for your operating system.</span></li>
<li data-sourcepos="16:1-16:112">If you are using a Linux server, you may need to install the Mono runtime environment before installing Oxide.</li>
<li data-sourcepos="17:1-18:0">If you are updating Oxide, make sure to back up your Rust server files before you begin.</li>
</ul>
<p data-sourcepos="19:1-19:236">Once Oxide is installed, you can start installing plugins. <span class="citation-3 entailed citation-end-3" role="button" tabindex="0">Plugins are extensions that add new features and functionality to your Rust server.</span> You can find plugins on the Oxide website or through other third-party websites.</p>
<p data-sourcepos="21:1-21:188">To install a plugin, simply download the plugin file and place it in the <code>/rust/oxide/plugins/</code> directory. Once a plugin is configured, restart your Rust server so the changes can take effect. The plugin will be loaded when the server starts.</p>
<p data-sourcepos="23:1-23:177"><span class="citation-4 entailed citation-end-4" role="button" tabindex="0">Once a plugin is installed, you can tweak the configure file by editing the plugin's configuration file.</span> Configuration files are located in the <code>/rust/oxide/config/</code> directory as of this posting.</p>
<p data-sourcepos="25:1-25:103">For more information on installing and using Oxide and plugins, please consult the Oxide documentation.<span class="citation-6 entailed citation-end-6" role="button" tabindex="0"></span></p>
</div>
<p data-sourcepos="40:1-40:213"><span class="citation-6 entailed citation-end-6" role="button" tabindex="0">Once the Rust server is running, you may want to install some mods or plugins.</span> To do this, you will need to download the mod or plugin files and place them in the <code>C:\rustserver\oxide\plugins</code> folder.</p>
<p data-sourcepos="13:1-13:53">Here are some additional tips for installing plugins:</p>
<ul data-sourcepos="15:1-19:0">
<li data-sourcepos="15:1-15:60">Make sure that you download plugins from a trusted source.</li>
<li data-sourcepos="16:1-16:90">Make sure that the plugins are compatible with the version of Rust that you are running.</li>
<li data-sourcepos="17:1-17:113">Be careful when installing plugins, as some plugins may conflict with each other or cause your server to crash.</li>
<li data-sourcepos="18:1-19:0">It is a good idea to back up your Rust server files before installing any new plugins.</li>
</ul>
<p data-sourcepos="20:1-20:138">Once you have installed your desired plugins, you can start enjoying the new features and functionality that they add to your Rust server.</p>
<div _ngcontent-ng-c1102191209="" role="dialog" aria-live="polite" aria-atomic="true" cdktrapfocus="" class="container"></div>
<div _ngcontent-ng-c1102191209="" role="dialog" aria-live="polite" aria-atomic="true" cdktrapfocus="" class="container"></div>
<div _ngcontent-ng-c1102191209="" role="dialog" aria-live="polite" aria-atomic="true" cdktrapfocus="" class="container"></div>
<div _ngcontent-ng-c1102191209="" role="dialog" aria-live="polite" aria-atomic="true" cdktrapfocus="" class="container"></div>
<div _ngcontent-ng-c1102191209="" role="dialog" aria-live="polite" aria-atomic="true" cdktrapfocus="" class="container"></div>
<div _ngcontent-ng-c1102191209="" role="dialog" aria-live="polite" aria-atomic="true" cdktrapfocus="" class="container"></div>
<div _ngcontent-ng-c1102191209="" role="dialog" aria-live="polite" aria-atomic="true" cdktrapfocus="" class="container"></div>
<div _ngcontent-ng-c1102191209="" role="dialog" aria-live="polite" aria-atomic="true" cdktrapfocus="" class="container"></div>
<div _ngcontent-ng-c1862129701="" class="response-container-content ng-tns-c1862129701-202">
<div _ngcontent-ng-c2554690515="" class="response-content ng-trigger ng-trigger-responsePopulation ng-tns-c1862129701-202">
<div _ngcontent-ng-c1415017246="" class="markdown markdown-main-panel" style="--animation-duration: 600ms;" dir="ltr">
<p data-sourcepos="1:1-1:63"><strong>To install Carbon on a Rust server, you can follow these steps:</strong></p>
<ol data-sourcepos="3:1-8:0">
<li data-sourcepos="3:1-3:74">Download the latest version of Carbon for Rust from the <a href="https://github.com/CarbonCommunity/Carbon/releases" title="install carbon" target="_blank" rel="noopener">Carbon website</a>.</li>
<li data-sourcepos="4:1-4:38"><span class="citation-0 entailed citation-end-0" role="button" tabindex="0">Stop your Rust server.</span></li>
<li data-sourcepos="5:1-5:83"><span class="citation-1 entailed citation-end-1" role="button" tabindex="0">Extract the Carbon files to the root directory of your Rust server.</span></li>
<li data-sourcepos="6:1-6:69"><span class="citation-2 contradictory citation-end-2" role="button" tabindex="0">Replace any existing files with the new Carbon files.</span></li>
<li data-sourcepos="7:1-8:0">Start your Rust server.</li>
</ol>
<p data-sourcepos="9:1-9:153">To verify that Carbon is installed correctly, open the Rust console and type <code>c.version</code>. You should see the version number of Carbon that you installed.</p>
<p data-sourcepos="11:1-11:192"><strong>Note:</strong> <span class="citation-3 contradictory citation-end-3" role="button" tabindex="0">If you are using a Rust server hosting provider, they may have a different process for installing Carbon.</span> Please consult with your hosting provider for more information.</p>
<p data-sourcepos="13:1-13:52">Here are some additional tips for installing Carbon:</p>
<ul data-sourcepos="15:1-18:0">
<li data-sourcepos="15:1-15:86">Make sure that you download the correct version of Carbon for your operating system.</li>
<li data-sourcepos="16:1-16:113">If you are using a Linux server, you may need to install the Mono runtime environment before installing Carbon.</li>
<li data-sourcepos="17:1-18:0">If you are updating Carbon, make sure to back up your Rust server files before you begin.</li>
</ul>
<p data-sourcepos="19:1-19:238">Once Carbon is installed, you can start installing plugins. <span class="citation-4 entailed citation-end-4" role="button" tabindex="0">Plugins are extensions that add new features and functionality to your Rust server.</span> You can find plugins on the Carbon website or through other third-party websites.</p>
<p data-sourcepos="21:1-21:202">To install a plugin, simply download the plugin file and place it in the <code>/rust/carbon/plugins/</code> directory. <span class="citation-5 contradictory citation-end-5" role="button" tabindex="0">Then, restart your Rust server.</span> The plugin will be loaded when the server starts.</p>
<p data-sourcepos="23:1-23:165">Once a plugin is installed, you can configure it by editing the plugin's configuration file. Configuration files are located in the <code>/rust/carbon/config/</code> directory.</p>
<p data-sourcepos="25:1-25:105">For more information on installing and using Carbon and plugins, please consult the Carbon documentation.</p>
<p data-sourcepos="27:1-27:70">Here are some additional benefits of using Carbon on your Rust server:</p>
<ul data-sourcepos="29:1-36:0">
<li data-sourcepos="29:1-29:78"><span class="citation-6 entailed citation-end-6" role="button" tabindex="0">Carbon is a lightweight and high-performance modding framework.</span></li>
<li data-sourcepos="30:1-30:133"><span class="citation-7 entailed citation-end-7" role="button" tabindex="0">Carbon is backwards compatible with Oxide plugins, so you can continue to use your favorite Oxide plugins with Carbon.</span></li>
<li data-sourcepos="31:1-31:118"><span class="citation-8 entailed citation-end-8" role="button" tabindex="0">Carbon has a built-in stack and gather manager, which makes it easy to manage resources on your server.</span></li>
<li data-sourcepos="32:1-32:103">Carbon has a permissions system that allows you to give players different permissions on your server.</li>
<li data-sourcepos="33:1-33:84">Carbon has a hook system that allows you to customize the behavior of your server.</li>
<li data-sourcepos="34:1-34:117">Carbon has chat and console support, so you can interact with your players and manage your server from the console.</li>
<li data-sourcepos="35:1-36:0"><span class="citation-9 entailed citation-end-9" role="button" tabindex="0">Carbon has an embedded demystifier, which makes it easy to debug plugins and troubleshoot problems.</span></li>
</ul>
</div>
<message-content _ngcontent-ng-c2554690515="" class="model-response-text ng-tns-c2554690515-201 ng-star-inserted" _nghost-ng-c1415017246="" style="height: auto;" id="message-content-idr_6cf093c96a90c33d"></message-content></div>
<div _ngcontent-ng-c2554690515="" class="response-content ng-trigger ng-trigger-responsePopulation ng-tns-c1862129701-202">You can find more information about Carbon, how to install, install, setup and commands you can <a href="https://github.com/CarbonCommunity/Carbon" title="github" target="_blank" rel="noopener"> click here</a> to visit their GitHub</div>
</div>
<p data-sourcepos="42:1-42:295"><strong>Other information:</strong></p>
<p data-sourcepos="42:1-42:295">You can start the Rust server with specific configuration options. To do this, add the desired configuration options to the <code>RustDedicated.exe</code> command line in the batch file. For example, to start the server with a different port number, you would add the following line to the batch file:</p>
<div _ngcontent-ng-c285113196="" class="code-block ng-star-inserted">
<div _ngcontent-ng-c285113196="" class="code-block-decoration header gmat-subhead-2 ng-star-inserted"><span _ngcontent-ng-c285113196="">DOS Commandline<br></span></div>
<pre _ngcontent-ng-c285113196=""><code _ngcontent-ng-c285113196="" role="text" class="code-container">RustDedicated.exe -batchmode +server.port <span class="hljs-number">28017</span>
</code></pre>
</div>
<p data-sourcepos="48:1-48:88">You can find a list of all available configuration options on the official Rust website but the most common batch file looks something like:</p>
<pre class="language-csharp"><code> @echo off
:start 
C:\steamcmd\steamcmd.exe +login anonymous +force_install_dir c:\rustserver\ +app_update 258550 +quit

RustDedicated.exe -batchmode +server.port 28015 +server.level "Procedural Map" +server.seed 1234 +server.worldsize 4000 +server.maxplayers 10  +server.hostname "Name of Server as Shown on the Client Server List" +server.description "Description shown on server connection window." +server.url "http://yourwebsite.com" +server.headerimage "http://yourwebsite.com/serverimage.jpg" +server.identity "server1" +rcon.port 28016 +rcon.password letmein +rcon.web 1

goto start</code></pre>
<h2 style="white-space: pre-wrap;">Connecting to your server</h2>
<p class="" style="white-space: pre-wrap;">Run the Rust Client, and do not select a server. Note that your server will not show up under the “Local Network” tab. Instead, press F1 and go to the client console. Assuming you used the default port of <strong>28015</strong>, type in the following command to connect to your server:</p>
<pre><code>client.connect localhost:28015</code></pre>
<h2 style="white-space: pre-wrap;">Adding Owners and Moderators</h2>
<p class="" style="white-space: pre-wrap;">Once the server is up and running you may choose to assign ownership to yourself. This is done with the <strong>ownerid</strong> command. You will need your 17 digit SteamID number, <a href="https://www.steamidfinder.com/" title="steam id" target="_blank" rel="noopener">click here</a> to find it. The easiest way to get it, is to log in and then run the <strong>users</strong> command at the console. Then enter the command as follows:</p>
<pre><code>ownerid 12345678901234567 "Admin Name"</code></pre>
<p class="" style="white-space: pre-wrap;">You can do the same for moderators using the <strong>moderatorid</strong> command</p>
<pre><code>moderatorid 12345678901234567 "Mods Name"</code></pre>
<p class="" style="white-space: pre-wrap;">Note: As with most commands that allow the use of player names, if the name has spaces or special characters in it, you must use quotes to contain the name.Be sure to use the <strong>writecfg</strong> command after doing this and then the person must logout and log back in to receive the permissions. The two permissions are almost identical. Owners can create, kick and ban moderators if needed, but moderators cannot affect owners.</p>
<div class="sqs-block html-block sqs-block-html" data-block-type="2" id="block-yui_3_17_2_2_1427558286432_19844">
<div class="sqs-block-content">
<div class="sqs-html-content">
<h2 style="white-space: pre-wrap;">Sharing Your Server with the World</h2>
<p class="" style="white-space: pre-wrap;">If you wish others to be able to connect to your server from the outside world, you will need to setup a port forward using the port you used listed above. I recommend using this <a href="http://portforward.com/english/applications/port_forwarding/Steam_Server/default.htm">Steam Server Guide</a> if you are unfamiliar with setting up port forwarding. You will need to forward your “<strong>server.port</strong>” as well as “<strong>rcon.port</strong>” if used.  By default these are <strong>28015 </strong>and <strong>28016.</strong></p>
<p class="" style="white-space: pre-wrap;">Even if your server does not show up on the server list, players may be able to connect to you via the <strong>client.connect</strong> command if they know your public IP.  Local firewall programs can also affect the ability to connect from the outside world.  If you suspect this, turn off the firewall briefly.</p>
<p><img src="https://mywild.work/uploads/images/202310/image_750x_653c1991a2480.jpg" alt=""></p>
<p class="" style="white-space: pre-wrap;"></p>
</div>
</div>
</div>
<h2 data-sourcepos="50:1-50:13">Conclusion</h2>
<p data-sourcepos="52:1-52:183">Building a Rust server using a batch file and post install is a relatively straightforward process. By following the steps above, you can have a Rust server up and running in minutes.</p>
