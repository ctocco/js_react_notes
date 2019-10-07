# Prettier setup

if someone doesn't want prettier on save or does not have this option then we can put this into a
script that people can run before they commit.

1. npm i -D prettier (install prettier as a dev dependency)

2. in scripts in JSON file

"format" : "prettier \"src/\*_/_.{js, html}\" --write",

3. npm run format (will edit the file with prettier format)

this will target either js or html

if in Visual Studio install prettier then go to settings

select only two things

1. format on save
2. require config - will only edit if there is a prettier config file
3. in your project make a prettierrc file with empty brackets as shown it is just default
