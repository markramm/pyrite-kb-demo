---
id: red-rock-eater-digest
title: Red Rock Eater Digest
type: writing
writing_type: rre-post
date: 2004-06-29
url: http://web.archive.org/web/20040704074317/commons.somewhere.com/rre/
coauthors: []
key_concepts: []
importance: 1
research_status: partial
tags:
  - administrative
  - index
  - rre-post
---




## Source

Automatically imported from: http://web.archive.org/web/20040704074317/commons.somewhere.com/rre/

## Content

//<![CDATA[
var \_\_wm = (function(){
var wbPrefix = "/web/";
var wbCurrentUrl = "https://web.archive.org/web/20150123051408/http://commons.somewhere.com/rre";
var firstYear = 1996;
var imgWidth = 500,imgHeight = 27;
var yearImgWidth = 25,monthImgWidth = 2;
var displayDay = "4";
var displayMonth = "Jul";
var displayYear = "2004";
var prettyMonths = ["Jan","Feb","Mar","Apr","May","Jun","Jul","Aug","Sep","Oct","Nov","Dec"];
var $D=document,$=function(n){return document.getElementById(n)};
var trackerVal,curYear = -1,curMonth = -1;
var yearTracker,monthTracker;
function showTrackers(val) {
if (val===trackerVal) return;
var $ipp=$("wm-ipp");
var $y=$("displayYearEl"),$m=$("displayMonthEl"),$d=$("displayDayEl");
if (val) {
$ipp.className="hi";
} else {
$ipp.className="";
$y.innerHTML=displayYear;$m.innerHTML=displayMonth;$d.innerHTML=displayDay;
}
yearTracker.style.display=val?"inline":"none";
monthTracker.style.display=val?"inline":"none";
trackerVal = val;
}
function getElementX2(obj) {
var $e=jQuery(obj);
return (typeof $e=="undefined"||typeof $e.offset=="undefined")?
getElementX(obj):Math.round($e.offset().left);
}
function trackMouseMove(event,element) {
var eventX = getEventX(event);
var elementX = getElementX2(element);
var xOff = Math.min(Math.max(0, eventX - elementX),imgWidth);
var monthOff = xOff % yearImgWidth;
var year = Math.floor(xOff / yearImgWidth);
var monthOfYear = Math.min(11,Math.floor(monthOff / monthImgWidth));
// 1 extra border pixel at the left edge of the year:
var month = (year \* 12) + monthOfYear;
var day = monthOff % 2==1?15:1;
var dateString = zeroPad(year + firstYear) + zeroPad(monthOfYear+1,2) +
zeroPad(day,2) + "000000";
$("displayYearEl").innerHTML=year+firstYear;
$("displayMonthEl").innerHTML=prettyMonths[monthOfYear];
// looks too jarring when it changes..
//$("displayDayEl").innerHTML=zeroPad(day,2);
var url = wbPrefix + dateString + '/' + wbCurrentUrl;
$("wm-graph-anchor").href=url;
if(curYear != year) {
var yrOff = year \* yearImgWidth;
yearTracker.style.left = yrOff + "px";
curYear = year;
}
if(curMonth != month) {
var mtOff = year + (month \* monthImgWidth) + 1;
monthTracker.style.left = mtOff + "px";
curMonth = month;
}
}
function hideToolbar() {
$("wm-ipp").style.display="none";
}
function bootstrap() {
var $spk=$("wm-ipp-sparkline");
yearTracker=$D.createElement('div');
yearTracker.className='yt';
with(yearTracker.style){
display='none';width=yearImgWidth+"px";height=imgHeight+"px";
}
monthTracker=$D.createElement('div');
monthTracker.className='mt';
with(monthTracker.style){
display='none';width=monthImgWidth+"px";height=imgHeight+"px";
}
$spk.appendChild(yearTracker);
$spk.appendChild(monthTracker);
var $ipp=$("wm-ipp");
$ipp&&disclaimElement($ipp);
}
return{st:showTrackers,mv:trackMouseMove,h:hideToolbar,bt:bootstrap};
})();//]]>

body {
margin-top:0 !important;
padding-top:0 !important;
min-width:800px !important;
}
\_\_wm.bt();

rnum=Math.round(Math.random() \* 100000);
document.write('<scr'+'ipt src="/web/20040704074317/http://www.burstnet.com/cgi-bin/ads/ad8070a.cgi/v=2.0S/sz=468x60A|728x90A/'+rnum+'/NI/RETURN-CODE/JS/"></scr'+'ipt>');

# Red Rock Eater Digest

