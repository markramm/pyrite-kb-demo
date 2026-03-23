---
id: ssl-tunneling-and-privacy-proxies
title: SSL Tunneling and Privacy Proxies
type: writing
writing_type: rre-post
date: 1995-06-30
url: http://commons.somewhere.com:80/rre/1995/SSL.Tunneling.and.Privac.html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - commerce
  - cryptography
  - education
  - environment
  - forwarded-content
  - law
  - privacy
---



## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1995/SSL.Tunneling.and.Privac.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008140009/http://www.somewhere.com/)

  

# SSL Tunneling and Privacy Proxies

```
Date: Fri, 30 Jun 1995 21:13:47 -0700
From: Hal <hfinney@shell.portal.com>
To: ssl-talk@netscape.com
Subject: SSL Tunneling and Privacy Proxies

Using SSL Tunneling to Increase User Privacy			Hal Finney
--------------------------------------------			June 30, 1995

Abstract

A recent proposed Internet Draft suggests an extension to the methods
supported by WWW proxy servers to allow SSL tunneling.  The same ideas
can serve as the basis for a technique to allow the user to browse the
web with enhanced privacy, such that even his internet service provider
does not learn the contents or even the addresses of the web sites he
visits.

Rationale

Privacy is a concern of increasing importance to users on the net,
where the basic communication protocols are notoriously insecure.
Encryption technologies such as SSL (Secure Sockets Layer from Netscape
Communications Corporation) enhance user privacy and security by
allowing communications which are secure against eavesdropping.
Although these are most commonly deployed today primarily to protect
the transfer of sensitive data (credit card numbers, etc.), the same
approach can provide privacy of message contents in a more general
sense.  A user of the internet does not want to feel that every byte he
sends and receives, every web site he browses, every file he views or
downloads, is capable of being recorded and monitored by others on the
net.  The use of encryption can protect the contents of the data he
sends and receives.

However, despite the existence of SSL and similar technologies, the
typical user will still be vulnerable to one important loss of
privacy.  Usually the organization which serves as the user's interface
to the net has the power to learn a great deal about the user's
activities.  Even if SSL or other privacy enhancements are used, at
least the set of sites visited by the user is generally visible to the
ISP (internet service provider).  At the most fundamental level, the
nature of the TCP/IP connections used in the net makes it possible for
those whose systems pass the packets to observe where they are going.

The problem is especially acute in the growing segment of the WWW
market consisting of individuals who have a connection to the net via a
commercial ISP.  These individuals are often browsing the net from
home, and therefore have a greater expectation of privacy than business
or some academic users who get net access through their employer or
educational establishment.

In some cases, such as with large commercial networks like America
OnLine and Prodigy, the interface between the end user and the ISP is
proprietary, with the ISP originating the net connection.  On these
systems there is almost no opportunity for the user to protect his
privacy from the commercial provider.  He is essentially reduced to
trusting the provider to use the information it gathers about his
browsing habits appropriately.

However, there are increasing numbers of end users getting more direct
access to the Internet via SLIP, PPP, and similar protocols, with a
commercial company providing the net interface using these standards.
These users have much more control over the tools they use to browse
the net and the protocols they use to connect to remote sites.  They
can use SSL to protect what they send and receive, but with current
technology they are still vulnerable to the ISP knowing where they
connect.

This kind of information is definitely of interest to ISP's.  A recent
article in the New York Times ("Microsoft's On-Line Service to
Withhold Subscriber Names From Its Own Vendors", by Don Clark, circa
June 23, 1995) describes the efforts of Microsoft as it enters the ISP
market to control information about where subscribers browse.  The
competition between Microsoft and the vendors on the Microsoft Network
for this kind of information demonstrates its commercial value.  The
users' privacy interests are not mentioned.  However, as awareness of
the problem rises, so will the motivation to seek a solution.

Privacy Proxies

The concept of "privacy proxies" provides a way of solving this problem,
allowing a user to visit sites on the net in such a way that neither
the ISP nor any other single entity on the net will know where he is
connecting.  The information will be dispersed in such a way that only
by collecting data from multiple points on the net simultaneously
would it be possible for a snooper to link a user with the sites he
has visited.

The basic idea is to use a special kind of WWW proxy whose purpose is
to enhance user privacy.  This proxy acts as a forwarder for packets
between the user and the site he is visiting.  Unlike the normal kind
of proxy, this privacy proxy may not necessarily be located in close
proximity to the user on the net, but may be a remote system which
offers this service to general users.  Connections to these proxies are
made using encryption, such as via SSL.  Once the secure channel to the
proxy is established, the user's browser sends commands to connect to
further sites.

If only a single privacy proxy were used, the user's privacy would
still be vulnerable to that proxy's owners and operators.  The proxy
will see both the incoming connection from the user and the site to
which the user wishes to connect.  This information could be recorded
and ultimately represent as much a threat to the privacy of the user
as if it were collected by the ISP.

However, this problem can be mitigated by using multiple proxies in a
chain.  The user connects to privacy proxy A, using encryption, and
sends a command requesting it to connect to privacy proxy B.  The user
and B then negotiate a secure connection using SSL or other encryption.
Now the user can send a proxy request to B requesting it to connect to
the final site the user wishes to visit.  This message is not visible
to earlier sites in the chain, neither proxy A nor the local ISP.  And
proxy server B sees only a request from proxy server A; it gets no
information about the original source of the request.  The result is
that no one in the chain, not the ISP, not proxy A, not proxy B, and
not the end site, is able to know both the user and the site he is
visiting.  His privacy is thereby protected.

The same strategy can be applied to build longer chains, further
dispersing the information which must be collected in order to
determine which sites a user is browsing.  Clearly a tradeoff will
exist between the length of the chain and the response time to
connection requests, but various shortcuts may be possible to reduce
the costs associated with chains of moderate length.

Note too that this approach has the byproduct of further protecting the
user's privacy, because all his web connections, not just the one to
special "secure" sites, are encrypted as they pass through the ISP.
So not only are the destinations protected, the message contents are,
too.  This is true even for connections made to insecure WWW sites.

In order for this approach to enhancing privacy to be effective,
several steps must occur.  A protocol must be defined for
communication with and between browsers, privacy proxies, and other
kinds of WWW proxies and servers.  Browsers must be enhanced to
support chains of privacy proxies, or other means made available to
users to allow them to access the privacy network.  And an
infrastructure of privacy proxies must be established, with proxy
addresses and policies published so that users and their software
agents can choose an appropriate chain through the network.

Most of these steps are beyond the scope of this document.  However the
communications protocol can be based closely on the current proposal
for SSL Tunneling.

SSL Tunneling

The existing Internet Draft "Tunneling SSL Through a WWW Proxy" by Ari
Luotonen of Netscape Communications Corporation (<URL:
ftp://ds.internic.net/internet-drafts/draft-luotonen-ssl-tunneling-00.txt>)
describes a proposed modification to the behavior of conventional WWW
proxies to allow for the use of SSL in a situation where a proxy must
be used, possibly in an insecure environment.  Although the situation
addressed by that document (hereafter called the "Tunneling SSL" draft)
is for a specific purpose, the modifications suggested are also well
suited for dealing with the privacy issues discussed here.

The enhancement proposed by the "Tunneling SSL" draft is to add a new
command (or, using HTTP terminology, "method") to the WWW proxy, called
CONNECT.  This command is followed by an internet address in the form
of hostname and port number to which a connection should be made.  The
proxy makes a TCP/IP connection to the specified host and port, and
then simply transfers bytes transparently between the new connection
and the incoming one on which the CONNECT command was given.  It
therefore serves as a transparent pipeline once the connection is
made.  This allows SSL negotiation to occur between the user and the
remote host with the proxy serving as a forwarder.  As a result, once
an SSL session has been set up between the user and the remote host,
the proxy is not able to read the contents of the encrypted SSL data
sent between user and remote system.

For the purposes of the privacy proxy, the principal additional
requirement beyond those discussed in the "Tunneling SSL" draft is that
the CONNECT functionality be available even when connection to the
proxy server is made securely via SSL.  This is a reasonable assumption
since SSL is designed to be transparent, and a proxy server which
accepts GET on SSL connections can easily be enhanced to accept
CONNECT.

(Although one point made in the "Tunneling SSL" draft is that the proxy
server need not run SSL, it would of course require this ability in
order to accept encrypted connections.  However it is reasonable to
anticipate that implementations of SSL will be widely available,
making it very practical for proxy servers to run SSL.)

A server which accepts encrypted SSL connections and then supports the
CONNECT command described in the "Tunneling SSL" draft would satisfy
the requirements for the privacy proxy described earlier.  In
particular, it would be possible to set up a chain of proxies,
successively passing CONNECT commands to all but the last proxy in the
chain.  A separate SSL negotiation occurs with each proxy so that no
proxy sees the connections made by other proxies in the chain.

There is a security issue relating to the limitations on incoming
connections and on outgoing connections which will be allowed.  For the
purposes of a privacy proxy, incoming connections will typically be
accepted from a wide and possibly unlimited set of machines, depending
on the policies of the operator of the proxy.  However it would be
dangerous to allow an unlimited set of outgoing connections, as the
privacy proxy could then be used as a base for various forms of attacks
based on security flaws in hosts on the net.

The "Tunneling SSL" draft suggests that outgoing connections be allowed
only to ports defined as accepting SSL connections.  However, this
advice should be modified for the purpose of a privacy proxy.  Although
connections to other privacy proxies would typically be made on the
https port, it would also frequently be the case that connections were
made to ordinary http (not https) servers.  This would generally be the
case for the last connection in the chain, where the actual data being
requested comes from a server which may not support SSL.  So for
privacy proxies an appropriate recommendation would be to allow
outgoing connections to ports assigned or commonly used for https and
http connections.  This should provide the necessary functionality
while reducing the security risks borne by the operator of the privacy
proxy.

Summary

The extensions to the WWW proxy mechanism proposed in "Tunneling SSL
Through a WWW Proxy" are well suited to the purpose of increasing
browser privacy.  The main additional requirement is that the CONNECT
functionality be available on incoming encrypted SSL connections.
Agreement on this protocol would be the first step in the development
of a widespread infrastructure of privacy proxies running WWW servers
with these extensions and allowing unlimited incoming connections.
Such a development can increase end user privacy by allowing users to
protect the sites they browse in addition to the contents of the data
they view.
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991008140009/http://www.somewhere.com/)