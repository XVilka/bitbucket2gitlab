# bitbucket2gitlab

At Inbot we recently set up our own Gitlab server and we needed to port our issues over from bitbucket. Since I could find no tool to do this, I hacked together a quick tool that gets the job done.


Instructions:

- from bitbucket export the issues from your project. You should get a zip file with a json file inside
- modify the global variables inside bitbucket2gitlab.rb to match your project settings
- run the script, I recommend testing this with a test project in gitlab that you can discard before running this against the real thing

Limitations
- it gets you the raw content (comments and issues) but things like milestones, assignments, create timestamps, etc are lost
- comments are in the order they are listed in the dump

# Pull requests

This was a quick and dirty job. Somebody with spare time could likely find many ways to improve it. Therefore feel free to **fork and own**. We're done with bitbucket so we won't need this script again. The License allows you to do what you want but we do appreciate being mentioned.
