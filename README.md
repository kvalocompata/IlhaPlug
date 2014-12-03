basicBot-customization
Click here for basicBot's main repository.

Using custom room settings or adding functionality is done by loading your own script loading and modifying the bot. This repository's purpose is to facilitate this. You can fork the repository and customise the example script. When you have forked the repo, bookmark the following script, but change Yemasthui to your own github handle.

javascript:(function(){$.getScript('https://rawgit.com/Yemasthui/basicBot-customization/master/extension.js');})();

If you are using your own hosting service for your script, swap the link with your own.

A detailed overview of the possible settings can be found here.

(A custom .json file can still be used for custom file settings, but is discouraged as the method provided here allows for more customization.)

Blacklists

Blacklists can be added in the settings through either links to raw json files with the same format as those in the examples provided (forking and using rawgit's development link is a great way to do this), or replacing the link with a custom function that loads your lists into the bot (this option requires extensive knowledge of javascript and a good understanding of the bot's inner workings).

To update your lists manually, you can use the details specified in chat messages after a song is blacklisted, or use either of these in the console periodically:

bot.getNewBlacklistedSongs(); //get a javascript object
bot.logNewBlacklistedSongs(); //get a list
Copyright

Copyright © 2014 Yemasthui
