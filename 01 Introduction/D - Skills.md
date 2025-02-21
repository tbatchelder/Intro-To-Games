# Skills needed for Web Game Development

So you want to make a web game. Ok, but what skills do you need in order to do so?

Creating games is an intricate and demanding job, requiring a blend of skills and tools. Having the right tools in your arsenal can significantly impact your success.

Having the right tools in your toolbox is essenctial for streamlining workflows, enhancing game performance and improving the player experience. Whether you're developing a small mobile game or a large-scale PC/Console game, from concept art to coding and debuggin, the tools you choose will shape the outcome of your game.

Gathered below are research notes I've run across on the skills needed, sorted by what I feel is most important for each section.

## The Hard Skills

These skills are not "hard" in the sense that they are difficult to learn the basics of but are instead the knowledge skills you will need to program the game.

- _HTML / CSS / JavaScript_

  You absolutely need HTML/CSS/JavaScript. There is no way around it. Every bit of code which will be running in the user's browser on their device must be in one of these 3 languages. Try to shift as much of your game's code as possible to the front-end without sacrificing security.

- _React, NextJS, Tailwind, Prisma, etc._

  Whether you will need these frameworks / libraries or not depends upon what you are designing and building. There are an immense host of other frameworks and libraries avaiable as well that can make the buidling process smoother. Some even cater specifically to game development.

- _Test Driven Development (TDD)_

  A software development process that involves writing tests before writing code. This creates higher quality code and can identify bugs before they roll out to users. Learning can produce cleaner code that does more with less coding.

- _IDE (Integrated Development Environment)_

  These are software programs that give developers a full development environment for testing, debugging and modifying code. They typically come with support for collaboration, version control and project file management. Additionally, they help you code better by using extensions that find errors before you roll your game out.

- _Version Control_

  You need to know a version control tool.

- _Graphics Editors_

  These are software programs used to develop the game's visual components such as characters, backgrounds and animations.

- _Audio Tools_

  You need to know an audio tool or where to get audio from.

- _Game Engines_

  These are pre-built frameworks that drive a game. These typically come with pre-built physics, graphics, animination and more. While knowing how to use this is an assest, it is not needed to start building your first game.

- _Backend / Server_

  You can use any language for the back-end. PHP, Python, JavaScript (Node.js), Java, Ruby, Go, etc. The list is endless. Really it comes down to picking a language you want to work in and has tools that you feel would be helpful. For example, if you feel you could share code between your client and server, it might make sense to make your server in Node.js so you can reuse that JavaScript code.

---

## The Soft Skills

These skills below are the often over-looked skills that encompass ability, communication, drive and desire.

---

## The Gotchas

These are not so much skills but things you need to code for and prepare for when designing and builing any game.

- _Hacking Attempts_

  Remember that the client cannot be trusted. In an online game, you must assume that every player is a hacker and is using a modded client. You must code defensively and sanitize/validate every input you receive to the server. This being said, find the least number of aspects that you need to check to be confident that the inputs are legitimate. For some games this requires sending every mouse/keyboard input directly to the server to process, other games might just be distinct API calls with most of the data already stored on the server.

- _Hosting_

  Something else to consider when architecting your game, try to make it serverless. This will likely result in a much cheaper and easier to manage server experience and will automatically scale with traffic. I'd specifically recommend AWS for hosting here.

  The main idea with serverless is that every piece of your application (or as many as possible) can scale from 0-infinity automatically. So if no one is playing everything scales to 0 and you are essentially charged nothing. And if you get a surge of players, everything automatically scales up to handle it.

- _Client Resources_

  You have to design every part of your application to be stateless (in memory). If you do need state, it must be stored to disk.

[Essential Game Development Tools You Need in Your Arsenal](https://sdlccorp.com/post/essential-game-development-tools-you-need-in-your-arsenal/)
