---
id: suit-against-spammer
title: suit against spammer
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/1998/suit.against.spammer.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1998/suit.against.spammer.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008104054/http://www.somewhere.com/)

  

# suit against spammer

```
[The editors of TidBITS report having filed a lawsuit against WorldTouch
Network, perhaps the worst spammers on the Internet.  I personally have
received well over a hundred identical messages from them, from at least
half that many distinct domains.  If I understand their headers correctly,
they have a program that systematically searches the Internet host tables
for hosts whose mailers that can be hijacked to send spam, and they then
automatically send out innumerable copies of their message from each one.
Lately they appear to have been working their way through the host tables
of several small European countries.  I make it a practice to report the
problem to the postmasters of every single one of these hosts, and have
encountered many poor (poor as in, they have no food) sysadmins in places
like Poland who absolutely cannot afford to have their systems overrun in
this way.  The TidBITS editors now allege that WorldTouch Network's spam
violates the new law in Washington State that creates a cause of action
(i.e., you as the recipient can file a lawsuit and receive damages) for
messages with falsified headers.  At least one person has collected actual
money from a spammer in an out-of-court settlement under this law, which
is preferable to the Spam Legitimation Act (aka the Murkowski bill, whose
text I sent to this list when it was first introduced) that recently
passed the US Senate with support from spammers and corporate lobbying
groups.  I have enclosed the entire issue of TidBITS that contains the
article about the spam suit in case you find the publication useful.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Mon, 20 Jul 1998 22:02:27 -0700
From: TidBITS Editors <editors@tidbits.com>
To: editors@tidbits.com (TidBITS Distribution)
Subject: TidBITS#439/20-Jul-98

TidBITS#439/20-Jul-98

---

  Ever wanted to sue a spammer? We're doing it - read on for our
  announcement of how we're testing Washington State's new anti-spam
  laws on a prolific spammer. Also, Adam starts a two-part review of
  crash detection devices that keep servers running and
  editorializes about Symantec ignoring Visual Page for the Mac.
  News this week includes Apple's third quarter profit, a patch for
  the much-publicized OLE bug, RAM Doubler 8, a security fix for
  NetCloak, and more.

Topics:
    MailBITS/20-Jul-98
    TidBITS Sues Spammer
    Closing the Book on Visual Page
    The Battle of the Bouncers, Part 1

<http://www.tidbits.com/tb-issues/TidBITS-439.html>
<ftp://ftp.tidbits.com/pub/tidbits/issues/1998/TidBITS#439_20-Jul-98.etx>

Copyright 1998 TidBITS Electronic Publishing. All rights reserved.
   Information: <info@tidbits.com> Comments: <editors@tidbits.com>
   ---------------------------------------------------------------

This issue of TidBITS sponsored in part by:- APS Technologies -- 800/443-4199 -- <sales@apstech.com> -- How
     do you back up your APS hard disks? Try APS tape, removable,
     magneto-optical, and CD-R drives! <http://www.apstech.com/>- Northwest Nexus -- 1 888-NWNEXUS -- <http://www.nwnexus.com/>
       Internet business solutions throughout the Pacific Northwest.- Small Dog Electronics -- Special Deal for TidBITS Readers!
         LaserWriter 12/640 (refurbished), new toner, AppleCare: $979!
         UMAX C500/240 (refurbished) with new 14-inch KDS monitor: $779
         For details: <http://www.smalldog.com/> -- 802/496-7171- Cyberian Outpost -- the Cool Place to Shop for Computer Stuff! <- NEW!
           Tired of waiting for Norton? Buy TechTool Pro 2.0 for $89.95
           Order online or call 860/927-2050 x228
           <http://www.tidbits.com/tbp/tech-tool-pro.html>- TERRY MORSE MYRMIDON
             Turns any Mac file into a Web page with one click!
             See Terry outshine Microsoft's and Adobe's own converters.
             --> The proof: <http://www.terrymorse.com/comparisons.html> <--
             ---------------------------------------------------------------

          MailBITS/20-Jul-98

          ---

          **Apple Racks Up $101 Million Profit** -- Apple Computer last week
            announced a profit of $101 million for the third fiscal quarter of
            1998, although bolstered by $26 million in one-time investment
            gains. $101 million works out to $.65 per share, almost double
            analysts' estimates of $.33 per share. Revenues for the quarter
            equaled last quarter at $1.4 billion, gross margins were 25.7
            percent (the highest in three years, thanks to the Power Macintosh
            G3s and PowerBook G3s), and Apple CFO Fred Anderson said that
            company has almost $2 billion in cash on hand. Anderson also noted
            that the introduction of the low-margin iMac in the next fiscal
            quarter will drive down gross margins but should increase
            revenues. [ACE]

          <http://www.apple.com/pr/library/1998/jul/15results.html>

          **OLE Security Patch for Mac Office 98** -- Microsoft Corporation
            has released an OLE update for English language versions of
            Microsoft Office 98 designed to prevent OLE applications from
            storing extraneous data - possibly including email, financial
            data, or other sensitive information - within document files. (See
            "Oil of OLE: Document Security and You" in TidBITS-437 for a
            complete description of the problem.) Although the revised version
            of OLE corrects the extraneous data problem for all applications
            that use OLE (including PageMaker and previous versions of Office
            applications), Microsoft's updater requires the Microsoft Office
            First Run application to install the files. As a result, unless
            you have Microsoft Office 98, this updater apparently cannot be
            used to install the revised version of OLE for use with other
            applications. At this point, it's unknown whether Microsoft plans
            to release a stand-alone update to OLE, or make the fix available
            to other application developers who use OLE. The update is
            available in MacBinary (3.3 MB) or BinHex (4.5 MB) formats, and it
            also includes a previously released fix for Visual Basic for
            Applications that corrected a problem with the Office 98's Memo
            and Resume Wizards. [GD]

          <http://www.microsoft.com/macoffice/productinfo/98dl/offi98patch.htm>
          <http://db.tidbits.com/getbits.acgi?tbart=04973>

          **Free RAM Doubler 8 Update** -- Users of Connectix's RAM Doubler
            2.x can now update to RAM Doubler 8 using a free updater (379K
            download) available from Connectix's Web site. Despite the large
            version number change, the update is fairly minor, offering
            primarily some additional reporting and configuration options in
            the RAM Doubler control panel, plus a fix for a conflict with
            Microsoft Office 98 (see "Minor Connectix Updates" in
            TidBITS-431). [ACE]

          <http://www.connectix.com/html/rd__mac__update.html>
          <http://db.tidbits.com/getbits.acgi?tbart=04902>

          **Maxum Moves to Plug NetCloak Security Hole** -- Maxum
            Development has released an interim "final candidate" version of
            NetCloak 2.5.4, its server-side tool for creating dynamic Web
            content. Version 2.5.4 fixes a serious security problem in
            previous versions of NetCloak, and Maxum recommends that all
            NetCloak users with secure content on their Web servers upgrade to
            version 2.5.4 as soon as possible. Maxum is not identifying the
            security problem in order to prevent hackers from using it against
            sites that haven't installed the 2.5.4 update, and Maxum expects
            to release a fully tested release version of NetCloak 2.5.4
            shortly. The update can be obtained by filling out a form at
            Maxum's Web site. [GD]

          <http://www.maxum.com/NetCloak/>
          <http://www.chi.maxum.com/Misc/DemoAccess.html>

          **Griffin iMates USB and ADB** -- Griffin Technology last week
            announced the iMate, a $29 USB-to-ADB adapter that enables iMac
            users to use standard ADB devices such as keyboards, mice,
            trackballs, and joysticks. Plans for a future version include
            support for less standard ADB devices such as copy-protection
            dongles. iMate users will be able to mix and match USB and ADB
            devices, and ADB devices attached to an iMate can be daisy
            chained. Reportedly, the iMate also enables USB-equipped PCs
            running Windows 98 to use ADB devices. Griffin plans to ship the
            iMate in mid-August, to correspond with the iMac release date.
            [ACE]

          <http://www.nashville.net/~griffin/usb_pr.html>

          **Keep It Up More Often** -- Karl Pottie has released Keep It Up
            1.4.1, a minor bug fix for his useful application monitoring
            utility. Keep It Up watches selected applications and relaunches
            them if they quit or crash. After a user-specified number of
            attempts to relaunch an application, Keep It Up can restart the
            Mac. Other features include the capability to open specified
            documents on application launch, perform scheduled restarts, and
            keep one application frontmost at all times. Keep It Up is $22
            shareware and is a 186K download. [ACE]

          <http://www.vl-brabant.be/mac/kiu.html>

          **AutoShare 2.4 Released** -- Mikael Hansen has released AutoShare
            2.4, his freeware mailing list server and auto-responder. New in
            version 2.4 are several additional process extender types, a
            sample process extender for vacation mail, enhancements to the
            automatic bounce processing module, plus minor improvements and
            bug fixes. AutoShare 2.4 is a 1.8 MB download. [ACE]

          <http://www.dnai.com/~meh/autoshare/>

          **Tenon Revs Up WebTen 2.1** -- Last week, Tenon Intersystems
            released WebTen 2.1, a high-performance, Apache-based, Macintosh
            Web server, which also includes DNS, multihoming FTP, NFS, and SSL
            3.0. WebTen is based on Tenon technology that essentially wraps
            Unix applications in a shell that turns them into Macintosh
            applications while retaining excellent performance and features.
            WebTen 2.1 builds in the latest code for Apache 1.2.6, domain name
            service based on BIND 8.1.2, caching software based on Squid
            1.1.20, Perl 5.004_4, and updated documentation. Tenon also
            announced the availability of a version of the popular Unix
            ht://Dig search engine for WebTen, plus a deal on the automatic
            server monitoring and restart device MacCoach 2.0 from Neuron Data
            Systems. MacCoach 2.0 normally retails for $99, but for a limited
            time is available for WebTen customers from Tenon for $55. Prices
            for WebTen vary from $350 sidegrades to $495 for a CD and printed
            documentation; Tenon also offers educational and government
            discounts. [ACE]

          <http://www.tenon.com/products/webten/>
          <http://www.neuronsys.com/>

          **Disk Copy 6.3 Adds and Improves Features** -- Apple has released
            Disk Copy 6.3, a free program for creating and manipulating disk
            image files, including the New Disk Image Format (NDIF) archives
            that Apple uses for software updates. Disk Copy 6.3 adds the
            capability to duplicate floppy disks and create self-mounting disk
            images (usually identified by an ".smi" extension). In addition,
            Disk Copy 6.3 supports HFS Plus volumes (under Mac OS 8.1) and
            Apple's forthcoming Navigation Services (set to debut in Mac OS
            8.5). Although the feature is often overlooked, Disk Copy offers
            significant AppleScript support, including recordability and an
            attachable Scripts menu; version 6.3 changes some of the
            AppleScript terminology but also offers new functionality. Disk
            Copy requires U.S. English System 7.0.1 or later, although many
            features (such as read/write images and drag & drop support)
            require System 7.5 or higher. Disk Copy 6.3 can be downloaded in
            BinHex (983K) or MacBinary (729K) formats. [GD]

          <ftp://ftphqx.info.apple.com/Apple_Support_Area/Apple_SW_Updates/US/
          Macintosh/Utilities/Disk_Copy/Disk_Copy_6.3.smi.hqx>
          <ftp://ftp.info.apple.com/Apple_Support_Area/Apple_SW_Updates/US/
          Macintosh/Utilities/Disk_Copy/Disk_Copy_6.3.smi.bin>

          **Newer Present at Macworld** -- Oops. We biffed it in
            TidBITS-438 when we said that Newer Technology wasn't present
            at Macworld. In fact, Newer Technology was sharing a booth with
            NewerRAM, which is now owned by Peripheral Enhancements
            Corporation. Eric Dahlinger of Newer Technology noted that Newer
            didn't show off processor upgrade cards at their usual demo-based
            booth this year, which may have caused us and others to miss them.
            Our apologies. [ACE]

          <http://www.newertech.com/>
          <http://www.newerram.com/>

          TidBITS Sues Spammer

          ---

            by Adam C. Engst <ace@tidbits.com>

            On Friday, 17-Jul-98, with the help of long-time TidBITS reader
            and Seattle attorney Brady Johnson, the four TidBITS editors
            living in Washington State filed suit against WorldTouch Network
            for numerous violations of Washington State's new anti-spam law
            (see "Washington State Outlaws Spam" in TidBITS-422). WorldTouch
            sells the Bull's Eye Gold email address collection tool, a $259,
            Windows-based, Web spider program that visits Web pages, following
            links and recording the email addresses it finds. Appropriately
            enough, WorldTouch advertises Bull's Eye Gold by repeatedly
            sending unsolicited email advertisements extolling the program's
            virtues to vast numbers of Internet users. Currently, TidBITS
            staff members have received nearly 100 identical copies of the
            advertisement since 11-Jun-98, the day Washington's law went into
            effect.

          <http://www.fremontlaw.com/>
          <http://db.tidbits.com/getbits.acgi?tbart=04780>

            The Washington anti-spam law prohibits "the sending of commercial
            electronic mail messages that use a third party's Internet domain
            name without the third party's permission, misrepresent the
            message's point of origin, or contain untrue or misleading
            information in the subject line." Messages must be sent from a
            computer located in Washington State or to a resident of
            Washington State, and the law places the burden of determining
            residency on the senders of unsolicited commercial email.

            Examination of the Bull's Eye Gold spam shows that WorldTouch uses
            randomly generated bogus return addresses purporting to originate
            from large Internet service providers run by IBM, MCI, Sprint, or
            AT&T. The spam is generally routed through mail servers in Europe
            and also includes false routing information in an attempt to avoid
            being traced. In almost all cases, the spam contains no actual
            subject line in the message header; instead it includes one in the
            message body where email programs don't recognize it and thus
            won't display it in a mailbox window.

            Although Washington resident Bruce Miller recently collected $200
            from a spammer by threatening to file suit, we believe ours will
            be the first case to test Washington's new law, which in turn is
            one of the country's first anti-spam laws that understands the
            issues involved and provides damages to spam victims. Our goal in
            filing the lawsuit is twofold.

          <http://www.eskimo.com/~brucem/tugpayup.htm>

            First, we hope to prevent WorldTouch Network from continuing to
            send out vast quantities of spam. Informal polls indicate that
            many of our acquaintances have also received Bull's Eye Gold
            advertisements as well, so putting an end this particular spam
            campaign will help numerous people.

            Second, we hope that a successful conclusion to the case will send
            a message to current and future spammers that the act of sending
            unsolicited commercial email is not only socially unacceptable,
            but also a violation of Washington State law. Plus, if the
            Washington State law proves effective in this and other cases, we
            hope that other states, and eventually other countries, will enact
            similar legislation. From April of 1997 to April of 1998, I
            personally received 2,300 pieces of spam, and from April of 1998
            to the present, over 1,100 pieces, or about 10 per day. Those
            3,400 messages total about 15 MB of disk space and have consumed
            significant quantities of my time.

            We'll write more about the case as it progresses. For more
            information on the suit, including links to the full complaint and
            the text of the Washington State law, visit the Web page we've set
            up at the URL below.

          <http://www.tidbits.com/anti-spam/>

          Closing the Book on Visual Page

          ---

            by Adam C. Engst <ace@tidbits.com>

            Normally in TidBITS we try to be calm and well-reasoned, but every
            now and then, we hear about a move so stupid that it makes our
            stomachs hurt. That's happened recently at Symantec (motto: "If
            you can't beat the competition, buy them and kill their product")
            with their highly regarded HTML authoring tool Visual Page. We've
            written about Visual Page a number of times in TidBITS, and it's
            fared well in all our comparisons of basic HTML authoring tools.

          <http://db.tidbits.com/getbits.acgi?tbtxt=Symantec%20Visual%20Page>

            Visual Page was a perfect middle ground between a text-based HTML
            editor like BBEdit and the high-end as represented by GoLive
            CyberStudio, Macromedia Dreamweaver, or NetObjects Fusion. The
            fact is, most people would probably prefer not to learn the
            details of HTML, nor do most people need the burgeoning feature
            sets offered by high-end programs.

            Add to this the fact that Adobe seems to be ignoring the Mac with
            PageMill 3.0 (currently available only for Windows) and that Home
            Page has disappeared into the gaping maw of FileMaker, and you
            come up with a situation where Symantec was, as it has been said,
            faced with insurmountable opportunities.

            When faced with such a loss of competition, would you immediately
            decide to refrain from additional Macintosh development? I didn't
            think so. However, the official word, as relayed on Symantec's
            support newsgroup by Scott Morrison, Lead Technician for Internet
            Tools Technical Support, is "We have no plans for any future
            upgrades to this product." Of course, the Windows version of
            Visual Page 2.0 just shipped, where it will have to do battle with
            Microsoft FrontPage, which is bundled with everything short of
            breakfast cereal.

            Scott Morrison, by the way, does deserve a golden apple for his
            work in Symantec's newsgroups. He was unfailingly honest about the
            situation, managed to remain polite while replying to irate Visual
            Page fans, and even offered the professional courtesy of
            recommending that people check out GoLive CyberStudio, which now
            has a Personal Edition that Visual Page owners can pick up for
            free (see "GoLive CyberStudio Gets Personal" in TidBITS-433).

          <http://www.golive.com/>
          <http://db.tidbits.com/getbits.acgi?tbart=04922>

            Our colleague Neil Robertson, a professional Web designer at
            Phinney Bischoff Design House and a frequent speaker at Web design
            conferences, seconded the pointer to CyberStudio. "I was already
            seriously looking at GoLive Cyberstudio since Symantec was taking
            so long to upgrade Visual Page, so it now looks like Symantec has
            lost my business and any future recommendations I might have
            made."

          <http://www.pbdh.com/>

            When I asked Scott Morrison if there was anything Visual Page
            users could do, he encouraged people to leave messages in the
            Symantec technical support newsgroup, where he plans to collect
            them for presentation to upper management. So, if you're a Visual
            Page user, check out the Web interface to the Symantec newsgroups
            and offer your opinion. Make sure to include quantifiable numbers,
            such as the number of copies your organization owns, the number of
            copies you caused to be bought, and the number of Macs for which
            you're responsible. And if you're an individual user, your
            opinions count as well, perhaps even more so than before with
            Apple's renewed focus on the consumer market with the iMac.

          <http://service.symantec.com/cgi-bin/newsgroups.pl?count=50&sortby=
          BYSUBJECTA&group=symantec.support.devtools.mac.visualpage.announce&
          Submit=Browse>

            I think what tweaks me off the most about this entire situation is
            that all these programs originated on the Mac, starting with
            PageMill. They came from small start-ups inhaled by larger
            companies, who have either let the products languish or refocused
            their entire attention on the Windows world. Companies that have
            remained independent and focused on the Mac, such as GoLive
            Systems and Bare Bones Software, seem to be doing fine, so I don't
            believe the market has changed all that much.

          <http://www.barebones.com/>

            I think we're staring into the twisted visage of corporate greed
            here. Sure, the Mac market isn't as large as the Windows market,
            but as has been pointed out ad infinitum, Mac users buy more
            software and tend to be more brand loyal (even considering the
            Apple soap opera of 1997). Loyalty would seem to be a concept lost
            on companies like Symantec, Adobe, and FileMaker, and as long as
            they don't get it, I see no reason they deserve any loyalty from
            the user community.

          The Battle of the Bouncers, Part 1

          ---

            by Adam C. Engst <ace@tidbits.com>

            I run a number of Macintosh-based Internet servers, and for the
            most part, these servers are stable. Crashes aren't frequent, but
            they do happen often enough to be a nuisance, particularly on Web
            servers that need to run all the time. Worse, several of my
            servers are a 45-minute drive away, in an office building I can't
            access after business hours. The laws of the universe state that
            crashes tend to happen on Friday evenings so that the server can
            be unavailable for as long as possible.

            In part, I work around the laws of the universe by using crash-
            detection devices that can watch for crashes and restart a hung
            Mac without human interference. These devices connect to the ADB
            port (and sometimes the power outlet) and communicate with special
            software to determine if the Mac is operational. When they
            determine a crash has occurred, they restart the Mac, either by
            turning it off and on again, or by sending a keyboard restart over
            ADB - just as though you had pressed Command-Control-Power.

            The main device I've used over the years to watch for crashes and
            restart Macs automatically is the PowerKey Pro from Sophisticated
            Circuits. A pair of PowerKey Pros watch our main servers in
            Seattle, and a third kept an eye on our internal file server until
            recently, when the time came to test several newcomers. On our
            internal file server, I installed the new crash-detection device
            from Sophisticated Circuits called Rebound. On our SE/30-based
            mailing list host I installed a crash-detection peripheral from
            Kernel Productions, called Lazarus. I never received another
            competitor, MacCoach from the Belgian company Neuron Data Systems,
            but I'll try to include information about it when possible.

          <http://www.sophisticated.com/products/powerkey.html>
          <http://www.sophisticated.com/products/rebound.html>
          <http://www.kernel.com/kernel/lazarus.html>
          <http://www.neuronsys.com/Products/>

            Although I've found ways all that these devices can be fooled into
            restarting a Mac that hasn't crashed, the most important fact is
            that none have so far failed to restart a crashed Mac. That said,
            how do these products compare?

          *Hardware* -- The PowerKey Pro comes in two different models,
            the 200 and the 600. The two units are physically similar, each
            offering six power outlets, a telephone jack, and an ADB plug. The
            200 lacks the phone tone control and manual switches of the 600,
            but the 200 has 160 Joules of surge protection, whereas the 600
            can take an add-on surge protector. (Omitting surge protection
            from the PowerKey Pro 600 is intentional, since people who buy the
            PowerKey Pro 600 also often have a UPS - uninterruptible power
            supply - and many UPS manufacturers don't recommend plugging surge
            protectors into a UPS.) The important feature for monitoring
            servers comes with the software, an optional $39.95 component
            called the Server Restart Option (SRO) that's currently bundled
            with the 600. Because the PowerKey Pro offers six power outlets
            and has space for the telephone jack, the ADB port, and its own
            power cord, it's quite a bit larger than the other devices I
            evaluated.

            The PowerKey Pro's telephone jack bears mention. Before the SRO
            became available, we plugged the PowerKey Pro into a telephone
            line and created events that would restart the server if we called
            and let it ring 12 times. The PowerKey Pro can also detect
            distinctive ringing, so you could set up an alternate number for
            your main phone line and let the PowerKey Pro only detect calls
            specifically to the alternate number.

            The minuscule Rebound is a stark contrast to the beefy PowerKey
            Pro. It's a sleek three-inch long black ADB cable tipped with a
            bright yellow ball. It fits anywhere in your ADB chain, so you can
            move it around. TidBITS Technical Editor Geoff Duncan ran into
            some "problems" with the Rebound's physical design - you'll enjoy
            reading his report and Sophisticated Circuits' response.

          <http://www.quibble.com/geoff/rebound/>

            Lazarus falls in between the previous two in size, since it's a
            black plastic box with a pair of power plugs (one for the cord to
            the wall, the other for a cord to the Mac), and a pair of ADB
            ports so it can sit in your ADB chain. The Lazarus device I
            received was an early unit and had a distinct hand-made feel.

            MacCoach closely resembles Rebound, with a boxy connector
            replacing the yellow ball on one end of the ADB cable.

          **Restart Method** -- Function follows form with these devices.
            The PowerKey Pro, with its six power outlets, restarts a Mac by
            cutting power to the Mac's power outlet. If the Mac isn't plugged
            into one of the switchable outlets in the PowerKey Pro 200, then
            the PowerKey software instead tries a keyboard restart, which is
            the same as pressing Command-Control-Power on most (but not all)
            Macs. Ideally, the PowerKey Pro should first try Command-Control-
            Power and if that fails, toggle power to the Mac, since toggling
            power can be stressful for the Mac's power supply and other
            components. This is especially true if an application crashes on
            startup, causing the Mac to restart constantly until someone
            intervenes.

            The tiny Rebound can perform only keyboard restarts, limiting its
            range and effectiveness slightly. Some older Macintosh models
            don't support keyboard restarts, so the Rebound doesn't work for
            them. In addition, a crash could totally wipe out ADB, at which
            point a keyboard restart would fail. Luckily, such severe crashes
            are extremely unusual.

            Like the PowerKey Pro, Lazarus toggles power to restart the Mac,
            so it works on all desktop Macs. One small advantage Lazarus has
            over the PowerKey Pro is that international users can use Lazarus
            with no trouble (as I understand it, the female end of power plugs
            is standardized, whereas the male end varies by country). The
            PowerKey Pro's power cable is permanently attached, so it would
            need an adapter in other countries. Neither Rebound nor MacCoach
            worry about power plugs, being ADB devices.

            None of these devices are likely to work well on PowerBooks.
            PowerBook servers probably still have batteries installed, so they
            can withstand short power outages. I think of an internal
            PowerBook battery as a sort of built-in UPS. Thus, neither the
            PowerKey Pro nor Lazarus could restart a PowerBook by toggling
            power. In addition, PowerBooks reportedly have different ADB
            controller chips than desktop Macs, which eliminates MacCoach and
            Rebound (Sophisticated Circuits thought Rebound might work on the
            PowerBook 520/540 series and older, but not on newer PowerBooks).
            The MacCoach information explicitly says it won't work on
            PowerBooks or some 68K Macs.

          **Crash Detection** -- All of these devices use essentially the
            same method of detecting crashes. They rely on software that
            regularly "pings" the hardware to check that the Mac is still
            alive, in essence continually resetting a timer. If that timer
            runs out because the hardware fails to receive pings for a user-
            specified amount of time, the device restarts the Mac.

            The PowerKey Pro and Rebound use a faceless background application
            loaded from the Extensions folder to perform the pinging, whereas
            Lazarus relies on a normal application launched from the Startup
            Items folder. It's possible to quit the Lazarus application and
            lose protection, but it's also easier to turn off Lazarus's
            protection for maintenance or troubleshooting. MacCoach reportedly
            relies on a driver that loads very early, but may not be as
            sensitive as an application.

            The PowerKey Pro, Rebound, and Lazarus can make sure specific
            applications remain active. Applications must explicitly support
            the PowerKey Pro and Rebound, whereas Lazarus can watch any
            application to make sure it's still active (as can the 2.0 version
            of the MacCoach software, reportedly). The list of server
            applications supporting the PowerKey Pro and Rebound currently
            includes WebSTAR, LetterRip Pro, Newsstand, Quid Pro Quo,
            WebServer 4D, WebSiphon, CommuniGate, TeleFinder, and PageSentry.
            Applications support the PowerKey Pro and Rebound by continually
            resetting a hardware timer. An advantage of the PowerKey
            Pro/Rebound method is that applications can restart the Mac if
            they detect low memory situations or other potential problems
            before they cause a crash.

            For multiple server setups, the PowerKey Pro can work with Maxum's
            PageSentry Pro monitoring software to restart a number of servers.
            You plug the PowerKey Pro's ADB cable into the Mac running
            PageSentry, then plug the servers into the PowerKey Pro's
            switchable power outlets. When PageSentry detects that a server
            isn't responding, it toggles power to that server. My servers
            aren't even in the same area code, so this feature doesn't help
            me, but it's useful for many people running multiple servers.

          <http://www.maxum.com/pagesentry/>

            Be careful when deciding which applications Lazarus should watch.
            There's a button to add all the active applications to Lazarus's
            list, but when I accidentally added Email Admin (a LetterRip Pro
            processor), I ran into troubl, since Email Admin launches when
            LetterRip Pro receives its first message, not at startup. After
            startup, when all the other applications launched, Lazarus noticed
            that Email Admin wasn't running, and it restarted the Mac
            repeatedly until I noticed.

            I prefer the method used by Karl Pottie's Keep It Up, a $22
            shareware application that watches applications and when they quit
            or crash, tries to relaunch them, restarting the Mac only if
            relaunching fails.

          <http://www.vl-brabant.be/mac/kiu.html>

          **Restart Next Week** -- The second part of this article will
            discuss the documentation, logging features, interface, and
            pricing of these restart devices.

          $$

           Non-profit, non-commercial publications may reprint articles if
           full credit is given. Others please contact us. We don't guarantee
           accuracy of articles. Caveat lector. Publication, product, and
           company names may be registered trademarks of their companies.

           This file is formatted as setext. For more information send email
           to <setext@tidbits.com>. A file will be returned shortly.

           For information: how to subscribe, where to find back issues,
           and more, email <info@tidbits.com>. TidBITS ISSN 1090-7017.
           Send comments and editorial submissions to: <editors@tidbits.com>
           Back issues available at: <http://www.tidbits.com/tb-issues/>
           And: <ftp://ftp.tidbits.com/pub/tidbits/issues/>
           Full text searching available at: <http://www.tidbits.com/search/>
           -------------------------------------------------------------------
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008104054/http://www.somewhere.com/)
