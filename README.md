# emoji

First, obtain a JSON of the emoji list from your original workspace by going to https://api.slack.com/methods/emoji.list/test and inputting your admin token.

Then, copy the JSON into a file called `emoji.json`, and keep only the object named "emoji" (i.e. wipe "ok" and "cache_ts"). Essentially, remove everything until you have just a single map of emoji names to urls. I have included an example `emoji.json` file.

Place this file in the same directory as `script.py`. Then, run the Python script:
```sh
python3 script.py
```
which will create all the new image files in the same directory.

From there, you can use the bulk add chrome extension found at https://chrome.google.com/webstore/detail/neutral-face-emoji-tools/anchoacphlfbdomdlomnbbfhcmcdmjej/ to add all the emojis into your new workspace.