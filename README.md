# React Self Editor

If I can build a fullstack React app with file system access,

Why can't I build a React app, that can edit itself? 

LOL. I can of course. {:

For my next trick, Npm install root directory and client. 

Run in dev mode, and edit, create or delete react components from the front end. Save them and watch your changes live in real time.

Obviously if it you break something, you have to go in to the components via text editor to fix. LOL.

---------------

Below is info from my React File Manager Build. So far this is the same build with a different path.

------------------------

Who said React can't access a computer's file system? With Node/Express it can.

Create, Read, Update and Delete files with React and Express.

This branch contains .env variables on both the client and server side.

The client .env contains the following:

REACT_APP_MY_ENV=yourPasswordForFrontEnd

REACT_APP_API_SECRET=yourBackEndSecret

the server side .env (root directory) .env contains:

API_SECRET=yourBackEndSecret

Create two .env files, include these variables, and make your secrets match up!

Files parsed come from the directory: client/src/filesToParse

A list of all files in the directory is displayed. 

Clicking on a file will open an editor where you can:

 1. Edit the text of a file. 
 2. Rename a file
 3. Delete a file

 The + button creates a new file.
 ** creates a new directory. currently just one directory of depth, until I get bored and fix it :)
 
 That's pretty much it! 

FIRST:

create a file named ".env" in the client directory.

add the following variable: REACT_APP_MY_ENV="whateverPasswordYouChoose".

This is a simple hard-coded password protection, useful for remote deployment.
 
# Use "remoteBranch" for remote deployment. 

!!!For remote deployment!!! 

In client/src/fileManager.js, replace the server ip address with your own server ip in ALL axios requests:    
axios("http://myVeryOwnServer:5000/createFile/", ...)

TO RUN: 

1) npm install in root directory

2) cd client

3) npm install

4) back to root directory

5) npm run dev

Cheers!
𝓛ⲉⲓ𝓯 Ⲥⲏꞅⲓ𝛓ⲧⲓⲁⲛ