> The RRE News Service is a mailing list organized by Phil Agre. Topics usually concern the social and political aspects of computing and networking. The last issue was released on Tuesday, June 29 2004, and updates normally
> come out five times a week.
> Questions and comments regarding the content of this zine should be directed to
> Phil Agre.
> Further information about Red Rock Eater Digest may be found at
> Phil Agre's [personal site](/web/20150123051408/http://web.archive.org/web/20040704074317/http://dlis.gseis.ucla.edu/pagre/) or at
> the [official web site](/web/20150123051408/http://web.archive.org/web/20040704074317/http://dlis.gseis.ucla.edu/people/pagre/rre.html).
>
> |  |  |  |  |  |
> | --- | --- | --- | --- | --- |
> | |  |  | | --- | --- | | Keywords: |  | | *Search matches all keywords entered, but it is not currently a full-text  search, only a partial list of keywords is searched.* | | |

|  |  |  |  |
| --- | --- | --- | --- |
| **2004** | **Jun** | | |
|  | **29** | [pointers](2004/RRE.pointers2.html) | |
|  | **May** | | |
|  | **4** | [pointers](2004/RRE.pointers1.html) | |
|  | **Mar** | | |
|  | **24** | [pointers](2004/RRE.pointers.html) | |
| **2003** | **Aug** | | |
|  | **18** | [Vaclav Havel](2003/RRE.Vaclav.Havel.html) | |
|  | **May** | | |
|  | **19** | [The Practical Republic](2003/RRE.The.Practical.Republ.html) | |
|  | **15** | [reading list](2003/RRE.reading.list3.html) | |
|  | **12** | [reading list](2003/RRE.reading.list2.html) | |
|  | **9** | [reading list](2003/RRE.reading.list1.html) | |
|  |  | [reading list](2003/RRE.reading.list.html) | |
|  | **5** | [what I'm interested in, part 26](2003/RRE.what.I.m.interested..html) | |
|  |  | [cheap pens](2003/RRE.cheap.pens.html) | |
|  |  | [pointers](2003/RRE.pointers3.html) | |
|  | **Apr** | | |
|  | **28** | [quiet](2003/RRE.quiet.html) | |
|  | **Feb** | | |
|  | **8** | [pointers](2003/RRE.pointers2.html) | |
|  | **Jan** | | |
|  | **23** | [pointers](2003/RRE.pointers1.html) | |
|  | **10** | [pointers](2003/RRE.pointers.html) | |
| **2002** | **Dec** | | |
|  | **24** | [pointers](2002/RRE.pointers126.html) | |
|  | **16** | [pointers](2002/RRE.pointers125.html) | |
|  | **10** | [pointers](2002/RRE.pointers124.html) | |
|  | **1** | [pointers](2002/RRE.pointers123.html) | |

  
**2002 [Nov](?Year=2002&Month=11&Search=#Focus)**
**[Oct](?Year=2002&Month=10&Search=#Focus)**
**[Sep](?Year=2002&Month=9&Search=#Focus)**
**[Aug](?Year=2002&Month=8&Search=#Focus)**
**[Jul](?Year=2002&Month=7&Search=#Focus)**
**[Jun](?Year=2002&Month=6&Search=#Focus)**
**[May](?Year=2002&Month=5&Search=#Focus)**
**[Apr](?Year=2002&Month=4&Search=#Focus)**
**[Mar](?Year=2002&Month=3&Search=#Focus)**
**[Feb](?Year=2002&Month=2&Search=#Focus)**
**[Jan](?Year=2002&Month=1&Search=#Focus)**
  
**[2001](?Year=2001&Search=#Focus)**
  
**[2000](?Year=2000&Search=#Focus)**
  
**[1999](?Year=1999&Search=#Focus)**
  
**[1998](?Year=1998&Search=#Focus)**
  
**[1997](?Year=1997&Search=#Focus)**
  
**[1996](?Year=1996&Search=#Focus)**
  
**[1995](?Year=1995&Search=#Focus)**
  
**[1994](?Year=1994&Search=#Focus)**

Questions regarding [The Commons](/web/20150123051408/http://web.archive.org/web/20040704074317/http://commons.somewhere.com/)
or [Somewhere.Com, LLC](/web/20150123051408/http://web.archive.org/web/20040704074317/http://www.somewhere.com/) should be directed
to [Kee Hinckley](https://web.archive.org/web/20150123051408/mailto:webmaster%40somewhere.com?Subject=Red Rock Eater Digest @ The Commons).
Do you have a mailing list you'd like to see us carry? Let us know! And see the
other lists we carry on [The Commons](/web/20150123051408/http://web.archive.org/web/20040704074317/http://commons.somewhere.com/).