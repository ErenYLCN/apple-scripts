# apple-scripts

Useful apple scripts that I use for productivity.

## How to use

osascript <script_name>.scpt <arguments>

## Scripts

1. prep: Takes project path as an argument and creates 3 instances of iTerm 2:
   - First instance: Opens the project with nvim
   - Second instance: Runs 'npm run dev' in the project directory
   - Third instance: Extra tab for running other commands on project root such as 'git status'
