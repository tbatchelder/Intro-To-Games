# Skills needed for Web Game Development

I've been doing some research on the skills you may need in order to make a browser game. Detailed below are some of the skills you may find useful in developing.

- _HTML / CSS / JavaScript_

  You absolutely need HTML/CSS/JavaScript. There is no way around it. Every bit of code which will be running in the user's browser on their device must be in one of these 3 languages. Try to shift as much of your game's code as possible to the front-end without sacrificing security.
  • You can use any language for the back-end. PHP, Python, JavaScript (Node.js), Java, Ruby, Go, etc. The list is endless. Really it comes down to picking a language you want to work in and has tools that you feel would be helpful. For example, if you feel you could share code between your client and server, it might make sense to make your server in Node.js so you can reuse that JavaScript code.
  • Remember that the client cannot be trusted. In an online game, you must assume that every player is a hacker and is using a modded client. You must code defensively and sanitize/validate every input you receive to the server. This being said, find the least number of aspects that you need to check to be confident that the inputs are legitimate. For some games this requires sending every mouse/keyboard input directly to the server to process, other games might just be distinct API calls with most of the data already stored on the server.
  • Something else to consider when architecting your game, try to make it serverless. This will likely result in a much cheaper and easier to manage server experience and will automatically scale with traffic. I'd specifically recommend AWS for hosting here.
  • The main idea with serverless is that every piece of your application (or as many as possible) can scale from 0-infinity automatically. So if no one is playing everything scales to 0 and you are essentially charged nothing. And if you get a surge of players, everything automatically scales up to handle it.
  • You have to design every part of your application to be stateless (in memory). If you do need state, it must be stored to disk.
