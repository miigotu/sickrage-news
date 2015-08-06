## News from SickRage developers

<br/>

####Please read [Wiki/FAQ](https://github.com/SiCKRAGETV/sickrage-issues/wiki) before opening an issue####
All issues and error reports must be opened at [GitHub](https://github.com/SiCKRAGETV/sickrage-issues/issues) and you **MUST** follow **ALL** [guidelines](https://github.com/SiCKRAGETV/sickrage-issues#submitting-a-bugissue-ticket)

We can track better errors reports in GitHub. Not so much in SickRage forum

<br/>

####2015-08-06####

 - We need some help writing the Wiki for Anime. If you want to help please contact neoatomic in IRC
 - All Wiki pages are now at this [URL](https://github.com/SiCKRAGETV/sickrage-issues/wiki) so users can contribute

<br/>

####2015-07-24####

 - if you have issues with strange characters (ie. ƒÆ'A+â?TAƒâ) in files names and/or in the SR interface and/or your database file (sickbeard.db) is suddenly way bigger than it should be please FULL update & refresh all your shows and force a mass rename after. Depending on your library size it can take some minutes or some hours. Backup DB first.

<br/>

####2015-07-23####

 - Now you can choose your default page when opening/logging to SR (General Options > Misc > Initial page)

<br/>

####2015-07-21####

- Added ability to run an external script for every subtitle downloaded (can be used to embed subs in mkv/mp4)
    For info about the parameters passed see [PR#2139](https://github.com/SiCKRAGETV/SickRage/pull/2139)

- Added IRC tab in web ui, to connect to the SickRage IRC channel

<br />

####2015-07-18####

- Added setting to disable SSL certificate verification under config -> general -> advanced settings
  (Committed on July 15)

  This might help if you have SSL errors

<br/>

####2015-07-17####

- Added new sub-menu called "Changelog". You can check what has changed in SickRage in each release

<br/>

####2015-07-16####

+ **Default Episode Status**: We recently fixed this feature so you need  to:

    - Edit your shows via 'Mass update' and set the default status to WANTED instead of SKIPPED (if you want unaired episodes to be downloaded)
    - Set all new episodes that were marked SKIPPED before that to WANTED. You can check all of them at "Episode Status Management" selecting "SKIPPED" in "Manage episodes with status". Be carefull with this! Make sure you have a backup of your database. Be advised!
    - Now when you will add a **NEW** show you will be asked for two status settings: already aired episodes and unaired episodes.

<span style="margin-left:100px">
<img src="https://cloud.githubusercontent.com/assets/2620870/8724471/3cb943f4-2ba6-11e5-99cd-d645fb9e824f.png" width="300">
</span>

+ **Providers:** Sick beard index and Womble provider are blocking SR application so avoid using them

+ **Develop branch**

    - We are upgrading Subliminal module and this may and will break your installation
    - Please avoid using the develop branch until we fully tested everything unless you know what you are doing
