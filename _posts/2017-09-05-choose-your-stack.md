---
layout: post
title:  "Choose your stack"
date:   2017-09-05
categories: development
---

## Choosing your stack:
Once you have a domain and traffic is being routed to your server, it is then time to choose your software stack.

### A few things I took into consideration
As with any endeavor, upfront planning now will save time, money and stress later on.  In the sub-sections below I will reason about the software stack selections I have chosen.

#### Cost of ownership
Simply put, a Windows environment is just more expensive to run and license.  So that was enough of a reason for me to rule out the .NET stack.

#### DevOps
I can certainly maintain my own servers, but I do not want to feel like this is more of a task than building the application.  So I will not choose anything that I know will take up too much of my time to maintain.

#### Language Selection
I began by weighing my personal preferences against what makes the most sense in an effort to reach a Minimum Viable Product in a reasonable time-frame.

That said, I am most familiar with .NET development for server side processing and HTML / CSS and JavaScript for front-end development.

---

##### ~~Ruby~~
This is my favorite language to develop in. I also love the speed at which a site can be created using Ruby on Rails.
- Its beautiful
- Its minimal
- Fast development time

But at the end of the day, I have a love-hate relationship with Ruby on Rails. In my experience, keeping the server OS updated with the latest updates has always been a headache because of software version conflicts, gem dependency issues, or incompatibility issues of some kind.  Of course, this is not always the case... but it is enough of an issue for me that I am ruling RoR out as my chosen language / framework.

---

##### ~~.NET~~
I am very familiar with .NET and ASP.NET is a solid choice. 

So the pros:
- It is more than capable.
- I like the C# syntax.
- Visual Studio is awesome.
- Resharper makes me better and more efficient.
- Mature and stable.

And the cons:
- I do not want to be tied to the Microsoft Stack.
- Software licenses can get expensive ...and fast.
- I prefer open source ( yes .NET is now open source, and there is Mono and .NET Core... But its still very much tethered to Microsoft at the moment ) and I don't think running either of these on Linux is a good choice when compared to some of the other options available today.

---

#### ~~PHP~~
PHP has come a long way other the years, and a lot of the web runs on PHP.  I do not believe that there is any question that PHP could handle my needs, but more a question of personal preference.

And to be honest, I am not in love with PHP as a language ( mostly due to some of its syntax )... So simply out of personal preference, I am ruling this one out as well.

---

#### Honorable mention: ~~Java~~
Java was actually my runner up.  It is capable in every way and would be a good choice for my needs.  But I really like node.js for this project.

---

#### My choice: JavaScript running on node
Speaking of having come a long way... JavaScript has morphed into a very powerful language that is no longer just for client side scripting.  With node.js I can use JavaScript ( a language I already know very well ) on both the front and back end of my web app.

Pros:
- No matter the need... there is a library for that.
- NPM.
- It can be ran on basically everything.
- Environment; It just works.
- Many more.

Cons:
- Single threaded.
- Not great for heavy computational processing.


## Conclusion

### OS / Server / DB:
- I will have a [Ubuntu Linux](www.ubuntu.com) server.
- Running a [Nginx](https://www.nginx.com/) web-server.
- Powering a [node.js](https://nodejs.org/) back-end.
- Connecting to a [MongoDB](https://www.mongodb.com/) database.


I will be building the front-end using [React](https://facebook.github.io/react/) with [Express](https://expressjs.com/) powering the back-end api.

---

Check back soon for updates on the development progress.

[t. payne](http://www.tpayne.net/) @ [tinkr.deisgn](http://www.tinker.deisgn/)
