# rcAllowNet
bashrc command to wrap current shell ... or change os to whitelist network traffic to specific urls.

plan:
1. create function to put in bashrc file that will read from a whitelist file and restrict traffic to only what is in that file.
2. trap on exit of the terminal to turn this off.
3. launch agent to turn this off on startup or wake from sleep.

research:
1. need to find out how to monitor url traffic in bash (on mac computer for now)
  a. tldr nettop
  b. https://gist.github.com/jjnilton/add1eeeb3a9616f53e4c
  c. nettop -t wifi

potential other features:
1. show which urls bounceback due to failing the whitelisting
2. allow-read rights to file system (whitelisting files).
3. quickly enable and disable
