## News from SickRage developers

<br/>

####Please read the [Wiki/FAQ](https://github.com/SiCKRAGETV/sickrage-issues/wiki) before opening an issue####
All issues and bug reports must be opened at [GitHub](https://github.com/SiCKRAGETV/sickrage-issues/issues) (not the forum!) and you **MUST** follow **ALL** [guidelines](https://github.com/SiCKRAGETV/sickrage-issues#submitting-a-bugissue-ticket).

<br/>

####2015-09-26####

- Today we introduced our new [Feature Tracker.](http://feathub.com/SiCKRAGETV/SickRage) Let us know what features YOU would like to see added. And cast your vote for the already submitted features. 
- (All feature requests should go to the new tracker, not the forum or issue-tracker.)

####2015-09-20####

- *ShowsRage*
- One of our contributors (MGaetan89) has released his Android application for managing SickRage to Google Play. Be sure to check it out, rate, and provide feedback to show your support.
You can read the full description and information on [Google Play](https://play.google.com/store/apps/details?id=com.mgaetan89.showsrage) and the [ShowsRage GitHub Project](https://github.com/MGaetan89/ShowsRage)

<br />

####2015-09-09####

- As you might have noted the [TVRage](http://www.tvrage.com) website pulled the plug/shut down. And that is causing some issues we needed to address. We pushed a fix that automatically converts the TVRage ID to a TheTVDB ID. So that new data is pulled from theTVDB.com instead. That works for most users but sadly not all. So be aware that when you used TVRage shows, you might experience some issues. Be assured that we are working hard to get this all sorted out.
Also as a consequence of the TVRage shutdown we where forced to push some changes for the theme/layout that where not completely tested. Therefore the Network logos are currently not working. Fix coming soon.

- But not only bad news, we have a brand new [SickRage installer](https://github.com/SiCKRAGETV/sickrage-issues/wiki/SickRage-Windows-Installer) for Windows!

<br />

####2015-09-08####

- We are removing support for autoProcessTV in favor of Clinton Hall's nzbToMedia project, which we have imported in `contrib`
- autoProcessTV will be removed by 31-10-2015. Please update your post-processing scripts or they will break.

<br />

####2015-08-16####

- Switched to using mako templates in master. We should have ironed out all the issues regarding mako in past week. If not, please open an issue, using the guidelines above!

<br />

####2015-08-08####

- Switched to mako in develop branch. Please test it out and report in IRC, or on github. Security improvements such as moving sql out of the templates, form/input/uri validation coming soon. Performance improvements coming also, such as moving js out of the templates.

<br />

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

- Added setting to disable SSL certificate verification under Config -> General -> Advanced Settings
  (Committed on July 15)

  This might help if you have SSL errors

<br/>

####2015-07-17####

- Added new sub-menu called "Changelog". You can check what has changed in SickRage in each release

<br/>

####2015-07-16####

+ **Default Episode Status**: We recently fixed this feature so you need  to:

    - Edit your shows via 'Mass update' and set the default status to WANTED instead of SKIPPED (if you want unaired episodes to be downloaded)
    - Set all new episodes that were marked SKIPPED before that to WANTED. You can check all of them at "Episode Status Management" selecting "SKIPPED" in "Manage episodes with status". Be careful with this! Make sure you have a backup of your database. Be advised!
    - Now when you will add a **NEW** show you will be asked for two status settings: already aired episodes and unaired episodes.

<span style="margin-left:100px">
<img src="https://cloud.githubusercontent.com/assets/2620870/8724471/3cb943f4-2ba6-11e5-99cd-d645fb9e824f.png" width="300">
</span>

+ **Providers:** Sick beard index and Womble provider are blocking SR application so avoid using them

+ **Develop branch**

    - We are upgrading Subliminal module and this may and will break your installation
    - Please avoid using the develop branch until we fully tested everything unless you know what you are doing
