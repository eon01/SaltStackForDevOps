# Preface

        o   ^__^
         o  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||

## Every Book Has A Story, This Story Has A Book

I wanted to quickly resign from that job, my suggestions about setting up a continuous delivery/deployment have not been considered! I'm lazy and there are hundreds of configuration files and thousands of variables to copy from an excel file and to reconfigure in some platforms, a huge number of poorly-configured servers; hundreds of servers to manage. .  I wanted to work on the automation of procedures, I was aware that this is the solution, that was not the priority of the customer.

It was a position within a team of ten people working on the integration of a number of  heavy applications. At the beginning, I was obliged to follow my colleagues and my boss in the methods of work they have adopted which have one goal : satisfy the unceasing demands of the customer.

No, but .. wait, this is not good at all!

I spent almost two weeks searching and working on some solutions before I convinced my boss to give me the time to set up what I am working on, so that it can ease the heavy load, accelerate daily procedures and reduce human errors. Among other procedures I have set up, I found Saltstack the perfect solution that meets the expectations of integration process, or rather,  the continious integration, deployments and tests.

I hesitated between several alternatives: puppet, CFEngine, Ansible .. etc. The choice was made based on several criteria and I have never regretted.

In the beginning I wanted to resign from my job, just few days after of the discovery of Salt, I was in love with my job, with what I was doing and with Saltstack.

Well, I tried SaltStack first time when I saw my team taking more than 3 days to configure hosted platforms at each deployment. After using SaltStack, the same procedure was taking less than 1/2 hour.

Through this book, it's your turn to discover Saltstack, I am your guide.

I wish you a pleasant reading.

## To whom is this book addressed ? 

To developers, system administrators and anyone faced to work in one of these environments in collaboration with the other or simply in an environment that requires knowledge in development and system administration.

The most common idea, is that developers think they are here to serve the machines by writing code and applications, systems administrators think that machines should works for them, simply by making them happy.

Moreover, within the same company there is generally some tension between the two teams:

System administrators accuse developers to write code that consumes memory, does not meet system security standards or not adapted to the configuration of available machines.

Developers accuse system administrators to be lazy, to lack innovation and to be seriously uncool!

No more mutual accusations, now with the evolution of software development, infrastructure and methodologies adopted (such as Agile / Scrum), the concept of Devops was born.

The DevOps is a concept and a job that seeks closer collaboration and a combination of different roles involved in software development such as the role of developer, responsible for operations and responsible of quality assurance. The software must be produced at a frenetic pace while at the same time the developing in cascade seems to have reached its limits.

If you are a fan of this concept, if you are a system administrator working on software operations, if you are a start up developer seeking to join the new movement this book is addressed to you.

## Conventions used in this book

Basically, this is a technical book where you will find commands (Saltstack commands) and code (Python, YAML, Jinja2 ..etc). Commands and code are written in different fonts.

Example :

```
python -c 'import urllib; print urllib.urlopen("https://bootstrap.saltstack.com").read()' | \ sudo  sh -s -- git develop
```

- Some technical words are *quoted* Some others are using **bold** or *italic* font. The goal is to get your attention when you're reading and help you identify keywords.
- You will find two icons, I have tried to be as simple as possible so I have chosen not to use too many symbols, you'll only find:

![](images/info.png) To highlight useful and important information.

![](images/error.png) To highlight a warning or to prevent.

##How to properly enjoy this book
This book contains technical explanations and shows in each case an example of a command or a configuration to follow. The only explanation gives you a general idea and the code that follows gives you convenience and help you to practice what you're reading. Preferably, you should always look both parts for a maximum of understanding.
Like any new tool or programming language you learned, it is normal to find difficulties and confusions in the beginning, perhaps even after. If you're not used to learn new technologies, you can even have a modest understanding while being in an advanced stage of this book. Do not worry, everyone has passed at least once by this kind of situations.
At the beginning try to make a diagonal reading while focusing on the basic concepts, then try the first practical manipulation on your server or just using your laptop and occasionally come back to this book for further reading on a about a specefic subject or concept.
This book is not an encyclopedia, but sets out the most important parts to learn and even to master Saltstack, if you find words or concepts that you are not comfortable with, just try take your time and do your research. Learning can be serial so understanding a topic require the understandding of other topics.
Through this book, you will learn how to install configure and use Saltstack. Just before finishing the book, you will go through a chapter where a good example of a practical use case is explained. Through this chapter, try to showcase your acquired undrestanding, and no it will not hurt to go back to previous chapters if you are unsure or in doubt.
Finally, try to be pragmatic and have an open mind if you encounter a problem. The resolution begins by asking the right questions.

## How to contribute to this book ?
This work is in progress. I am an adopter of the lean philosophy, so the book will be continuously improved in function of many criteria, but the most important one is your feedback.
If you have any suggestions please do not hesitate to contact me, you can find me on [Twitter](https://twitter.com/eon01) or you can use [my blog contact page](http://eon01.com/blog/contact-me/). 

This book is not perfect, so you can find typo, punctuation errors or missing words, like in every book but every line of the used code was tested before (I used mainly Redhat and Debian distributions).

## About The Author
[Aymen El Amri](http://eon01.com) is a Linux/web engineer, he worked on development and system administration for companies and co-founded some projects in connection with the community of free and open source software. He is more and more interested in the DevOps philosophy, the lean programming and the tools/methodologies that comes with since his last experiences in this domain were successful.
