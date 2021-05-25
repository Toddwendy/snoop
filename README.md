Snoop project
=============

## Snoop Project is one of the most promising OSINT tools for finding nicknames.
- [X] This is the most powerful software taking into account the CIS location.

<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/snoop.png" />

Is your life slideshow? Ask Snoop.  
Snoop project is developed without taking into account the opinions of the NSA and their friends,  
that is, it is available to the average user.  

Snoop is a research project (proprietary database / closed bugbounty)  
in the field of search and processing of public data on the Internet.  
In terms of specialized search, Snoop is able to compete with traditional search engines.  

Comparison of indexing database nicknames of similar tools:  
Snoop ** ~ 1900 ** sites;  
Spiderfoot ** ~ 350 ** sites;  
Sherlock ** ~ 350 ** sites;  
Whatsmyname ** ~ 290 ** sites;  
Namechk ** ~ 100 ** sites.  

| Platform | Support |
| ----------------------- |: ---------: |
| GNU / Linux | ✅ |
| Windows 7/10 (32/64) | ✅ |
| Android (Termux) | ✅ |
| macOS | ❗️ |
| IOS | 🚫 |
| WSL | 🚫 |  

Snoop for OS Windows and GNU / Linux
==================================

** Snoop Local database **
<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/snoop_run.png" />  
[Snoop Full version database 1900+ websites ⚡️⚡️⚡️] (https://github.com/snooppr/snoop/blob/master/websites.md "Database Snoop")    

## Release / Release
snoop.exe (for Windows) and snoop (for GNU / Linux)  
🇷🇺 🇺🇸 [Download Snoop Project] (https://github.com/snooppr/snoop/releases "download ready-to-use Snoop build for Windows and GNU / Linux")  

** RU **: Snoop comes with ready-made assemblies (release) and does not require dependencies (libraries) or python3 installation,
that is, it runs on a clean machine with OS Windows or GNU / Linux.  
** EN **: Snoop comes with ready-made assemblies (release) and does not require dependencies (libraries) or python3 installation, that is, it runs on a clean machine with OS Windows or GNU / Linux.  
 
<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/Run.gif" />  

Snoop project plugins
======================

## 1. Demonstration of one of the methods in the Plugin - [GEO_IP / domain]  
<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/GEO_IP.gif" />  

** Reports are also available in csv / txt / CLI / maps **  
<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/GEO_IPcsv.jpeg" />  

## 2. Demonstration of one of the methods in the Plugin - [Yandex_parser]  
<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/Yandex_parser.gif" />  

** Search report dozen username (Plugin - Yandex_parser) **  
<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/Yandex_parser 4.png" />  

## 3. Demonstration of one of the methods in the Plugin - [Reverse Vgeocoder]  
<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/RVG.gif" /> 

<details>
<summary> Using </summary>  

** Russian version - of Snoop see release (available 'Snoop EN version'). **
``,
$ python3 snoop.py --help

usage: snoop.py [-h] [--donate y] [--version] [--verbose] [--base]
                [--web-base] [--site] [--time-out] [--found-print] [--no-func]
                [--userload] [--list all] [--country] [--save-page]
                [--cert-on] [--normal] [--module y] [--update y]
                USERNAMES [USERNAMES ...]

Snoop: nickname search on all fronts! (Version :: Source 1.2.9D_rus Snoop for GNU / Linux)

positional arguments:
  USERNAMES The nickname of the wanted user, supported
                        several names

optional arguments:
  -h, --help show this help message and exit
  --donate y, -dy Donate to Snoop development. Buy full version
  --version, - about, -V BEGIN! Printing versions: OS; Snoop;
                        Python and Licenses
  --verbose, -v When searching for 'username', print
                        detailed verbalization
  --base, -b Specify another database to search for 'username' (Local)
  --web-base, -w Connect to search for 'username' to updatable
                        web_DB (Online)
  --site, -s Specify the name of the site from the database '--list all'. Search for 'username'
                        on one specified resource
  --time-out, -t 9 Set max timeout to wait for a response
                        from the server (seconds). Affects the duration
                        search. Affects 'Timeout errors:' On. this option
                        it is necessary with a slow Internet connection in order to
                        avoid long freezes in case of network problems
                        (by default, the value is set to 9s)
  --found-print, -f Print only found accounts
  --no-func, -n ✓ Monochrome terminal, don't use colors in url
                        ✓ Mute the sound ✓ Prevent the opening of the web browser
                        ✓Disable printing of country flags ✓Disable
                        indication and status of progress. Saves system resources
                        and speeds up the search
  --userload, -u Specify a file with a list of users. Example, 'snoop -u
                        ~ / snoop / listusers.txt start '
  --list all Print local database information
                        Snoop
  --country, -c Sort 'print / write_results' by
                        countries, not alphabetically
  --save-page, -S Save found user pages to
                        local files
  --cert-on, -C Enable verification of certificates on servers. Default
                        verification of certificates on servers is disabled, which gives
                        fewer mistakes and more positive results with
                        looking up username
  --normal, -N Mode switch: SNOOPninja> normal mode>
                        SNOOPninja. Default (GNU / Linux Full Version) on
                        'SNOOPninja mode': search acceleration ~ 25pct, saving
                        RAM ~ 50pct, re-flex on bad
                        resources. SNOOPninja mode is only effective
                        for Snoop for GNU / Linux Full Version. Default
                        (Windows) on 'normal mode'
  --module y, -my OSINT search: using various Snoop plugins (list
                        plugins will be added)
  --autoclean y, -ay Delete all reports, clear space
  --update y Update Snoop source
``,

** Example **
``,
# To search for just one user:
$ python3 snoop.py username1 #Running from source
$ snoop username1 #Running from release
# Or, for example, Cyrillic is supported:
$ python3 snoop.py olesya #Running from source
# To search for a name containing a space:
$ snoop "ivan ivanov" #Running from release
$ snoop ivan_ivanov #Running from release
$ snoop ivan-ivanov #Running from release

# Run on OS Windows:
$ python snoop.py username1 #Running from source
$ snoop.exe username1 #Running from release
# To search for one or more users:
$ snoop.exe username1 username2 username3 username4 #Running from release

# Search for multiple users - sorting the output of results by country;
# avoid freezing on sites (more often the 'dead zone' depends on your ip-address);
# print only found accounts; save pages found
# of accounts locally; specify a file with a list of wanted accounts;
# connect to search for Snoop's extensible and updatable web-base:
$ snoop -с -t 6 -f -S -u ~ / file.txt -w start #Running from release
# check the Snoop database:
$ snoop --list all #Running from release
# print help for Snoop functions:
$ snoop --help #Running from release

# Include Snoop plugins:
$ snoop --module y #Running from release

# 'ctrl-c / z' - interrupt the search # it is not recommended to interrupt the search in this way in the 'SNOOPnina' mode.
$ kill $ (ps aux | grep python / snoop | awk '{print $ 2}') # cure for offloading RAM on interrupts.
``,
The accounts found will be stored in ~ / snoop / results / * / username. {Txt.csv.html}.  
Root is required to access search results on Android platform.  
csv open in * office in ** utf-8 ** encoding, field separator ** comma **.  

Destroy ** all ** search results - delete the directory '~ / snoop / results'.  
or `` snoop.exe --autoclean y #Running from release OS Windows``
``,
# Update Snoop to test new software features:
$ python3 snoop.py --update y # Git installation required.
``,
</details>  

<details>
<summary> Self-build software from source </summary>  

** Native Installation **  
Note: the required python version is 3.7; 3.8 or 3.9

``,
# Clone the repository
$ git clone https://github.com/snooppr/snoop

# Enter the working directory
$ cd ~ / snoop

# Install python3 and python3-pip if not installed
$ apt-get update && apt-get install python3 python3-pip

# Install the 'requirements' dependencies
$ pip install --upgrade pip
$ python3 -m pip install -r requirements.txt
# Or install all dependencies from 'requirements.txt' manually via
$ pip3 install module
# If special characters are displayed instead of country flags, deliver a font package such as monochrome
$ apt-get install ttf-ancient-fonts or colored apt-get install fonts-noto-color-emoji
# On Windows OS use cmd or powershell (your choice of convenience), but not WSL!
``,
</details>

<details>
<summary> Snoop for Android </summary>  
search username
<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/snoopandroid.png" />  

plugins
<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/Snoop_termux.plugins.png" />  

** Native Installation **  

Install [Termux] (https://play.google.com/store/apps/details?id=com.termux&hl=en "Google Play")  
``,
# Note: installing Snoop on Termux is time consuming
# Enter Termux home folder (i.e. just open Termux)
$ termux-setup-storage
$ ls # / data / data / com.termux / files / home # default / home directory

# Install python3 and dependencies
$ apt update && pkg upgrade && pkg install python libcrypt libxml2 libxslt git
$ pip install --upgrade pip

# Clone the repository
$ git clone https://github.com/snooppr/snoop -b snoop_termux
# (If the flash drive is FAT (not ext4), in this case,
# clone the repository only to the Termux HOME directory)

# Enter the Snoop working directory
$ cd ~ / snoop
# Install the 'requirements' dependencies
$ python3 -m pip install -r requirements.txt


# Add-on for outdated gadgets (Android 6)
# Note on modern gadgets the packages are already preinstalled and configured
# add any 'random' name and mail:
$ git config --global user.email "you@example.com"
$ git config --global user.name "username"
# Install coreutils
$ pkg install coreutils
``,
</details>

<details>
<summary> Basic errors in </summary>

| Party | The problem | Solution |
|: ---------: | -------------------------------------------------- ---- |: -------: |
| ========= | =========================================================================================================================================================== =============== | ======= |
| Client | Connection blocking by proactive protection (* Kaspersky) | 1 |
| | Insufficient speed of the Internet connection EDGE / 3G | 2 |
| | Too low value for option '-t' | 2 |
| | invalid username | 3 |
| | Connection errors: [GipsysTeam; RamblerDaing; Mamochki] | 7 |
| | Connection errors: [Virtualireland; Forum_rzn; Ddo] | 7 |
| ========= | =========================================================================================================================================================== =============== | ======= |
| Provider | Internet Censorship | 4 |
| ========= | =========================================================================================================================================================== =============== | ======= |
| Server | Site changed its response / API; updated CF / WAF | 5 |
| | Blocking by the server a range of client ip-addresses | 4 |
| | Triggering / protecting the resource captch | 4 |
| | Some sites are temporarily unavailable, technical work | 6 |
| ========= | =========================================================================================================================================================== =============== | ======= |

Solutions:
1. Reconfigure your Firewall (for example, Kaspersky blocks Adult Resources).

2. Check the speed of your internet connection:  
$ python3 snoop.py -v username  
If any of the network parameters are highlighted in red, Snoop may freeze while searching.  
At low speed, increase the 'x' value of the '--time-out x' option:  
$ python3 snoop.py -t 15 username  

3. In fact, this is not a mistake. Fix username  
(for example, some sites do not allow Cyrillic characters; "spaces"; or 'Vietnamese-Chinese_encoding'
in usernames, in order to save time: - requests are filtered).

4. ** Change your ip-address **  
("Gray" ip and censorship are the most common causes of which the user receives skip / false positive errors / and in some cases '** Alas **'.  
When using Snoop from the IP address of a mobile operator's provider, the speed ** may ** drop significantly, depending on the provider.  
For example, the most effective way to solve the problem is ** USE VPN **, Tor is not very well suited for this task.  
Rule: one scan from one ip is not enough to get the most out of Snoop).

5. Open in Snoop repositories on Github-e Issue / Pull request  
(inform the developer about it).

6. Do not pay attention, sites sometimes go to repair work and return to service.

7. [Problem] (https://wiki.debian.org/ContinuousIntegration/TriagingTips/openssl-1.1.1 "easy and solvable problem") with openssl on some GNU / Linux distributions.  
Decision:
``,
$ sudo nano /etc/ssl/openssl.cnf

# Change at the very bottom of the file the lines:
[MinProtocol = TLSv1.2]
on the
[MinProtocol = TLSv1]

[CipherString = DEFAULT @ SECLEVEL = 2]
on the
[CipherString = DEFAULT @ SECLEVEL = 1]
``,
</details>

<details>
<summary> Additional information </summary>

[Project development history / History] (https://raw.githubusercontent.com/snooppr/snoop/master/changelog.txt "Project development history")  

[Snoop Project / License] (https://github.com/snooppr/snoop/blob/master/COPYRIGHT)  

[Documentation / Documentation] (https://drive.google.com/open?id=12DzAQMgTcgeG-zJrfDxpUbFjlXcBq5ih)  

** Public key fingerprint: ** [076DB9A00B583FFB606964322F1154A0203EAE9D] (https://raw.githubusercontent.com/snooppr/snoop/master/PublicKey.asc "pgp key")  

** Information for civil servants: ** Snoop Project is included in the register of domestic software. Order of the Ministry of Telecom and Mass Communications of the Russian Federation No. 515, register No. 7012.  

** Snoop is imperfect: websites are crashing; there are no end tags; hosting is not paid on time. From time to time it is necessary to keep an eye on all this "Web rock 'n' roll", so donations are welcome: **  
[Examples of DB correction / Example close / bad websites] (https://drive.google.com/file/d/1CJxGRJECezDsaGwxpEw34iJ8MJ9LXCIG/view?usp=sharing)
** BTC (donation): ** 1Ae5uUrmUnTjRzYEJ1KkvEY51r4hDGgNd8  

** email: ** snoopproject@protonmail.com
</details>
<img src = "https://raw.githubusercontent.com/snooppr/snoop/master/images/zvezda.jpeg" />
