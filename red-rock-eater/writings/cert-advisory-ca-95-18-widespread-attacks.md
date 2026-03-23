---
id: cert-advisory-ca-95-18-widespread-attacks
title: CERT Advisory CA-95:18 - Widespread Attacks
type: writing
writing_type: rre-post
date: 1995-12-18
url: http://commons.somewhere.com:80/rre/1995/CERT.Advisory.CA-95.18.-.html
coauthors: []
key_concepts: []
importance: 6
research_status: partial
tags:
  - activism
  - history
  - internet-culture
  - libraries
  - technology-policy
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1995/CERT.Advisory.CA-95.18.-.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991003165041/http://www.somewhere.com/)

  

# CERT Advisory CA-95:18 - Widespread Attacks

```
[... and they're not just talking about the Senate.]

Date: Mon, 18 Dec 95 14:22:57 PST
From: RISKS List Owner <risko@csl.sri.com>
Subject: RISKS DIGEST 17.55

RISKS-LIST: Risks-Forum Digest  Monday 18 December 1995  Volume 17 : Issue 55

---

Date: Mon, 18 Dec 1995 12:11:33 -0500
From: CERT Advisory <cert-advisory@cert.org>
Subject: CERT Advisory CA-95:18 - Widespread Attacks

CA-95:18                         CERT Advisory
                               December 18, 1995
                       Widespread Attacks on Internet Sites

Over the last several weeks, the CERT Coordination Center has been working
on a set of incidents in which the intruders have launched widespread
attacks against Internet sites. Hundreds of sites have been attacked, and
many of the attacks have been successful, resulting in root compromises at
the targeted sites. We continue to receive reports, and we believe that more
attacks are going undetected.

  **********************************************************************
  All the vulnerabilities exploited in these attacks are known, and are
  addressed by CERT advisories (see Section III).
  **********************************************************************

We urge everyone to obtain these advisories and take action to ensure that
systems are protected against these attacks. Also, please feel free to
redistribute this message.

As we receive additional information relating to this advisory, we
will place it in
        ftp://info.cert.org/pub/cert_advisories/CA-95:18.README

We encourage you to check our README files regularly for updates on
advisories that relate to your site.

I.   Description

     Intruders are doing the following:

* using automated tools to scan sites for NFS and NIS vulnerabilities* exploiting the rpc.ypupdated vulnerability to gain root access* exploiting the loadmodule vulnerability to gain root access* installing Trojan horse programs and packet sniffers* launching IP spoofing attacks

II.  Impact

     Successful exploitation of the vulnerabilities can result in unauthorized
     root access.

III. Solution

     The CERT staff urges you to immediately take the steps described in
     the advisories and README files listed below. Note that it is important
     to check README files as they contain updated information we received 
     after the advisory was published.
 
     a. Using automated tools to scan sites for NFS and NIS vulnerabilities

* CA-94:15.NFS.Vulnerabilities* CA-94:15.README* CA-92:13.SunOS.NIS.vulnerability

b. Exploiting the rpc.ypupdated vulnerability to gain root access

* CA-95:17.rpc.ypupdated.vul* CA-95:17.README

c. Exploiting the loadmodule vulnerability to gain root access

* CA-93:18.SunOS.Solbourne.loadmodule.modload.vulnerability* CA-95:12.sun.loadmodule.vul* CA-95:12.README

d. Installing Trojan horse programs and packet sniffers

* CA-94:01.ongoing.network.monitoring.attacks* CA-94:01.README

e. Launching IP spoofing attacks

* CA-95:01.IP.spoofing* CA-95:01.README

The CERT advisories and README files are available from

         ftp://info.cert.org/pub/cert_advisories

     If you find a compromise, please complete the Incident Reporting Form
     that we have provided in the appendix of this advisory, and return the
     form to cert@cert.org. This completed form will help us better assist
     you.   

     Note: Because of our workload, we must ask you not to send log files of 
     activity, but we would be happy to work with you as needed on how to
     interpret data that you may collect. Also, the CERT staff can provide
     guidance and advice, if needed, on how to handle incidents and work with
     law enforcement. 

     If you see activity that indicates an attack is in progress, we encourage
     you to contact other sites involved and the service providers, as well as
     the CERT Coordination Center.

Contacting the CERT Coordination Center

For sensitive information, please use encrypted email. 
The CERT public PGP key is available from 
                
        ftp://info.cert.org/pub/CERT_PGP.key

If you prefer to use DES, please call the CERT hotline

        +1 412 268 7090

to exchange a DES key over the phone.

Other CERT contact information:

Internet email: cert@cert.org
Telephone: +1 412-268-7090 (24-hour hotline)
           CERT personnel answer 8:30 a.m.-5:00 p.m. EST(GMT-5)/EDT(GMT-4),
           and are on call for emergencies during other hours.
Fax: +1 412-268-6989

Postal address:  CERT Coordination Center
                 Software Engineering Institute
                 Carnegie Mellon University
                 Pittsburgh, PA 15213-3890
                 USA

CERT advisories and bulletins are posted on the USENET newsgroup
comp.security.announce. If you would like to have future advisories and
bulletins mailed to you or to a mail exploder at your site, please send mail
to cert-advisory-request@cert.org.

Past CERT publications, information about FIRST representatives, and
other information related to computer security are available from
ftp://info.cert.org/pub/

Copyright 1995 Carnegie Mellon University
This material may be reproduced and distributed without permission provided it
is used for noncommercial purposes and the copyright statement is included.

CERT is a service mark of Carnegie Mellon University.

  [The Copyrighted 1995 Incident Reporting Form is omitted from this
  RISKS version.  Send e-mail to the CERT to obtain a copy.  PGN]

CERT is a service mark of Carnegie Mellon University.

---

End of RISKS-FORUM Digest 17.55 

---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991003165041/http://www.somewhere.com/)