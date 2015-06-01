TALKS

=====



Part 1

------

Russell Keith-Magee: What on earth are Python & Django?

Russell explains what they are, what you can do you with them and why you might want to - and why programming is much easier and more fun than you probably think.

Simple introduction to what you can achieve with python/django and why you won't come back to a exel file.



Mark Steadman: A web framework for the creative mind

Mark discusses Django from the perspective of a content creator (weblogger, podcaster and in daylight hours a web developer).

@iamsteadman - creator of poddle
idea: django helps you get more creative

content to explore --> filebrowser, django-social-auth (compared to django-allauth?)
Once hosted, to scale it up, see caching, ansible + digitalOcean (in his case)
find support:

djangonauths.slack.com
code.steadma.io
blog.steadman.io
podcast.poddle.io

The slack website is quite new


Rhiannon Titcomb: Understanding Bezier curves with Python

Rhiannon discusses the mathematics of key computer graphics techniques using Python.
https://github.com/RhiannonT/Bezier-Curves

No django here, but you wan check it out on github. (I made a pull request to help her out, she's a first year math student)



Tom Bakx: Python in Astronomy

Tom discusses the ways astronomers use Python to find and peer into far-away galaxies.

Talks begins with one image from hubble. Then show with python processing what we can achieve. 3D Simulation are really beautiful. (But the cake is a lie, they probably have been made with a C or C++ code) but most of the time, he uses python. 
Also talks a little bit of einstein ring if interested.
(Obvious use of cluster to run that code, he said it would take around 2k years to run the code on his own computer)



Part 2

------

Cory Benfield: Security Vulnerabilities - A Story About Panic

Cory tells a tale of every open-source project's worse nightmare: a report of a serious security flaw in the software.

@lukasaoz on twitter - @lukasa on github
maintainer of requests, urllib3 and some other cool projects
Story of a huge bug (security related) in the requests library. The talk is really great and he gives a few advice.

Please, use GPG key
Do not release on week ends, warn downstream distributors when you make a really important security update, define your policy for reporting bug(or still the ones from requests)

slides on: https://speakerdeck.com/lukasa/security-vulnerabilities-a-story-about-panic



Amit Nabarro: RESTful APIs in Django

Amit explains how Django developers can make use of the power of RESTful APIs in their projects.
@amitnabarro
.. use a rest app with django rest framework or tastypie. (avoid piston, unmaintained)
Those projects also rocks with nosql databases
expectations: serialization, pagination, validation auth, authorization, throttling, caching, API discovery, unit testing...




Yamila Moreno: Lessons learned

Yamila discusses two years of making good and bad decisions in a large Django project, and lessons she wishes she didn't have to learn the hard way.

slides on: http://yamila-moreno.github.io/lessons-i-learned-during-a-django-project/#/
Nice talk from this pylady. 10 main tips are below

tips:
- Separate API & front end
- get prepared for any change
- refator & abstraact the second time you have the choice
- 5th law of entropy: sooner or later, you're gonna make a bug --> TEST TEST TEST
- don't reinvent the wheel big community
- know the internals & dont be afraid of usingit
- use a distributed source control manager
- use PR as a basis in your workflow
- DocumentationS. One for the API, one internal
Documentation driven development. (wow... In fact, during the Q/A session, she admits it's a lot easier to say...)
- Opensource make as much as you can



Raphaël Barrois: Cyberponies - Django talks to machines [French guy]

Raphaël discusses Django's suitability for building systems that interface with thousands of remote machines, as part of an Internet of Things.

http://slides.xelnor.net/2015/djangocon_eu/cyberponies/#slide1

Workflow: 
1 - CRUD on devices
2 - Monitor, record events/updates, detect issues
3 - aggregate info, transformuser requests into commands
(use of django-reversion)


to scale, just add more server while your bdd can handle the charge.
if too much data, may use elastic search

ou will lose messages at some points, don't panic, it will happen all the time

tips: send full state, keeps datetime of previous change for boolean, keep last know version of object

challenge: split brain effect. We sometimes lack information and/or the system lack informations. Sensors could also be broken etc...

Q/A: how to tests? Good questions, really hard, but try to fake everything and everyevent in integration tests.
Use of websocket? It would require more bandwidth...




Part 3

------





14.00 Adrienne Lowe: Coding with knives

Adrienne describes what it's like for a professional chef to become a programmer - and why cooking and coding are not that different.

The talk is really nice but it is more the journey of discovering django and coming from a non technical background than a tech talk.



Árni St. Sigurðsson: Data-driven democracy

Árni discusses a mission using Django data-gathering tools to help the electorate in Iceland make better-informed decisions.
Well.. The technical part of the talk was almost inexistant. It is most a talk about how we could use data for politics and decision making in politics/democracy.
[I had trouble understanding this guy accent] 




Žan Anderle: Mistakes and lessons in developing user experience
Žan discusses how any development team can improve the user experience of their applications.

works at datafy.it
twitter @z_anderle

mistakes he learned from through UX:
- forgetting about UX because of lack of resources
- forgetting about the user
- lack of communication between team (in the company itself) --> include dev in the support
- overcomplicating apps --> simplify the app!! Show less feature (unless you're paid for it)
- Use technical language, use plain english in your app
- not listenning to the users
- fail to adapt basic principles (consistency & feedback)

TL;DR take care of the UX




Alasdair Nicol: Ponies and moustaches, or Templates in Django
@al_sdair
Alasdair introduces one of Django's notable new features, its support for multiple template engines, and explains why it matters (and what moustaches are).

We can modift database, sessions, caching, what about templating? Well, with django 1.8, we can have fun with the template engine.
But, warning guyz, the interest might be limited.
Jinja2 has been integrated after a campaign launched by Aymeric Augustin. 

In the book 2 scoops of django, you can find one chapter about templating.
See his github --> github.com/alasdairnicol/django-moustache
moustache implementation for django 



Part 4

------



Christopher Hunt: Arduino sensors, mobile apps and virtual reality

Christopher explores how Django can integrate with all sorts of physical devices to capture, transmit, store, visualise and derive intelligence from data.

@thisischrist

if the talk was interesting, (the guy good orator), i did not take any interesting note.





16.20 Katharine Jarmul: Data wrangling with Python

Katharine offers a whirlwind introduction to the Python tools that will help get wild and unruly data under control.

@kjam

analyse something with data, some tools: scipy, numpy, pandas
data --> OpenDta: http://data.gov.uk
other tools: xlrd (write read xl), gspread (for google spreadsheet without using the google spreadsheet API), pdfminer

github.com/pudo/dataset for an introduction to databases
To interact with a webpage: selenium or Ghost.py (to interact with browser)
take a really simple look on a page (lxml)
scrapping: scrappy, others.....

vizualiaztion : bokeh, matplotlib, pygal

see nltk (natural language toolkit), match word for fatfinger: https://github.com/seatgeek/fuzzywuzzy (helpful!)






Rivo Laks: Django and the real-time web

Rivo discusses the rise of the real-time web, and some tools and techniques to help put it into practice.

django is 10yo

in 2005, mobile web wasnt there and yet, django is still pretty reliable

Getting started:
PUbSub publish and subscribe pattern.
pusher -->Create a client to send push message
THen we need to receive on the client side those data
Message from client --> ajax

Websocket (2 ways connection)
support txt and binary data

django & websocket
asyncio (py3.3) and websockets library
custom server process
Client side
pure js or sawkit-client (see github)

Demo: http://djangocon.thorgate.eu
https://github.com/rivol/djangocon-realtime

new standard  by mozilla team: webpush, implementation in go and py3
also, django + websockets --> check out swarmdragon




17.00 Jamie Hannaford: Making our spaces more inclusive

Jamie discusses the social issues of an industry where dealing with code is easy, but dealing with people can be very hard.

That talk was really really good about the importance of diversity and how we should act to helps it become the standard. It is 0% technical but 100% interesting.

1 - workplace
diversity in the workplace
we know the techniques
2 - open source more inclusive for everybody
3 - conferences

Why diversity?
"The more diverse your team, the greater the potential for innovation"

Job posting remove hero ninja etc... make diversity commitment explicit
offer benefits people actually want (acces handicapé etc..°)

"Whiteboard coding interviews cfreate an inerently confrontational situation in which the candidate has to prove that they are intelligent
Let's build things together rather thn prove me how smart you are"

job performance and technical interview performance has 0 relation (google proved that)

Fear: fear of asking questions
fear of being a beginner
asking can be hard,  so don't stigmatise
Be empathetic, understanding, kind
No feigning surprise, No "well actually" answers

Praise in public, critique in private
Why don't people more people contribute to open-source?
People tend to focus only on code but you have docs tests, design etc

documentation is the heart of any project

how to tackle exclusion at events?
change the way we hire, move the fear, open source, 
support event diversity attetnd

slides: htttp://bit.ly/1LUJ440
@jamiehannaford
