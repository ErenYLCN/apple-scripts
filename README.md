# apple-scripts

Useful apple scripts that I use for productivity.

## How to use

For running a script, use the following format on terminal:

```

osascript <script_name>.scpt <arguments>

```

To take it to the next level, create a custom script to run the command like this:

1.  Create a `.custom_commands.sh` file with this type of code:

```
#!/bin/bash
function p() {
 osascript prep.scpt $1
}
```

2.  Add `source ~/.custom_commands.sh` to end of your `.bash_profile` file
3.  Voila!

## Scripts

1.  prep: Takes project path as an argument and creates 3 instances of iTerm 2:

- First instance: Opens the project with nvim
- Second instance: Runs 'npm run dev' in the project directory
- Third instance: Extra tab for running other commands on project root such as 'git status'
