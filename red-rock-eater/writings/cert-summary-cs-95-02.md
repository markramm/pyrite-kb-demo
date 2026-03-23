---
id: cert-summary-cs-95-02
title: CERT Summary CS-95:02
type: writing
writing_type: rre-post
date: 1995-09-26
url: http://commons.somewhere.com:80/rre/1995/CERT.Summary.CS-95.2.html
coauthors: []
key_concepts: []
importance: 6
research_status: partial
tags:
  - history
  - internet-culture
  - libraries
  - privacy
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1995/CERT.Summary.CS-95.2.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991003183850/http://www.somewhere.com/)

  

# CERT Summary CS-95:02

```
Date: Tue, 26 Sep 1995 16:26:56 -0400
From: CERT Advisory <cert-advisory@cert.org>
Subject: CERT Summary CS-95:02

CERT Summary CS-95:02
September 26, 1995

The CERT Coordination Center periodically issues the CERT Summary to draw
attention to the types of attacks currently being reported to our incident
response staff. The summary includes pointers to sources of information for
dealing with the problems. Starting with this summary, we will also list new
or updated files that are available for anonymous FTP from ftp://info.cert.org

Past CERT Summaries are available from 
     ftp://info.cert.org/pub/cert_summaries
  ---------------------------------------------------------------------------

Recent Activity

---

Since the July CERT Summary, we have seen these continuing trends in incidents
reported to us:

1. Sendmail Attacks

We receive several reports each week of attacks through sendmail, with
intruders using a variety of techniques. Most of the attacks are aimed at
gaining privileged access to the victim machine.

To combat these threats, we encourage sites to take the appropriate steps
outlined in the following:

  ftp://info.cert.org/pub/cert_advisories/CA-95:11.sun.sendmail-oR.vul
  ftp://info.cert.org/pub/cert_advisories/CA-95:11.README

  ftp://info.cert.org/pub/cert_advisories/CA-95:08.sendmail.v.5.vulnerability
  ftp://info.cert.org/pub/cert_advisories/CA-95:08.README

A number of sites have reported some confusion on the need to continue using
the sendmail restricted shell program (smrsh). You need to run the smrsh tool
in conjunction with the most recently patched version of sendmail for your
system.

Information on the smrsh tool can be obtained from these places in
  ftp://info.cert.org/pub/

                   tools/sendmail/smrsh/
                   cert_advisories/CA-93:16.sendmail.vulnerability
                   cert_advisories/CA-93:16a.sendmail.vulnerability.supplement
                   cert_advisories/CA-93:16a.README
                   cert_advisories/CA-95:11.sun.sendmail-oR.vul
                   cert_advisories/CA-95:11.README

The smrsh program can be obtained from

  ftp://info.cert.org/pub/tools/smrsh/

It is included in the sendmail 8.7 distribution.

2. Network Scanning

Several incidents have recently been reported in which intruders scan a large
address range using the Internet Security Scanner (ISS). As described in CERT
advisory CA-93:14, this tool interrogates all computers within a specified IP
address range, determining the security posture of each with respect to
several common system vulnerabilities.

Intruders have used the information gathered from these scans to compromise
sites. We are aware of many systems that have suffered a root compromise as a
result of information intruders obtained from ISS scans.

You may wish to run ISS against your own site in accordance with your
organization's policies and procedures. ISS is available from

  ftp://info.cert.org/pub/tools/iss/iss13.tar

We encourage you to take relevant steps outlined in these documents:

  ftp://info.cert.org/pub/cert_advisories/CA-93:14.Internet.Security.Scanner
  ftp://info.cert.org/pub/cert_advisories/CA-93:14.README
  ftp://info.cert.org/pub/tech_tips/security_info
  ftp://info.cert.org/pub/tech_tips/packet_filtering

3. Exploitation of rlogin and rsh

We have received some reports about the continued exploitation of a
vulnerability in rlogin and rsh affecting IBM AIX 3 systems and Linux systems.
This is not a new vulnerability, but it continues to exist. Sites have
reported encountering some Linux distributions that contain this
vulnerability.

Information on this vulnerability and available solutions can be
obtained from

  ftp://info.cert.org/pub/cert_advisories/CA-94:09.bin.login.vulnerability
  ftp://info.cert.org/pub/cert_advisories/CA-94:09.README

4. Packet Sniffers

We continue to receive new incident reports daily about sniffers on
compromised hosts. These sniffers, used to collect account names and
passwords, are frequently installed using a kit. In some cases, the packet
sniffer was found to have been running for months. Occasionally, sites had
been explicitly warned of the possibility of such a compromise, but the
sniffer activity continued because the site did not address the problem in the
comprehensive manner that we suggest in our security documents.

Further information on packet sniffers is available from

  ftp://info.cert.org/pub/cert_advisories/CA-94:01.network.monitoring.attacks
  ftp://info.cert.org/pub/cert_advisories/CA-94:01.README

Information about detecting sniffers using cpm is in the CA-94:01.README
file. 

What's New in the CERT FTP Archive

---

We have made the following changes since June 1, 1995.- New Additions:

  ftp://info.cert.org/pub/

      incident.reporting.form (the form you should fill out when
                               reporting an incident to our staff)

  ftp://info.cert.org/pub/cert_advisories/

      CA-95:08.sendmail.v.5.vulnerability
      CA-95:09.Solaris.ps.vul
      CA-95:10.ghostscript
      CA-95:11.sun.sendmail-oR.vul

  ftp://info.cert.org/pub/cert_bulletins/

      VB-95:05.osf    (OSF/DCE security hole)
      VB-95:06.cisco  (vulnerability in Cisco's IOS software)

  ftp://info.cert.org/pub/tech_tips/

      AUSCERT_checklist_1.0 (UNIX checklist developed by the Australian
                             Emergency Response Team)- Updated Files 

    ftp://info.cert.org/pub/cert_advisories/

      CA-93:14.README (Internet Security Scanner)
      CA-94:01.README (network monitoring)
      CA-94:02.README (SunOS rpc mountd vulnerability)
      CA-94:05.README (md5)
      CA-94:11.README (majordomo) 
      CA-95:01.README (IP spoofing and hijacked terminal connections) 
      CA-95:02.README (binmail vulnerabilities)
      CA-95:05.README (sendmail - several vulnerabilities)
      CA-95:08.README (sendmail version 5 and IDA sendmail) 
      CA-95:09.README (Solaris ps)
      CA-95:11.README (Sun sendmail -oR vulnerability) 

    We have begun adding a note to advisory README files reminding readers to
    check with vendors for current checksum values. After we publish checksums in
    advisories and READMEs, files and checksums are sometimes updated at
    individual locations.- Other Changes:

      As we will no longer be keeping the lsof directory current, the directory and
      its files have been removed from our FTP site. The current version of lsof is
      available from

        ftp://vic.cc.purdue.edu/pub/tools/unix/lsof

      ---

      How to Contact the CERT Coordination Center

      Email    cert@cert.org 

      Phone    +1 412-268-7090 (24-hour hotline) 
                      CERT personnel answer 8:30-5:00 p.m. EST
                      (GMT-5)/EDT(GMT-4), and are on call for
                      emergencies during other hours. 

      Fax      +1 412-268-6989

      Postal address
              CERT Coordination Center
              Software Engineering Institute
              Carnegie Mellon University
              Pittsburgh PA 15213-3890

      To be added to our mailing list for CERT advisories 
      and bulletins, send your email address to

              cert-advisory-request@cert.org

      CERT advisories and bulletins are posted on the USENET news group

               comp.security.announce

      If you wish to send sensitive incident or vulnerability information to CERT
      staff by electronic mail, we strongly advise that the email be encrypted.  
      We can support a shared DES key, PGP, or PEM (contact CERT staff for details).

      Location of CERT PGP key

               ftp://info.cert.org/pub/CERT.PGP_key

        ---------------------------------------------------------------------------
        Copyright 1995 Carnegie Mellon University
        This material may be reproduced and distributed without permission
        provided it is used for noncommercial purposes and credit is given to the
        CERT Coordination Center.  CERT is a service mark of Carnegie Mellon Univ.

      ---
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991003183850/http://www.somewhere.com/)