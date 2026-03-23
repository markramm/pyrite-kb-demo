---
id: path-profiling-and-year-2000-problems
title: path profiling and year 2000 problems
type: writing
writing_type: rre-post
date: 2000-05-24
url: http://commons.somewhere.com:80/rre/1997/path.profiling.and.year..html
coauthors: []
key_concepts: []
importance: 5
research_status: partial
tags:
  - auto-imported
  - education
  - forwarded-content
  - libraries
  - military
  - rre
  - rre-post
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1997/path.profiling.and.year..html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20000527064423/http://commons.somewhere.com/rre/) | **Most Recent Article: Wed, 24 May 2000** |

# path profiling and year 2000 problems

```
[So now there's a whole science for reverse engineering old computer
programs, treating them the same way that one would treat any other
mysterious artifact that might be dug up, or left behind by aliens.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Mon, 24 Mar 1997 16:00:22 -0800 (PST)
From: risks@csl.sri.com

RISKS-LIST: Risks-Forum Digest  Monday 24 March 1997  Volume 18 : Issue 93

---

Date: Fri, 21 Mar 1997 20:09:19 -0600 (CST)
From: Thomas Reps <reps@cs.wisc.edu>
Subject: The Year 2000 Problem -- a new principle for Y2K tools (RISKS-18.53)

Back in October, PGN posted the following note to the RISKS newsgroup.

>> I ran into Tom Reps this morning in San Francisco ...  Tom has been 
>> chartered by DARPA to make serious recommendations on the Year-2000 problem.

I would like to bring one of the results that came out of this to the
attention of RISKS readers.

As PGN indicated, the Defense Advanced Research Projects Agency (DARPA)
asked me last summer to help them plan a project aimed at reducing the
impact of the Year 2000 (Y2K) problem on the Department of Defense.  DARPA
was particularly interested in whether there were "any techniques in the
research community that could be applied to the Y2K problem and have impact
beyond present commercial Y2K products and services".  The most exciting of
the ideas that turned up concerns a method for using path profiling as a
heuristic to locate some of the sites in a program where there are
problematic date manipulations.  It works as follows:

  In path profiling, a program is instrumented so that the number of
  times each different loop-free path executes is accumulated during an
  execution run.  With such an instrumented program, each run (or set of
  runs) of the program generates a path spectrum for the execution --- a
  distribution of the paths that were executed.  Path spectra can be
  used to identify paths in a program that are good candidates for being
  date-dependent computations by finding differences between path
  spectra from execution runs on pre-year-2000 data and post-year-2000
  data.  By choosing input datasets to hold all factors constant except
  the way dates are used in the program, any differences in the spectra
  obtained from different execution runs can be attributed to
  date-dependent computations in the program.  Differences in the
  spectra reveal paths along which the program performed a new sort of
  computation during the post-year-2000 run, as well as paths --- and
  hence computations --- that were no longer executed during the
  post-year-2000 run.

With some further analysis of the spectra, for each such path that shows up
in the spectral difference, it is possible to identify the shortest prefix
that distinguishes it from all of the paths in the other path set.

For the Y2K problem, the path-spectrum comparison technique may
provide help with two aspect of the problem:

  (i)  determining the sites at which date-manipulation code occurs, and
  (ii) post-renovation testing.

Of course, the path-spectrum comparison technique is not guaranteed to
uncover all sites of date manipulations.  No technique can do this; all one
can hope for are good heuristics.  However, because path-spectrum comparison
involves a different principle from the principles that lie behind the
heuristics used in commercial Y2K tools, it should be a good complement to
current techniques.

Furthermore, the path-spectrum comparison technique is actually applicable
to a much wider range of software-maintenance problems than just the Y2K
problem; it offers new perspectives on program testing, on the task of
creating test data, and on what tools can be created to support program
testing.

This work is described in the following paper:

  Reps, T., Ball, T., Das, M., and Larus, J., "The use of program
  profiling for software maintenance with applications to the Year 2000
  Problem".  Technical Report TR-1335, Computer Sciences Department,
  University of Wisconsin, Madison, WI, January 1997.

The paper is available over the WWW at URL
  http://www.cs.wisc.edu/wpis/papers/tr1335.ps.

A prototype tool for gathering and comparing path spectra (for programs that
run under Solaris on Sun SPARCstations) has been built at the University of
Wisconsin.

(The Wisconsin Alumni Research Foundation is in the process of seeking
patent protection for these techniques.)

Tom

---

End of RISKS-FORUM Digest 18.93 

---

Standard Risks reuse disclaimer:

  Reused without explicit authorization under blanket
  permission granted for all Risks-Forum Digest materials.
  The author(s), the RISKS moderator, and the ACM have no
  connection with this reuse.
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20000527064423/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20000527064423/mailto:webmaster@somewhere.com). |