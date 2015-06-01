Part 1
======

see http://foobacca.github.io/foobacca-event-notes/DjangoConEurope2015/index.html for a sum up of each talk

Baptiste Mispelon: Baptiste's adventures in Djangoland
------------------------------------------------------
Our keynote speaker describes how he tackled burnout by travelling around Europe, eating Welsh cakes, pierogi and stroopwafel.

@bmispelon
Basically just the story of the guy. Really really nice. He got a standing ovation.
http://reinout.vanrees.org/weblog/2015/06/01/01-adventures-djangoland.html
slides: https://speakerdeck.com/bmispelon/baptistes-adventures-in-djangoland



Hanna Kollo: Avoiding monoliths
-------------------------------
Hanna explains how to take advantage of Django's flexibility to build modular systems, when working with large projects with ever-changing requirements.
github - spil-hanna
woks at spilgames gamesgames.com


aviod monolith apps --> one project with one app
their story: 
they started with many many apps with a few models
second iteration: started with one app and then added more apps.

--> fewer apps with more models in each of them
where to put business logic?
Not everything can go to models. They chose the service layer
--> all the logic is is in services.
Really interessting
see: http://reinout.vanrees.org/weblog/2015/06/01/02-avoiding-monoliths.html
slides :http://harbour77.eu/?p=86



Abdulrahman Alotaibi: Injecting Django into the work environment
----------------------------------------------------------------
Abdulrahman discusses what makes users willing to switch from one framework or language to another.
He hesitated between django & rails
that conf made his choice clear https://youtu.be/cb9KDt9aXc8  python and rubies
notes: http://reinout.vanrees.org/weblog/2015/06/01/03-work-environment.html
slides on adminq80.github.io
History of him introducing django in Kuwait.



Ola Sitarska: Pushing the pony’s boundaries
-------------------------------------------
Ola is a Django core developer and has spent five years pushing Django's admin to its limits. She'll discuss some of the things you can do, and some you really should try, with this amazing toolbox.

DJANGO-FLAT-THEME



Dafydd Evans: CAMEL, the Cardiff Maths e-learning project
---------------------------------------------------------
Dafydd introduces a new virtual learning environment aimed at mathematicians.

Use django-mptt to mimic latex in a full web way. Neat!



Lucie Daeye: Reaching out - Django in the social sciences
---------------------------------------------------------
Lucie first encountered Django in 2014; a few months later she was using it in her doctoral studies to manage and map social sciences research data.
@patjouk


Yann Malet: Salt for django developers
--------------------------------------
Yann overviews Salt and describe some of its unique features. By the end of the talk, you should be able to dive in and start writing your own Salt states and working with existing ones.
@yml on github
@gwadeloop

Quick intro on salt.




Mathieu Agopian: Switching from nose to py.test at Mozilla
-----------------------------------------------------------
Mathieu talks about the move between two testing frameworks for a large code base.



Erik Romijn: A sincere tale of Django, developers and security
--------------------------------------------------------------
Erik discusses ways to understand security better, making it intrinsic to our work, issues common to Django websites and why it matters so much.
https://speakerdeck.com/erik/a-sincere-tale-of-django-developers-and-security

nothing new, ponycheckup, some guidelines. See slides but nothing incredible

Check password strength: github.com/dropbox/zxcvbn


Maik Hoepfel: On privilege and moral duty
-----------------------------------------
Maik Hoepfel raises questions about the privileges and freedoms many of us in the software industry enjoy, and considers what duties follow from them.

superpowers:
our impact on the world in enormous




Lightning talks
---------------
Five-minute talks on any subject.
See notes from  http://foobacca.github.io/foobacca-event-notes/DjangoConEurope2015/index.html

