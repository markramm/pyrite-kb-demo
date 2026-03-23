---
id: rre-that-worm-i-was-talking-about
title: "[RRE]that worm I was talking about"
type: writing
writing_type: rre-post
date: 1999-06-10
url: http://commons.somewhere.com:80/rre/1999/RRE.that.worm.I.was.talk.html
importance: 6
research_status: partial
tags:
  - civil-liberties
  - commerce
  - cryptography
  - education
  - international
  - internet-policy
  - law
  - media
  - military
  - privacy
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1999/RRE.that.worm.I.was.talk.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009081111/http://www.somewhere.com/)

  

# [RRE]that worm I was talking about

```
[Pathetic.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html
or send a message to requests@lists.gseis.ucla.edu with Subject: info rre

---

Date: Tue, 15 Jun 1999 12:07:31 -0700 (PDT)
From: risks@csl.sri.com

RISKS-LIST: Risks-Forum Digest  Tuesday 15 June 1999  Volume 20 : Issue 44

---

Date: Mon, 14 Jun 1999 07:16:05 -0400
From: CERT Advisory <cert-advisory@cert.org>
Subject: CERT Advisory CA-99.06 - New information regarding ExploreZip

CERT Advisory CA-99-06-explorezip

   Original issue date: Thursday June 10, 1999
   Last Revised Date: June 14, 1999
   Added information about the program's self-propagation via networked
   shares; also updated anti-virus vendor URLs.
   
   Source: CERT/CC
   
Note: The CERT Coordination Center has discovered new information
regarding the ExploreZip worm. This re-issue of CERT Advisory CA-99-06
contains new information regarding an additional means by which the
Worm can spread, and a caution about disinfecting your systems. We
will continue to update this advisory as new information is
discovered. We encourage you to check our web site frequently for any
new information.

Systems Affected

* * Machines running Windows 95, Windows 98, or Windows NT.* * Machines with filesystems and/or shares that are writable by a
    user of an infected system.* * Any mail handling system could experience performance problems or
      a denial of service as a result of the propagation of this Trojan
      horse program.

Overview

   The CERT Coordination Center continues to receive reports and
   inquiries regarding various forms of malicious executable files that
   are propagated as file attachments in electronic mail.
   
   During the second week of June 1999, the CERT/CC began receiving
   reports of sites affected by ExploreZip, a Trojan horse/worm program
   that affects Windows systems and has propagated in e-mail attachments.
   The number and variety of reports we have received indicate that this
   has the potential to be a widespread attack affecting a variety of
   sites.
   
I. Description

   Our original analysis indicated that the ExploreZip program is a
   Trojan horse, since it initially requires a victim to open or run an
   e-mail attachment in order for the program to install a copy of itself
   and enable further propagation. Further analysis has shown that, once
   installed, the program may also behave as a worm, and it may be able
   to propagate itself, without any human interaction, to other networked
   machines that have certain writable shares.
   
   The ExploreZip Trojan horse has been propagated between users in the
   form of e-mail messages containing an attached file named
   zipped_files.exe. Some e-mail programs may display this attachment
   with a "WinZip" icon. The body of the e-mail message usually appears to
   come from a known e-mail correspondent, and typically contains the
   following text:
   
   I received your email and I shall send you a reply ASAP.
          Till then, take a look at the attached zipped docs.
          
   The subject line of the message may not be predictable and may appear
   to be sent in reply to previous e-mail.
   
   Opening the zipped_files.exe file causes the program to execute. It is
   possible under some mailer configurations that a user might
   automatically open a malicious file received in the form of an e-mail
   attachment. When the program is run, an error message is displayed:
   
   Cannot open file: it does not appear to be a valid archive. If this
   file is part of a ZIP format backup set, insert the last disk
   of the backup set and try again. Please press F1 for help.
          
Destruction of files

* * The program searches local and networked drives (drive letters C
  through Z) for specific file types and attempts to erase the
  contents of the files, leaving a zero byte file. The targets may
  include Microsoft Office files, such as .doc, .xls, and .ppt, and
  various source code files, such as .c, .cpp, .h, and .asm.* * The program may also be able to delete files that are writable to
    it via SMB/CIFS file sharing. The program appears to look through
    the network neighborhood and delete any files that are shared and
    writable, even if those shares are not mapped to networked drives
    on the infected computer.* * The program appears to continually delete the contents of targeted
      files on any mapped networked drives.
      The program does not appear to delete files with the "hidden" or
      "system" attribute, regardless of their extension.

System modifications

* * The zipped_files.exe program creates a copy of itself in a file
  called explore.exe in the following location(s):
         
  On Windows 98 - C:\WINDOWS\SYSTEM\Explore.exe
  On Windows NT - C:\WINNT\System32\Explore.exe
                  
  This explore.exe file is an identical copy of the zipped_files.exe
  Trojan horse, and the file size is 210432 bytes.
  MD5 (Explore.exe) = 0e10993050e5ed199e90f7372259e44b* * On Windows 98 systems, the zipped_files.exe program creates an
    entry in the WIN.INI file:
           
    run=C:\WINDOWS\SYSTEM\Explore.exe
                    
    On Windows NT systems, an entry is made in the system registry:
           
    [HKEY_CURRENT_USER\Software\Microsoft\Windows
    NT\CurrentVersion\Windows]
    run = "C:\WINNT\System32\Explore.exe"

Propagation via file sharing

   Once explore.exe is running, it takes the following steps to propagate
   to other systems via file sharing:

* * Each time the program is executed, the program will search the
  network for all shares that contain a WIN.INI file with a valid
  "[windows]" section in the file.* * For each such share that it finds, the program will attempt to
    + + copy itself to a file named setup.exe on that share+ + modify the WIN.INI file on that share by adding the entry
        "run=_setup.exe"The account running the program on the original infected machine
    needs to have permission to write to the second victim's shared
    directory. (That is, no vulnerabilities are being exploited in
    order for the program to spread in this manner.)
    The setup.exe file is identical to the zipped_files.exe and
    explore.exe files on the original infected machine.* * The original infected system will continue to scan shares that
      have been mapped to a local drive letter containing a valid
      WIN.INI file. For each such share that is found, the program will
      "re-infect" the victim system as described above.

On Windows 98 systems that have a "run=_setup.exe" entry in the
   WIN.INI file (as described previously), the C:\WINDOWS\_setup.exe
   program is executed automatically whenever a user logs in. On Windows
   NT systems, a "run=_setup.exe" entry in the WIN.INI file does not
   appear to cause the program to be executed automatically.
   
   When run as setup.exe, the program will attempt to

* * make another copy of itself in C:\WINDOWS\SYSTEM\Explore.exe* * modify the WIN.INI file again by replacing the "run=_setup.exe"
    entry with "run=C:\WINDOWS\SYSTEM\Explore.exe"

Note that when the program is run as setup.exe, it configures the
   system to later run as explore.exe. But when run as explore.exe, it
   attempts to infect shares with valid WIN.INI files by configuring
   those files to run setup.exe. Since this infection process includes
   local shares, affected systems may exhibit a "ping pong" behavior in
   which the infected host alternates between the two states.
   
Propagation via e-mail

   The program propagates by replying to any new e-mail that is received
   by the infected computer. The reply messages are similar to the
   original e-mail described above, each containing another copy of the
   zipped_files.exe attachment.
   
   We will continue to update this advisory with more specific
   information as we are able to confirm details. Please check the
   CERT/CC web site for the current version containing a complete
   revision history.
   
II. Impact

* * Users who execute the zipped_files.exe Trojan horse will infect
  the host system, potentially causing targeted files to be
  destroyed.* * Users who execute the Trojan horse may also infect other networked
    systems that have writable shares.* * Because of the large amount of network traffic generated by
      infected machines, network performance may suffer.* * Indirectly, this Trojan horse could cause a denial of service on
        mail servers. Several large sites have reported performance
        problems with their mail servers as a result of the propagation of
        this Trojan horse.

III. Solution

Use virus scanners

   While many anti-virus products are able to detect and remove the
   executables locally, because of the continuous re-infection process,
   simply removing all copies of the program from an infected system may
   leave your system open to re-infection at a later time, perhaps
   immediately. To prevent re-infection, you must not serve any shares
   containing a WIN.INI file to any potentially infected machines. If you
   share files with everyone in your domain, then you must disable shares
   with WIN.INI files until every machine on your network has been
   disinfected.
   
   In order to detect and clean current viruses, you must keep your
   scanning tools up to date with the latest definition files. Please see
   the following anti-virus vendor resources for more information about
   the characteristics and removal techniques for the malicious file
   known as ExploreZip.
   
   Aladdin Knowledge Systems, Inc.
          http://www.esafe.com/vcenter/explore.html
          
          Central Command
          http://www.avp.com/zippedfiles/zippedfiles.html
          
          Command Software Systems, Inc
          http://www.commandcom.com/html/virus/explorezip.html
          
          Computer Associates
          http://www.cai.com/virusinfo/virusalert.htm
          
          Data Fellows
          http://www.datafellows.com/news/pr/eng/19990610.htm
          
          McAfee, Inc. (a Network Associates company)
          http://www.mcafee.com/viruses/explorezip/default.asp
          
          Network Associates Incorporated
          http://www.avertlabs.com/public/datafiles/valerts/vinfo/va10185
          .asp
          
          Sophos, Incorporated
          http://www.sophos.com/downloads/ide/index.html#explorez
          
          Symantec
          http://www.symantec.com/avcenter/venc/data/worm.explore.zip.htm
          l
          
          Trend Micro Incorporated
          http://www.antivirus.com/vinfo/alerts.htm
          
   Additional sources of virus information are listed at
   
   http://www.cert.org/other_sources/viruses.html
          
Additional suggestions

* * Blocking Netbios traffic at your network border may help prevent
  propagation via shares from outside your network perimeter.* * Disable file serving on workstations. You will not be able to
    share your files with other computers, but you will be able to
    browse and get files from servers. This will prevent your
    workstation from being infected via file sharing propagation.* * Maintain a regular, off-line, backup cycle.

General protection from e-mail Trojan horses and viruses

   Some previous examples of malicious files known to have propagated
   through electronic mail include

* * False upgrade to Internet Explorer - discussed in CA-99-02
  http://www.cert.org/advisories/CA-99-02-Trojan-Horses.html* * Melissa macro virus - discussed in CA-99-04
    http://www.cert.org/advisories/CA-99-04-Melissa-Macro-Virus.html* * Happy99.exe Trojan Horse - discussed in IN-99-02
      http://www.cert.org/incident_notes/IN-99-02.html* * CIH/Chernobyl virus - discussed in IN-99-03
        http://www.cert.org/incident_notes/IN-99-03.html

In each of the above cases, the effects of the malicious file are
   activated only when the file in question is executed. Social
   engineering is typically employed to trick a recipient into executing
   the malicious file. Some of the social engineering techniques we have
   seen used include

* * Making false claims that a file attachment contains a software
  patch or update* * Implying or using entertaining content to entice a user into
    executing a malicious file* * Using e-mail delivery techniques which cause the message to appear
      to have come from a familiar or trusted source* * Packaging malicious files in deceptively familiar ways (e.g., use
        of familiar but deceptive program icons or file names)

The best advice with regard to malicious files is to avoid executing
   them in the first place. CERT advisory CA-99-02 discusses Trojan
   horses and offers suggestions to avoid them (please see Section V).
   
   http://www.cert.org/advisories/CA-99-02-Trojan-Horses.html
   ______________________________________________________________________
   
   This document is available from:
   http://www.cert.org/advisories/CA-99-06-explorezip.html.
   ______________________________________________________________________
   
CERT/CC Contact Information

  E-mail: cert@cert.org
  Phone: +1 412-268-7090 (24-hour hotline)
  Fax: +1 412-268-6989
  Postal address:
    CERT Coordination Center
    Software Engineering Institute
    Carnegie Mellon University
    Pittsburgh PA 15213-3890  U.S.A.
          
  CERT personnel answer the hotline 08:00-20:00 EST(GMT-5) / EDT(GMT-4)
  Monday through Friday; they are on call for emergencies during other
  hours, on U.S. holidays, and on weekends.
   
Using encryption

   We strongly urge you to encrypt sensitive information sent by e-mail.
   Our public PGP key is available from http://www.cert.org/CERT_PGP.key.
   If you prefer to use DES, please call the CERT hotline for more
   information.
   
Getting security information

   CERT publications and other security information are available from
   our web site http://www.cert.org/.
   
   To be added to our mailing list for advisories and bulletins, send
   e-mail to cert-advisory-request@cert.org and include SUBSCRIBE
   your-e-mail-address in the subject of your message.
   
   Copyright 1999 Carnegie Mellon University.
   Conditions for use, disclaimers, and sponsorship information can be
   found in http://www.cert.org/legal_stuff.html.

* * "CERT" and "CERT Coordination Center" are registered in the U.S.
  Patent and Trademark Office
  ______________________________________________________________________

   NO WARRANTY
   Any material furnished by Carnegie Mellon University and the Software
   Engineering Institute is furnished on an "as is" basis. Carnegie
   Mellon University makes no warranties of any kind, either expressed or
   implied as to any matter including, but not limited to, warranty of
   fitness for a particular purpose or merchantability, exclusivity or
   results obtained from use of the material. Carnegie Mellon University
   does not make any warranty of any kind with respect to freedom from
   patent, trademark, or copyright infringement.

Revision History

June 10, 1999:  Initial release
June 11, 1999:  Added information about the appearance of the attached file
                Added information from Aladdin Knowledge Systems, Inc.
June 14, 1999:  Added information about the program's self-propagation via
                networked shares; also updated anti-virus vendor URLs

  [(S)lightly edited for RISKS.  PGN]

---

Date: Fri, 11 Jun 1999 13:26:33 -0400
From: "Steven M. Bellovin" <smb@research.att.com>
Subject: W32/ExploreZip.worm "virus" and user interfaces

Subtitle: "I got it from Agnes, she got it from Jim"...  (Tom Lehrer)

Another month, another killer "virus".  By now, everyone has heard about
this latest piece of malware.  But what's interesting is that part of the
way it spread appears to be dependent on the user interface.

The actual damage was done by an executable, a .EXE file.  However,
according to some reports the file itself contained the icon of a .ZIP
file.  Thus, even moderately cautious users could be tricked into opening
the file -- which in this case meant executing it.

The underlying problem is that there are two different mechanisms used to
determine file type, and hence how it should be "opened".  One is what
is displayed to the user; the other is what is actually used.  That way
lies danger.

  [But it can also spread worm-like without your help.  Some folks still
  need to learn some of the lessons from the 1965 efforts on Multics!  See
    http://www.multicians.org/     
  PGN]

---

End of RISKS-FORUM Digest 20.44 

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991009081111/http://www.somewhere.com/)