# SaltStack For DevOps
Extremely fast and simple IT automation and configuration management.

Through this book you will learn how to use one of the most powerful System Administrators and DevOps tools.

# What SaltStack For DevOps Teaches

This book is a fruit of long hours of work and self-learning. Through this book, it's your turn to discover Saltstack, I will be your guide.

## The 10 most important tips you’ll learn

- Configuration Management And Data Center Automation.
- Advanced installation of SaltStack with a practical installation case.
- Configuration and troubleshooting.
- SaltStack concepts like master, minion, syndic, key management, runners, configurations, states and top file, event-based execution, formulas.
- Using SaltStack to provision and control a Vagrant environment.
- Using SaltStack with a Docker container and monitoring Docker host system.
- Real world examples: installation and configuration of Apache web server, creating you own private storage cloud (SaltStack + Vagrant + OwnCloud), monitoring minions, scheduling monitoring tasks, automating wordpress / LAMP installation and configuration, using Vagrant and Docker..etc
- A practical cheat sheet.
- SaltStack best practices
- Getting help and contributing to SaltStack community
----------
- Buy it now : http://bitly.com/SaltStackForDevOps
- See more at : http://saltstackfordevops.com/
- Get a free sample : http://bitly.com/1OrL3kv
- SaltStack CheatSheet : https://github.com/eon01/SaltStackCheatSheet


