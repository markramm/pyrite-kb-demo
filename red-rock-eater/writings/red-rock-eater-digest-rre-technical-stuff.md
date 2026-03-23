---
id: red-rock-eater-digest-rre-technical-stuff
title: Red Rock Eater Digest - RRE technical stuff
type: writing
writing_type: rre-post
url: http://commons.somewhere.com:80/rre/2000/RRE.RRE.technical.stuff.html
importance: 6
research_status: partial
tags:
  - cryptography
  - law
  - military
  - privacy
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/2000/RRE.RRE.technical.stuff.html

## Content

|  |  |
| --- | --- |
| [**Red Rock Eater Digest**](https://web.archive.org/web/20010124151500/http://commons.somewhere.com/rre/) | **Most Recent Article: Tue, 23 Jan 2001** |

```
I have enclosed a few notes from RRE subscribers on technical issues
relating to the list:
 
(1) A method for Eudora users to forward RRE messages without using
the antisocial "redirect" command or generating those annoying ">"
indentations for the forwarded message.  All Eudora users should find
this useful.

For those who don't know why "redirect" is antisocial:

  http://dlis.gseis.ucla.edu/people/pagre/rre-faq.html#redirect

Praise, by the way, to RRE's many Eudora users, who have been very good
in the last year about not using "redirect" to forward RRE messages.

(2) A perl script that converts my plain-text "notes and recommendations"
messages into more-readable html files.  Why don't I use HTML myself?
RRE has a low-tech, common-denominator policy to ensure that nobody will
have to contend with weird markup codes that aren't compatible with their
particular mail-reading program.  This perl script, whose author admits
that it is a total kludge, is for committed perl hackers only, obviously.

(3) Some notes on XEmacs, for Emacs people only.

I have deleted the authors' identities from each of these notes, so I
hope that they are clear enough.  I am unable to answer questions about
any of them.

Let me also confess a conspiracy that I chickened out on.  An RRE reader
brought my attention to anybirthday.com, a Web site that lists birthdays
for a large percentage of Americans (and others for all I know).  Neither
of us was happy about this site from a privacy perspective, and so my
correspondent wrote me a tcl script that would run straight through the
RRE subscriber list, do an anybirthday.com lookup on every name, and send
the results to the associated e-mail address, together with instructions
about how to opt out of the anybirthday.com database.  I figured that
this would be an opportunity for me to learn tcl as well as pull a good
stunt.  But, as I say, I chickened out.  There were just too many ways
that it might have gone wrong.  If anybody is interested (in, say, the
next couple of weeks) I can send you the tar file for the script and
associated documentation (though not, of course, the RRE subscriber list).

Phil

---

This message was forwarded through the Red Rock Eater News Service (RRE).
You are welcome to send the message along to others but please do not use
the "redirect" option.  For information about RRE, including instructions
for (un)subscribing, see http://dlis.gseis.ucla.edu/people/pagre/rre.html

---

Here's something for your FAQ that might help a bit with the redirect
problem:

Eudora users who wish to forward without quotes can use 
Edit->Text->Unquote on the forwarded text.

>I don't use Eudora.  Can you explain that suggestion just a little
>bit more?  By "without quotes" do you mean without those > indentations?

Yes, without ">" (as seen in your paragraph above, presumably).

Eudora users may use "redirect" because they don't want the forwarded 
message to have ">"'s. But they can easily remove the ">"s in a 
normally forwarded message:

In Eudora, choose the Forward command. Click in the body and type 
control-a or command-a to select all the text. Then choose the 
"Unquote" command from the Edit menu, Text submenu. (I'm on Mac, but 
Windows should be the same.)

Eudora includes the header of the forwarded message in the new body, 
so it's fairly clear the message is forwarded.

I'm not sure how far back this command goes - at least to Eudora 4 
(current is Eudora 5).

> How does one invoke this script under Unix?

One places it in a file 'agrify', makes it executable (chmod u+x
agrify), and executes it with a [[RRE message -PA]]] either on its
standard input or in a filename named on the command line.  One may
want to redirect its output to a file.  (All this is assuming Perl
is installed in /usr/bin/perl on your system.  If not, you can run
it with 'perl agrify filename' rather than './agrify filename'.)

I hope you don't find the use of your name in this manner offensive.

Here's an even kludgier version that handles blockquotes and '**'
section separators as well, and has slightly fine-tuned thresholds for
some things:

#!/usr/bin/perl -w
use strict;

# Philip Agre likes to write documents in ASCII.  This program does
# some heuristics to try to convert his ASCII documents to HTML.
# It's mostly a collection of crude kludges, and it's possible for it to
# produce stuff that's not valid HTML.  (Normally it produces valid HTML 
# 4.0 Transitional.)

my $between_paras = 1;
my $in_ul = 0;
my $in_ol = 0;
my $in_bq = 0;  # blockquote
my $did_title = 0;
my $was_short_line = 0;
my $length = undef;
sub end_ul {
    if ($in_ul) {
        print "</ul>\n";
        $in_ul = 0;
    }
}

sub end_ol {
    if ($in_ol) {
        print "</ol>\n";
        $in_ol = 0;
    }
}

while (<>) {
    if (/^$/) {
        $between_paras = 1;
    } elsif (/^\s*\*\*\s*$/) { # Phil's new '**' section divider
        end_ul; end_ol; print "<hr>\n"; $between_paras = 1;
    } else {
        # first nonblank line is the title; not perfect, but right sometimes
        if (not $did_title) {
            print '<!DOCTYPE HTML PUBLIC ',
                '"-//W3C//DTD HTML 4.0 Transitional//EN" ',
                '"http://www.w3.org/TR/REC-html40/loose.dtd">', "\n",
                "<html><head><title>$_</title></head>\n";
            print '<body bgcolor="white"><h1>', $_, "</h1>";
            $did_title = 1;
        } else {
	    # get length before munging
	    my $last_line_length = $length;
            $length = length();
            if ($between_paras) {
                # now we start a paragraph
		if (s/^\s*\*\s*//) {
                    end_ol;
                    if (not $in_ul) {
                        print "<ul>\n";
                        $in_ul = 1;
                    }
                    print "<li> ";
		    $between_paras = 0;
                } elsif (s/^\s*\((\d+)\)\s*//) {
                    end_ul;
                    if (not $in_ol) {
                        print "<ol>\n";
                        $in_ol = 1;
                    }
                    print "<li> ";
		    $between_paras = 0;
		} elsif (s|^\s*//||) {  # Phil uses // to start section titles
		    end_ol;
		    end_ul;
		    print "</blockquote>" if $in_bq;
		    $in_bq = 0;
		    $_ = "<h2>$_</h2>\n";
		    $between_paras = 1;  # the title is one line long
                } else {
                    end_ol;
                    end_ul;
		    # If Phil used multiple levels of indents, or if he
		    # indented the first lines of unindented paragraphs,
		    # this would work badly.  As it is, it sometimes 
		    # identifies things as blockquotes that are just indented
		    # paragraphs, but that's OK --- browsers render 
		    # blockquotes as indented paragraphs.
		    if (/^\s{2,}/) {
			print "<blockquote>" if not $in_bq;
			$in_bq = 1;
		    } else {
			print "</blockquote>" if $in_bq;
			$in_bq = 0;
		    }
                    print "<p>\n";
                    $between_paras = 0;
                }
            } else {
                # inside a paragraph, if the previous line
                # was "short", print a line break
                if ($was_short_line) {
                    print qq(<br len="$last_line_length">);  # invalid HTML
                    # print '<br>';
                }
            }
            # 57 seems to work OK for Phil's text; there really
            # are 57-char-wide lines in Phil's text sometimes.
            # this includes the \n.  Increasing this to 59 reduces
	    # the number of unintentional joins, but adds some accidental
	    # splits.  Perhaps we should look at text a paragraph at a time
	    # rather than a line at a time?
            $was_short_line = ($length < 57);
            s/\*(.*?)\*/<i>$1<\/i>/g;  # this is italics
            s/^>(>*From)/$1/;          # mailers mangle things
            # URLs become links; we assume they don't end with 
            # . or ,  --- although it's legal for them to do so, it
            # is unusual, but it is common for unnecessary , and .
            # characters to be appended.
            s|(http://[^ \n>")]*[^ \n.,>")])|<a href="$1">$1</a>|g;
            print;
        }
    }
}

end_ul;
end_ol;
print "</body></html>\n";

I know this is probably a closed issue, but I thought I'd alert you to
the fact that XEmacs now has (unofficial) support for NT in the source
distribution (it works great, especially in conjunction with Cygnus's
cygwin, a port of the core GNU utilities to Windows 95/98/ME/NT/2000).
They've been working on it for a couple years now, and while it's
not as robust as the Unix versions, it's more than usable enough for
prolific everyday use.

A more tentative project is http://my.ispchannel.com/~pjarvis/xemacs.html,
a new Macintosh port of XEmacs 19.14. It's got a ton of idiosyncracies
(it's undumped, which means that every time you run it, it has to
bootstrap all of the elisp code which is normally compiled into the
executable; it garbage collects a lot unless you give it a hefty
memory partition -- I give it 16MB; its font support is kludgy, and,
perhaps most importantly (aagh) there's no meta-key support right
now), but it works. The distribution even contains some small number
of Unix tools -- sh, rm, rmdir, mkdir -- which means that shell-mode
works. It's also built against Apple's Carbon libraries, which
means that the port should be available for MacOS X as soon as it's
released.

The reason GNU Emacs is so rarely available for the Mac is, I think,
Richard Stallman's historical reluctance to have anything to do with
the Macintosh.  He's got an amazing ability to fight battles that
everyone else stopped caring about long ago, and in this day and age
of ubiquitous and warring GUIs, I would think Apple's once-upon-a-time
proprietary attitude towards GUIs would be less important. I suppose
the great thing about Stallman is that he'll fight your battles for
you whether you want him to or not, and a certain degree of respect is
due to his kind of dogged ideological persistence, grounded as it is
within egalitarian principles.

The XEmacs community, on the other hand, couldn't care less, and some
of them probably even tangentially favor a Mac version of the port.
I expect we'll see a fuller port after MacOS X has been available for
a while, as it has much better support for the sorts of functionality
XEmacs requires.

So, anyway, if you want a useful port of Emacs for recent versions
of MacOS, don't want to subvert the Macintosh's delightful user
experience (I'm a die-hard Linux fan (if not advocate), but I also
love my PowerBook -- especially because it runs MacOS), and are
willing to put up with a few rough edges, I suggest you investigate
"pjarvis"'s port.

I myself tend to use XEmacs to hack code; BBEdit, Alpha, Pepper, and
Dreamweaver to hack HTML; and WriteNow to hack fiction (at work I
use XEmacs for NT and UltraEdit, both fine options; when I'm being a
sysadmin or Unix developer I use XEmacs and vi[m]). I figure that in
a world where there are so many great tools available for manipulating
words, I ought to use whatever's most appropriate for the job. I'm an
editor junkie.

end
```

|  |
| --- |
| **[ProcessTree Network](https://web.archive.org/web/20010124151500/http://www.processtree.com/?sponsor=23069)** TM  For-pay Internet distributed processing. |
| Advertising helps support hosting Red Rock Eater Digest @ The Commons. Advertisers are not associated with the list owner. If you have any comments about the advertising, please direct them to the [Webmaster @ The Commons](https://web.archive.org/web/20010124151500/mailto:webmaster@somewhere.com). |