This bot is super simple right now! Kinda only has one function (and might stay that way) 

**Content Warnings

To add a warning/associate with your user the chat command is: *@[botname] warn [keyword]

The bot will reply with a confirmation message, and add an array containing the keyword to a JSON object with the key the name of the user - or update an existing one. It also adds the keyword to a list of all the words it's keeping an eye on. 

Once you're done talking about a subject that you think/know required content warnings, sound the all-clear with: *@[botname] safe [keyword]

This will send a message out to anyone that has made the bot aware of their aversion to the subject in question. 


In the background, the bot scans every message for items from the list of all keywords. If found, it searches each user's personal lists and if it finds the keyword it adds them to the list of users that need warning. Then the bot sends a DM to every user on that list with the type of content as well as the channel.


**Upcoming updates: 

*(open an issue or something or hit me up elsewhere if there's anything anyone would like to see added/fixed/updated)

1. Rate limiting on the DM warnings, currently it sends a warning every time the word is mentioned so it's kinda spammy.
2. Cleaning up the code, the thing was made in a bit of a rush and there's at least one instance where I repeated some lines instead of spinning it out into a function. 
3. Sorting out the storage to handle multiple servers if needs be - doesn't need to be more fancy than JSON files given the simplicity of the data being stored, just need to keep the data unique to each server. 
4. Adding the add-bot link to this README so that the bot can be used on other servers. 
5. Potentially add filler text/nice images to the channel that the all-clear message is sent in.  