[![](http://saltstackfordevops.com/img/books.jpg)](http://bitly.com/SaltStackForDevOps)

Below, an excerpt taken from SaltStack For DevOps :

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

[Image here] To highlight useful and important information.

[Image here] To highlight a warning or to prevent.

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

# Chapter 0 - Introduction

        o   ^__^
         o  (@@)\_______
            (__)\       )\/\
                ||----w |
                ||     ||

## Configuration Management And Data Center Automation
Configuration management and data center automation are mechanisms to manage the technical description of a system, its components and all of the changes on the configuration during the life cycle of a system or during its different processes.

Source code deployments on multiple environments requires a configuration management and provisioning tool. 

From the development, integration, test, deployment, to the production environment, configuration management becomes a process of normalization of the configuration of the application according to the state of the infrastructure and other requirements. The same process of normalization should be ensured when changing the environment, the infrastructure or when the configuration itself changes.

With the adoption of agile development methods, the process of development, test and deployment of a software component has accelerated and therefore the methods of management have become faster, more automated and more adapted to changes.

Even if many specialists consider provisioning, change management and automation as a business issue, not an IT issue but to make this happen some special technical skills are required. That's why new positions in the IT industry have emerged: DevOps. The illustration below (taken from Wikipedia) shows the essence of the DevOps philosophy. 

[Image here]

Automation is important to the success of critical IT processes that are part of the life cycle of a product, including provision, change management, release management, patch management, compliance and security. Therefore having the technical skills and the know-how are very important to any "lazy but pragmatic sysadmin". This book will help you to learn using one of the most important IT automation configuration management and infrastructure automation/orchestration tool: SaltStack.

## DevOps Tool
Currently, several FOSS and proprietary automation and configuration management tools exists. Choosing one of these tools could based on several criteria.

### Choice Criteria 

**Performance** :  Between the memory consumption, the speed of execution and the adaptation to increasingly complexes architectures, several performance criteria could help you decide on the performance of a such tool.

**License** : You may choose between FOSS and proprietary software. Most of the existing softwares are Open Source. It remains to be seen what FOSS license you should choose: GPL, BSD, Apache, MIT..etc

**Programming Language** : A such tool is coded using a programming language, but it does not mean that the a DevOps will manage and automate ops and servers using the same language. For example, SaltStack uses Jinja and YAML ..etc 
Most of those tools are written in Python, Ruby or Java, but one can also find perl, C and C ++.

**Authentication Methods** : A configuration management or a data center automation tool is based on a model, roughly consisting of clients and a server. The authentication between a client and a server can be automatic, encrypted, secure, fast .. or not.

**Agents** : Some tools use agents that must be installed on the target servers (clients), some tools work without agents and others offer both choices.

**Scalability** : A tool that grows and evolves with the enterprise must provide technical means and capabilities to ensure scalability at several features and extended functional scopes.

**Portability** : Most if not all configuration management tools are compatible with *nix systems. Some servers runs on BSD, AIX, HP-UX, Mac OS X, Solaris, Windows and other OSs. In this case you must see this point: the compatibility. 

Thanks to [Wikipedia](http://en.wikipedia.org/wiki/Comparison_of_open-source_configuration_management_software) and its contributor for the next comparison concerning the portability of the following tools. 


| AIX |  BSD |  HP-UX |  Linux |  Mac OS X |  Solaris |  Windows |    Others |
|------|-------|-----------|----------|------------|---------|---------|---------|
|  Ansible   |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |
|  Bcfg   |  Partial |  Yes |  No |  Yes |  Partial |  Yes |  No |  No |
|  CFEngine   |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |
|  cdist   |   |  Yes |   |  Yes |  Yes |   |  No |   |
|  Chef   |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |
|  ISconf   |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  No |  No |
|  Juju   |   |   |   |  Yes |   |   |   |   |
|  LCFG   |  No |  No |  No |  Partial |  Partial |  Partial |  No |  No |
|  OCS Inventory NG   |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  No |
|  Opsi   |  No |  No |  No |  Yes |  No |  No |  Yes |  No |
|  PIKT   |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  No |  Yes |
|  Puppet   |  Yes |  Yes |  Yes |  Yes |  Partial |  Yes |  Yes |  Yes |
|  Quattor   |  No |  No |  No |  Yes |  Partial |  Yes |  No |  No |
|  Radmind   |  Yes |  Yes |  No |  Yes |  Yes |  Yes |  Yes |  No |
|  Rex   |   |  Yes |   |  Yes |  Yes |  Yes |  Yes |  No |
|  Rudder   |  Yes |  Partial |  No |  Yes |  Partial |  Partial |  Yes |  Yes |
|  Rundeck   |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  No |
|  SmartFrog   |  No |  No |  Yes |  Yes |  Yes |  Yes |  Yes |  No |
|  Salt   |  Yes |  Yes |  Partial |  Yes |  Yes |  Yes |  Yes |  Partial |
|  Spacewalk   |  No |  No |  No |  Yes |  No |  Yes |  No |  No |
|  STAF   |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |
|  Synctool   |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |  Yes |
|  Vagrant   |   |   |   |  Yes |  Yes |   |  Yes |   |

**Documentation, Support and Latest Stable Release:** Keep in mind that the quantity and the quality of official documentations, forums, groups, and paid support differs from a tool to another. A good thing to do is to see the date of the latest stable release, some tools are just no more updated which can cause security risks.

### Popular tools
Among the best and the most popular tools we find : Ansible, CFEngine, Puppet, Saltstack.

[Image here]

Among the best and the most popular tools we find : Ansible, CFEngine, Puppet, Saltstack.

**Ansible** : Combines multi-node deployment and ad-hoc task execution. Manages the nodes with SSH and requires Python (2.4 or later). Uses JSON and YAML modules and state as descriptions. It is built on python but its modules can be written in any language. [Ansible](http://www.ansible.com/home) is one of the most used softwares. It is used by Spotify, Twitter, NASA and evernote.

**Puppet** : [Puppet]( http://puppetlabs.com/) is based on a custom declarative language to describe the system configuration, uses the distributed client-server paradigm, and a library for configuration tasks.  Puppet requires the installation of a master server and client agents on every system that is to be managed. It is used by Vmware, Cisco, Paypal and SalesForce.

**Saltstack** : [Salt](http://saltstack.com/) is what the next chapter of this book will details.

# Chapter I - A Taste Of Salt

        o   ^__^
         o  (==)\_______
            (__)\       )\/\
                ||----w |
                ||     ||

## Presentation 
SaltStack is an Open Source project, you can read and modify its source code under the Apache license. 

Its source code is available on [github](http://girhub.com/salstack/salt).

SALSTACK Inc. is the company behind SaltStack, it was founded by Thomas Hatch, the original creator of SaltStack. SaltStack is used by Apple inc, Rackspace, Photobucket, NASA, LinkedIn, Hulu, HP Cloud Services, Cloud Flare and other know companies.

[Image here]

SaltStack fundamentally improves the way system administrators, integrators and DevOps use to configure and manage all aspects of a modern data center infrastructure.

It provides a different approach to some existing alternatives such as speed and adaptation to the size of the cloud. Several recognized businesses use SaltStack to orchestrate and control their cloud servers and infrastructure and automate the "DevOps Toolchain".

It is built on a platform running relatively fast while allowing remote control of distributed infrastructures, code and data. A layer of security is established while having two-way communications between the different components of this platform.

The following chapters are conceived for new and experienced system administrators, DevOps and full stack developers seeking to manage and configure multiple servers / application and software platforms more easily. 

The infrastructure to manage can be virtual machines, cloud (Amazon EC2 instances, Rackspace ..etc) or physical machines as well hosted applications and platforms that rely on configuration files. All you need is a root access, a good understanding of the environment to manage and the basic know-how for a sysadmin.

Even if it is possible to use a web access to manage SaltStack but the use of the command line is always more adapted to our needs for several reasons such as speed and efficiency. If you are familiar with the command line and programming, understanding Salt commands and its syntax will be easier but this is not a requirement to start using SaltStack.

Salt is portable and works with these systems:

- Amazon Linux 2012.09
- Arch, CentOS 5/6
- Debian 6.x/7.x/8(git installations only)
- Fedora 17/18
- FreeBSD 9.1/9.2/10
- Gentoo 
- Linaro
- Linux Mint 13/14
- OpenSUSE 12.x
- Oracle Linux 5/5
- Red Hat 5/6
- Red Hat Enterprise 5/6
- Scientific Linux 5/6
- SmartOS
- SuSE 11 SP1/11 SP2
- Ubuntu 10.x/11.x/12.x/13.04/13.10
- Elementary OS 0.2

According to the official website of Salt, other systems and distributions will be compatible in the future. If you want to stay informed just follow the development branch.

In the following sections, the installation and the use of SaltStack will be in the context of Linux server management. This could have some small differences for Windows, FreeBSD or Solaris..Etc. Overall, principles are the same.

You can use Salt installed on an operating system to manage other systems (A Linux to manage a Solaris or a BSD to manage a Windows ... etc.). The installation part of this book will cover Redhat and Debian. Be sure to check the documentation (docs.saltstack.com) for the installation and the specific use with your particular operating system.

## A brief summary

SaltStack is based on some special components:

- One or more "salt-master", "salt-minion" and "salt-syndic"
- A key management system "salt-key" that allows the authentication of a "salt-minion" on a "salt-master"
- A system of "states" to describe the configurations
- A "top.sls" that calls the "states"
- A system of "grain" on the minion to manage the configurations data
- A system of "pillars" to store other data on the master (such as confidential data)
- A transport and data management system called “ZeroMQ”
- An event management system called “reactors”
“returners”, “outputters” ..etc

A master can manage configurations or execute remote commands on one or more minions. This operations are based on “SLS” files, and these files are calling Salt modules, grains and/or pillars.

Salt could be used either from the command line or in executable scripts.

The various components of SaltStack will be explained in this book, some definitions appeal to others, that's why in the first order we need to have a global view on the functioning system of Salt.

## Expanding Salt Use

Provisioning and testing tools based on Salt and its GUI will not be part of this documentation, but they are interesting tools if you want to learn more about SaltStack.

Some of this tools are :

### Salty Vagrant

Salty Vagrant is a Vagrant plugin that allows you to use Salt as a provisioning tool. You can use “formulas” and existing configs for building development environments.

The simplest way to use Salty Vagrant is configuring it to work in “masterless” mode. Details are explained in the [official Vagrant documentation](https://docs.vagrantup.com/v2/provisioning/salt.html).

### Salt Cloud

[Salt Cloud](https://github.com/saltstack/salt-cloud) is a public cloud provisioning tool created to integrate Salt to each of the major cloud infrastructure providers (AWS, Rackspace, Parallels ..etc) in order to facilitate and accelerate the supply process.

Salt Cloud allows managing a cloud infrastructure based on “maps” and “profiles” of virtual machines. This means that many virtual machines in the cloud can be managed easier and faster.

### Halite

[Halite](https://github.com/saltstack/halite) is the client-side web interface (Salt GUI). It connects and operates a SaltStack infrastructure. This tool is a graphical complement, but it is not indispensable for the functioning of Salt. For best results, Halite works with Hydrogen and higher versions.

## Conclusion

The general presentation of Salt is not enough to begin mastering the tool, but it is required if you are not familiar with the concept of configuration management and data center automation.

_________

- Buy it now : http://bitly.com/SaltStackForDevOps
- See more at : http://saltstackfordevops.com/
- Get a free sample : http://bitly.com/1OrL3kv
- SaltStack CheatSheet : https://github.com/eon01/SaltStackCheatSheet

