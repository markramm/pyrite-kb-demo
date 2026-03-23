---
id: java-the-microsoft-perspective
title: Java - The Microsoft Perspective
type: writing
writing_type: rre-post
date: 1997-10-16
url: http://commons.somewhere.com:80/rre/1997/Java.-.The.Microsoft.Per.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - administrative
  - auto-imported
  - commerce
  - education
  - forwarded-content
  - internet-policy
  - labor
  - law
  - libraries
  - military
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/Java.-.The.Microsoft.Per.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991002105944/http://www.somewhere.com/)

  

# Java - The Microsoft Perspective

```
[I feel another outburst about Microsoft coming on, but I'll stifle it
this time and offer you Roger Sessions' analysis instead.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Sent: 	Thursday, October 16, 1997 12:36 PM
From: 	Roger Sessions[SMTP:roger@objectwatch.com]
To: 	SubscriptionList
Subject: 	ObjectWatch Newsletter # 7

---

ObjectWatch Newsletter Number 7
Focus on Distributed Object Technology

---

To be added to or removed from this subscription list, send mail to 
sub@objectwatch.com <mailto:sub@objectwatch.com> 

---

Main Story: Java - The Microsoft Perspective

---

JAVA - THE MICROSOFT PERSPECTIVE

Within the last week, I have heard that Microsoft
a) is trying to take over Java
b) is trying to hide from Java
c) deserves to be sued by Sun for crimes against humanity
d) should be revered among mortals for its weighty accomplishments

and last but not least, the humble, but ever so popular

e) loves Java
f) hates Java

I have spent much of the last year researching Microsoft's position on 
Java. I needed to understand this issue for my new book (COM and DCOM; 
Microsoft's Vision for Distributed Objects). I have read every memo, 
news release, and white paper I could find on this topic. I have spoken 
to many of Microsoft's Java team. For better or worse, I seem to have 
become the leading expert on What Microsoft Thinks of Java. In fact, 
based on some of my recent discussions, I suspect I understand this 
issue better than most people who work at Microsoft.

But before I can get into Microsoft's Java perspective, I need to give 
you some background. First, I need to give you some historical 
perspective on where Java is coming from. Second, I need to do some 
level setting on what Java is about technically. Third, I need to tell 
you what Microsoft is trying to accomplish over the next five years. 
Within this background, we will be able to discuss what Microsoft really 
thinks about Java.

JAVA HISTORY
Lets start with the history of Java. Java was introduced by Sun. Many 
companies jumped on the Java bandwagon. The most notable of these early 
adopters was IBM.

What fueled this odd alliance between Sun and IBM? The incredible 
superiority of Java as a programming technology? Unlikely. Remember, 
this alliance was formed back when Java had the most minimal of 
capabilities and was hardly more than a toy.

We can get some insight into the purpose of this alliance by looking at 
the last time these two companies joined together to lead a major 
industry effort. This last collaboration resulted in the distributed 
object technology known as CORBA, produced by an industry consortium 
called the Object Management Group (OMG).

I was very involved in the OMG. I worked for IBM at the time, and I was 
a lead architect for one of the CORBA services. I wrote my last book on 
this topic (Object Persistence; Beyond Object-Oriented Databases).

The OMG consortium was held together by one common purpose: to stop 
Microsoft. The OMG failed in this effort, and is now limping along with 
only a few companies making even a minimal profit on CORBA technologies.

Many people accuse Microsoft of meeting any technological threat with an 
embrace and smother strategy. This is certainly not true of Microsoft's 
reaction to CORBA. Despite the millions of dollars that IBM, Sun, and 
others were spending on CORBA, Microsoft never took CORBA seriously. 
Microsoft joined the OMG, and occasionally sent a representative to OMG 
meetings, but looked on the whole affair with an air of amusement, as if 
it was watching children at play. 

By 1994, it was clear to Sun and IBM (and later Netscape and the rest of 
the industry) that OMG was not going to be the knight in shining armor 
that would protect them from the Microsoft dragon. So they started 
looking for a new protector. And they thought they found it in Java. 
Soon most of the industry had jumped on the Love-Java/Stop-Microsoft 
bandwagon.

JAVA TECHNOLOGY
Why did the industry think Java would stop Microsoft? For that matter, 
what exactly was the industry trying to stop Microsoft from doing?

Sun and IBM in particular saw the whole world moving into the direction 
of Microsoft operating systems. IBM had been humiliated in its attempt 
to have OS/2 taken seriously. Sun was dependent on the success of its 
Solaris flavor of Unix. 

But the operating system vendors were in a bad position. By 1995, most 
of the world's computer's were running some version of Windows. Nobody 
was going to write new software for anything other than Windows. 

In Java, the industry thought it had a mechanism to write software than 
would run on any operating system. For operating system vendors, this 
would be great. Suddenly it wouldn't matter if they only owned a sliver 
of the operating system market, they could still offer software vendors 
a viable market. So Sun and IBM led the charge to creat write-once/run-
everywhere (WO/RE) software using Java.

Java promised a WO/RE solution through a combination of tried and true 
technologies. These included a language specification, a pseudo-
compiler, a virtual machine, and a series of libraries. These libraries 
were to be available on all Java platforms and were to define the 
"official" WO/RE Java API. These libraries are basic to WO/RE and 
according to Sun and IBM, WO/RE is basic to Java.

Java is not the first time the industry has been promised a WO/RE 
solution. In fact, this has been a recurrent theme since the dawn of 
software. Unix, CORBA, and C++ are just a few examples of the many 
products that originally made similar claims. 

George Santayana said, "Those who cannot remember the past are condemned 
to repeat it." Unfortunately, the collective memory of our industry 
seems particularly poor. WO/RE has never worked and it seems unlikely to 
me that it ever will. And we appear to be caught in an endless cycle of 
relearning this lesson.

The WO/RE dream faces a technological dilemma. Users, spoiled group that 
they are, have come to expect a high quality interactive experience and 
rich functionality. Software can only meet these expectations by taking 
every possible advantage of underlying operating system services. But 
software that takes advantage of underlying operating system services 
will not run everywhere. Software that really runs everywhere can only 
use technology that exists everywhere. Services that are universally 
available are going to be universally bland. Software built on such 
bland services can only end up as the McDonalds of software: offending 
nobody but impressing nobody.

While software vendors care that their products run everywhere, their 
users don't. A user cares only that a product runs well on one 
particular machine, the one at which the user is working. A product 
written for generic services will never be able to compete for that 
user's heart against a product written especially for that user's 
operating system.

Although the failure of WO/RE was predictable, many software vendors 
couldn't resist the lure. They worked hard to write products using only 
Java and the WO/RE libraries. These vendors have all learned their 
lessons the hard way. To the best of my knowledge, there isn't a major 
software vendor left still developing a commercial product based on the 
WO/RE capability of the Java libraries.

But the fact that WO/RE doesn't work doesn't mean that Java should be 
abandoned. We don't want to throw out the baby with the bath water. Java 
is still a great language, much better than C++. The problem is not in 
the language, but in the WO/RE libraries. Even then, the real problem is 
not so much the libraries themselves, but the edict that these libraries 
constitute the entire range of Java programming possibilities.

MICROSOFT GOALS
Microsoft's goal for the next five years is simple. It wants NT to be 
the platform of choice for doing distributed commerce applications. This 
basically sets the stage for a new war, and the battleground is the 
three-tier architecture.

Microsoft believes that the three-tier architecture will form the basis 
for distributed commerce. Three-tier architectures define a client tier, 
a component tier, and a data tier. The client tier has long been owned 
by Microsoft. Microsoft is now going after the component tier with a 
vengeance and is preparing to undergo a battle of attrition for the data 
tier.

Microsoft has defined an architecture that supports distributed 
applications based on components. A component is a package of software 
that can do specific, well defined tasks. Components can communicate 
with other components, and this communication can occur within a tier or 
across tiers.

Microsoft wants to be in the three-tier component plumbing business. It 
wants to provide the operating systems on which three-tier component 
based software systems will run. Microsoft will happily support any 
products that fit within this vision, and will not support those that do 
not. The most important pieces of Microsoft's plumbing are COM, DCOM, 
and MTS. These will all eventually be merged into COM+.

THE MICROSOFT POSITION ON JAVA
Now that we have looked at Java's history, Java's technology, and 
Microsoft's technical agenda, we can better understand Microsoft's 
position on Java.

It would be logical to assume that Microsoft hates Java. After all, Java 
was charged from its birth with the task of bringing Microsoft to its 
knees. And this was, in fact, Microsoft's original position on Java. 

But then two things happen to cause Microsoft to rethink this position. 
First, the cadre of highly intelligent and incessantly curious Microsoft 
engineers discovered how much easier it was to work with Java than with 
C or C++. Second, Microsoft discovered that Java is an ideal language 
for implementing the kind of components on which it had based its whole 
corporate strategy.

So Microsoft did an about-face, and threw its full strength behind Java 
the language. I see no evidence that this support has slacked off in the 
slightest. Microsoft seems fully committed to providing the best tools 
available for creating components using Java. Although Microsoft will 
always support other component development languages, I believe Java is 
Microsoft's language of choice for implementing the software that will 
run on the component tier.

But then there is the issue of the Java Write-Once/Run-Everywhere 
libraries. Here Microsoft diverges from the rest of the Java community, 
and in particular, from Sun.

Some of these WO/RE libraries are intended to support user interfaces. 
Microsoft has much better tools for building the software that will run 
on the client tier than Java. Some of these tools, such as DHTML, are 
even going to be available for non-Microsoft platforms. I agree with 
Microsoft that Java is an inferior technology for user interfaces.

Some of these WO/RE libraries are directly competitive with Microsoft's 
architecture. Java's Remote Method Invocation (RMI) capability, for 
example, allows Java objects to communicate across process boundaries. 
Microsoft sees this as competing with DCOM. In my opinion, RMI is not 
even in the same league as COM/DCOM/MTS, and doesn't begin to address 
important issues like language independence, object pooling, security, 
and transactional support. But those WO/RE libraries that Microsoft 
views, rightly or wrongly, as competing with its own architecture are 
going to get lukewarm support, at best.

Microsoft believes the COM/DCOM/MTS architecture is an advanced 
component runtime environment, and Java components should be allowed to 
take full advantage of everything this environment offers. Obviously 
components that do take advantage of this environment are not going to 
work in a non-COM/DCOM/MTS environment. But, the reasoning goes, do you 
want full featured components that work well in the environment for 
which they are intended, or insipid components that will run on any 
toaster that happens to have a microchip with an embedded Java virtual 
machine?

Microsoft does not support the WO/RE philosophy. If you are jaded, you 
might argue WO/RE is in conflict with Microsoft's self interest. But I 
believe WO/RE is a fantasy outside of the trivial world of browser 
applets. The Java WO/RE libraries today don't come even close to 
providing the rich infrastructure needed by distributed commerce 
applications. 

Part of the current legal dispute between Sun and Microsoft has to do 
with vision and part has to do with control. 

Sun's vision for Java is much different than Microsoft's. Sun sees Java 
as a complete object milieu, providing a total API package for 
everything from user interface to communications to database access. 
Microsoft sees Java as a good language for developing components that 
live on one of the three tiers, specifically, the component tier. It 
does not believe that programmers should be forced to use Java on the 
other tiers where Java is basically inferior technology just because 
they are using it on the component tier. And it does not believe that 
Java programmers should be forced to program in a medieval runtime 
environment as the price for using the language.

Sun seems to be saying that Microsoft wants to take control of Java. I 
find this argument unconvincing. I hear Microsoft saying that nobody 
should control Java. Different companies should be able to improve Java 
as they see fit. An open and free market is the appropriate forum to 
decide on the future of Java, not law courts and corporate cartels. 
Programmers who want a WO/RE environment should be free to choose WO/RE 
implementations. Programmers who want to do heavy duty commerce 
applications should be free to choose industrial strength 
implementations and runtime environments. If any company is trying to 
control Java, it is obvious to me that that company is Sun, not 
Microsoft.

In my studying of the Microsoft distributed component architecture, 
including Java, COM, DCOM, MTS, Falcon, and Wolfpack, I have found that 
Microsoft consistently provides open frameworks that encourage the 
participation of third parties, even when those third parties are 
selling products that directly compete with Microsoft. In some cases 
Microsoft doesn't even wait for its competitors to plug into the 
Microsoft frameworks, Microsoft writes the plugs for them! Does this 
sound like the stance of a company that is afraid to compete?

So I think we can summarize Microsoft's position on Java very simply. It 
fully supports and really likes Java the language. It is committed to 
providing competitive tools for developing Java components to run on the 
component tier. As far as the libraries and Java run-time environment, 
it says let each company provide the best underlying support for Java 
that it can, and may the best architecture win.

- Roger Sessions, October 16, 1997

---

Roger Sessions is the author of COM and DCOM; Microsoft's Vision for 
Distributed Objects, published by John Wiley. World wide availability 
will be November 1997.

ObjectWatch, Inc., offers a one day overview of the Microsoft 
Distributed Component Architecture, including COM, DCOM, MTS, Falcon, 
and Wolfpack. It is taught by Roger Sessions, author of four books and 
dozens of articles and a frequent conference speaker. Visit our web page 
at http://www.objectwatch.com <http://www.objectwatch.com>  or contact Roger
Sessions at 
roger@objectwatch.com <mailto:roger@objectwatch.com> 

---

Recent issues of this newsletter are available at 
http://www.objectwatch.com <http://www.objectwatch.com> 
# 6: Letter From the Microsoft Professional Developer's Conference
# 5: The World's Largest Software Company

---

Legal Notices:

The ObjectWatch newsletter does not accept advertising or rent out its 
subscription list.

This newsletter is copyright by ObjectWatch, Inc., Austin, Texas. It may 
be freely redistributed provided that it is redistributed in its 
entirety and that absolutely no changes are made in any way.

ObjectWatch is a registered trademark of ObjectWatch, Inc., Austin, 
Texas. All other trademarks are owned by their respective companies.

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991002105944/http://www.somewhere.com/)