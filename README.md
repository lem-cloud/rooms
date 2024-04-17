# Rooms

Powerful web-based Editor with collaborative editing

## What is this?
This project is to provide the text editor [Lem](https://github.com/lem-project/lem) as a web service.

When a user creates a room, an instance of Lem is launched in that room.  
In this room, the user can freely use the complete Common Lisp environment.

All you need is a web browser and a GitHub account.  
In Rooms, when a user creates a "room" an instance of Lem is launched.  
Users can then utilize a complete Common Lisp environment within their web browser.  
No installation of dependent libraries or local build environments is required.  
Additionally, Rooms supports usage on various devices including tablets and smartphones with the aid of a Bluetooth keyboard.  
It also supports editing the same file across different devices (Linux, macOS, iPad, etc).  
Invite others to your room, and collaborate seamlessly on a single instance of Lem.

## Project Status
This project is in its alpha stage.  
So, it comes with a limitation that only those who have been invited can create rooms.

## Technology stack
The technology stack is almost entirely Common Lisp.  
The server side uses web frameworks such as crack and ningle, and the ORM uses mito.  
The front end uses react, which compiles Common Lisp into JavaScript with [valtan](https://github.com/cxxxr/valtan).  
The core of the editor, the canvas operation, requires performance, but due to efficiency issues with the code output by valtan, the JavaScript is written by hand.  
I am sure that future improvements to the valtan compiler will solve this problem, but anyway, there is too much to do and not enough time to do it now.

## GitHub Sponsors
This project is looking for sponsors.  
https://github.com/sponsors/cxxxr
