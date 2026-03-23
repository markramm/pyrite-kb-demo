---
id: red-rock-eater-digest-building-characters-a-brief-history-of-the-web-war
title: "Red Rock Eater Digest - Building Characters: A Brief History of the Web War"
type: writing
writing_type: rre-post
url: "http://commons.somewhere.com:80/rre/2000/RRE.Building.Characters..html"
importance: 6
research_status: partial
tags:
  - cognitive-science
  - commerce
  - cryptography
  - international
  - media
  - military
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/2000/RRE.Building.Characters..html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20001215171200/http://commons.somewhere.com/rre/) | **Most Recent Article: Thu, 14 Dec 2000** |

```
---

This message was forwarded through the Red Rock Eater News Service (RRE).
You are welcome to send the message along to others but please do not use
the "redirect" option.  For information about RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html

---

Date: Mon, 20 Mar 2000 21:30:00 -0800
From: TidBITS Editors <editors@tidbits.com>
Subject: TidBITS#522/20-Mar-00
To: tidbits@tidbits.com (TidBITS Distribution)

TidBITS#522/20-Mar-00

---

[...]

Building Characters: A Brief History of the Web War

---

   by Geoff Duncan <geoff@tidbits.com>

   A little over a year ago in TidBITS-467, I wrote about some
   historical and technical reasons why text on Web pages can be
   illegibly small when viewed on a Macintosh - especially pages
   designed by and for Windows users.

<http://db.tidbits.com/getbits.acgi?tbart=05284>

   The principles and problems outlined in that article are as true
   today as they were then, but new Internet standards and a new
   generation of Web browsers are beginning to offer possible
   solutions to both Web users and Web authors. This article examines
   some of the history of text presentation on the Web; future
   installments will examine new Web standards and new browser
   capabilities, plus offer concrete advice on preparing platform-
   friendly Web content.

**Text Rules**-- Let's face it: much of the information we use on
   our computers is in the form of text. We write and edit documents,
   send and receive email, and browse and create Web pages. Compared
   to images, movies, and audio, text is a simple data type that
   crosses between platforms and operating systems with relative
   ease. So why does text so often display badly, especially on the
   Web? Why are we constantly fussing with window sizes, font sizes,
   and browser preferences when all we want to do is read text?

   In a nutshell, text differs between operating systems mainly
   because each operating system makes a different assumption about
   how pixels on a display translate to physical measurements. The
   Mac OS assumes a resolution of 72 dots per inch (dpi) regardless
   of the physical resolution of a display device, and there's no way
   to change this setting. In contrast, Windows assumes a resolution
   of 96 dpi (or 120 dpi using Large Fonts), and this setting can be
   changed arbitrarily under recent versions of Windows. Unix systems
   typically use resolutions from 75 to 100 dpi and can usually be
   configured by the user.

   The difference in assumed resolutions determines how many pixels
   the computer uses to render text. Assuming a point is 1/72nd of an
   inch, the Mac OS will use 12 pixels to render 12 point type, while
   a Windows system will typically use 16 pixels. If you display
   these characters side by side on the same display, the Windows
   characters will look 33 percent larger than the Macintosh
   characters.

<http://www.tidbits.com/resources/522/mac-win-text.html>

   Using a larger number of pixels to render text has many
   implications, but here are two key concepts to keep at the back of
   your mind:- Text is rendered with more accuracy, so important features in a
     typeface (serifs, special symbols, relationships and spacing
     between letters, etc.) are more likely to be preserved or
     presented accurately.- Fewer characters fit into an arbitrary region of your screen,
       like a Web browser window. Fewer characters convey less
       information to a user, so that region can be described as having a
       lower "information density" than it would if its text were
       rendered using fewer pixels.

    **Casualties of War** -- Believe it or not, these platform-related
       differences in text rendering didn't go unnoticed in the Web
       development community - in fact, they substantially predate the
       World Wide Web. If the issue is so old, why hasn't it been solved
       by now?

       The answer is complicated. Remember one truth that has been
       frustrating many Web authors for years: HTML wasn't meant to
       describe the physical or typographical presentation of a document;
       rather, HTML describes the structure of a document - which items
       are headings, which items are links, which items are lists, and so
       on - in a platform-independent manner. Decisions about a
       document's presentation were left up to individual Web browsers
       (or, more properly, "user agents"). They were supposed to look at
       the structure of the document and present it on their particular
       platform in a way that made sense.

       This is where the forces of the computing industry reared their
       ugly heads. For years, operating systems tried to present users
       with a WYSIWYG world - What You See Is What You Get. Along with
       graphical user interfaces, WYSIWYG was one of the attractions that
       brought people to personal computing. HTML's abstract approach
       frustrated computer users of all stripes - personal, professional,
       corporate, and others - who expected WYSIWYG. Those expectations
       morphed into strident demands as the Web became a vehicle for
       publishing, then commerce.

       When software developers hear strident demands from customers,
       those demands are translated directly to the phrase "market
       opportunity." Browser developers rapidly rolled out non-standard
       HTML tags which almost invariably described the presentation of a
       document rather than its structure. Netscape quickly muddied the
       water with CENTER tags, alignment attributes, colors, and ways to
       specify text wrapping. Web "designers" began publishing books on
       wringing WYSIWYG-like behaviors out of the browsers of the day (at
       best advocating extensive use of tables; at worst promoting
       "spacer GIFs" and violating virtually every principle of an
       adaptive, cross-platform technology). Although late to the game,
       Microsoft jumped in with contributions like MARQUEE, background
       sounds, and ways to slice and dice border colors. Simultaneously,
       a flurry of graphical HTML editors appeared, often producing
       markup that looked like the peckings of a thousand typewriter-
       equipped simians. And, of course, eventually Netscape went hog-
       wild, unleashing font tags, MULTICOL, the SPACER tag, and a
       "layers" technology that allowed arbitrary onscreen placement of
       objects.

       In short, the browser wars were well underway, and much of the
       artillery was aimed directly at the core principles of HTML.
       Although folks at the World Wide Web Consortium (W3C) tried to
       keep a rein on things, 1996's HTML 3.2 specification ended up
       being a mishmash compromise between the abstract structural
       concepts of HTML and the presentation demands of an explosively
       growing industry. And nobody was happy about it.

    <http://www.w3.org/TR/REC-html32.html>

    **Return to Standards** -- As the Internet exploded, however, a
       funny thing happened. Although the main devices using the Web
       continued to be personal computers with graphical interfaces,
       alternatives methods of accessing the Web began to multiply.
       Text-only browsers not only survived but gained popularity as
       power users became disgusted with long download times and
       pointless graphics. WebTV promised to turn any television into a
       limited Internet appliance, and folks connected PDAs like Apple's
       Newton to the Web, not to mention Palm devices and cellular
       telephones. Similarly, ever-present accessibility issues - for
       users who are visually impaired, color blind, or unable to use
       traditional computers - weren't being served by the combative,
       proprietary course of HTML development. Suddenly the structure
       of an HTML document was becoming important again, since details of
       a document's presentation were irrelevant to these devices. After
       all, what's a black-and-white Palm device with a 160-by-160 screen
       size going to do with an HTML table which insists it must be fire
       engine red and 600 pixels across?

       At the same time, the major browser vendors were hit with a
       backlash because their incompatible and often ill-conceived HTML
       extensions created confusion and impediments for both Web users
       and authors. Conformance to standards became a rallying cry, and
       standards-oriented efforts like Lynx and Opera gained substantial
       credibility (as has the Mac OS newcomer iCab). It didn't take long
       for the heavyweights to see the light, with Netscape spinning its
       Web browser development off to the Mozilla open source project,
       and Microsoft pledging to toe the line on standards, in part due
       to pressure from the ongoing federal antitrust case against the
       company.

    <http://lynx.browser.org/>
    <http://www.opera.com/>
    <http://db.tidbits.com/getbits.acgi?nbart=04593>
    <http://www.icab.de/>
    <http://www.mozilla.org/>
    <http://db.tidbits.com/getbits.acgi?tbser=1152>

       Nonetheless, demands that Web authors be able to indicate a
       document's presentation in addition to its structure weren't going
       to go away. The cat was already out of the bag, with hundreds of
       thousands of existing Web sites and millions of existing Web
       users, and more of each appearing every second. What could be
       done?

    **The Cascade Effect** -- Cascading Style Sheets, or CSS, offer a
       solution to the structure-and-presentation dilemma. CSS had been
       percolating quietly within the W3C during the browser wars and was
       adopted as a recommendation in late 1996, although no mainstream
       tools supported it. The basic idea behind CSS is to separate
       formatting information - positioning, sizing, margins, leading,
       type faces, and more - from the structure of a document, as
       represented by HTML.

    <http://www.w3.org/Style/CSS/>

       Style sheets may be integrated into an HTML document (using the
       STYLE tag) or exist as separately linked external files
       (convenient for multiple documents which share styles).
       Conceptually, CSS has similarities to styles used by a word
       processors: each CSS style, or rule, applies certain formatting
       characteristics to items. For instance:

        P { color: red; font-family: Palatino, serif; }

       Here, P is called a selector, and refers to any <P> tags in the
       current HTML document. The information in curly braces is called a
       declaration, and specifies the particular properties and values
       for a CSS rule. This rule says that the text within all <P> tags
       in the current HTML document should be presented in red,
       preferably using the Palatino font. If Palatino is not available,
       paragraphs should be displayed using the browser's default serif
       font. Using CSS, you can define a wide variety of display and
       presentation characteristics for any valid HTML tag in a document
    * - including the document body, heading tags, table cells, links,
      and more - specific tags, or even unique instances of a tag.For now, there are three important things to remember about CSS:- Unlike styles in a word processor, the display characteristics
         for any item are determined by the cascade, or the combination
         of multiple style sheets. At a basic level, at least three style
         sheets are always in play - the current document's, the user's,
         and the browser's default. Although a document's rules usually
         take precedence, they can be overridden by user or browser rules.
         Thus, in theory, a user can define his or her own style sheet so
         no text is ever displayed below 14 pixels in size, for example, no
         matter what size the document may specify for text sizing. This
         gives documents the capability to request particular formatting,
         while still accommodating the specific needs of users. Basically,
         documents suggest how they should be formatted, rather than
         demanding a particular presentation.- Style sheets are the recommended method to control virtually all
           document layout and presentation in the current HTML 4 standard,
           although HTML 4.0 Transitional still includes most of the
           presentation attributes from HTML 3.2, such as specifying some
           objects' widths and colors. The second version of CSS, called
           CSS2, was adopted as a W3C recommendation in mid-1998, and
           expanded on the capabilities of CSS1 in significant ways.

        <http://www.w3.org/TR/html401/>- Since CSS covers a wide range of formatting capabilities, it is
             extraordinarily complex to implement. As of this writing, no
             released browser fully supports CSS1 or CSS2, in part due to the
             fallout from the heated browser wars in the late 1990s. Some
             browsers support useful subsets of CSS1 and CSS2 - most notably
             the current versions of Microsoft Internet Explorer and Opera -
             although there are a myriad of significant bugs in current and
             older browsers. Netscape Communicator/Navigator 4.x makes no
             claims about supporting any aspect of CSS; instead, CSS support
             has been relegated to the Mozilla open source project. Some style
             sheets can influence the display of Web pages in current versions
             of Netscape, but more often than not the behaviors are incomplete
             or completely incorrect. This spotty support vastly complicates
             the use and deployment of style sheets.

          **To Be Continued** -- Wait! What does all this have to do with
             how many pixels are used to draw text on the Macintosh screen? How
             does any of this technology improve your Web browsing experience,
             or let you create friendlier Web pages? Those and other mysteries
             will be revealed in our next installment.

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
            And: <ftp://ftp.tidbits.com/issues/>
            Full text searching available at: <http://www.tidbits.com/search/>
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20001215171200/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20001215171200/mailto:webmaster@somewhere.com). |