<h2>Project name changed to VEHICLE and hosting changed to GitHub</h2>
The name of the ria-scip project was <b>changed</b> to <a href="https://github.com/hacktics/vehicle"><b>VEHICLE</b></a>, and the project is now hosted in it's new <a href="https://github.com/hacktics/vehicle">github repository</a>.<br><br>
An OWASP ZAP extension for security assessments of rich internet applications (RIA platforms) and modern web application frameworks (MWAF), including ASP.net and Mono.

<font size="5"><b>SCIP - Server Control Invisibility Purge!</b></font><br><br>
SCIP is a RIA / MWAF assessment platform, built as an extension for <a href="http://code.google.com/p/zaproxy/" target="_blank">OWASP Zed Attack Proxy (ZAP)</a>.<br>

Developed by <a href="http://www.hacktics.com" target="_blank">Hacktics ASC</a><br>
<a href="http://www.hacktics.com" target="_blank"><img src="http://diviner.googlecode.com/files/hacktics_logo.jpg" /></a><br>

SCIP is a unique platform that enables penetration testers to abuse configuration and programming flaws in modern web application frameworks (specifically in ASP.net and Mono), and execute dormant events of invisible, disabled and commented server web conrols.

<b>Requirements:</b>
<LI> SCIP requires Java <u>1.7.x</u>, and was tested with ZAP v.2.x.
<LI> Verify that ZAP proxy is executed using Java 1.7.x, prior to running the installer.
<br>

<font size="5"><b>How Does it Work?</b></font><br>
SCIP can locate insecure ASP.net configuration, as well as locate traces of invisible, disabled and commented controls and events.
It can then be used to enumerate invisible controls, and execute dormant events of server controls by forging a valid postback call (invisible controls without event validation or disabled & commented controls in any scenario),  or by reconstructing the viewstate and eventvalidation fields of invisible controls (in  case the eventvalidation is on but the MAC is off).

SCIP also provides a manual interface for performing additional RIA/ASP.net targeted attacks such as reusing hijacked viewstate/eventvalidation fields, reconstructing viewstate fields after content alteration/parameter tampering, etc.
<p><img src="http://ria-scip.googlecode.com/svn/wiki/images/SCIP-RIA Event Enumerator.png" /></p>
<hr/>
<p><font size="5"><b>SCIP Demo - Event Execution of Invisible Controls</b></font></p>
<wiki:video width="560" height="315" url="http://www.youtube.com/watch?v=0c8Y7TlXcWs"/>
<hr/>
<font size="5"><b>Quickstart</b></font><br>
SCIP can currently be used by right-clicking on any ASP.net page in ZAP's treeview. <br>
Currently supports ASP.net, while the next release will support mono and additional* technologies.

<font size="5"><b>Developers</b></font><br>
RIA-SCIP is developed and maintained by <a href="https://twitter.com/nashcontrol">Alex Mor</a>, <a href="https://twitter.com/sectooladdict/">Shay Chen</a> and <a href="https://twitter.com/nivselatwit">Niv Sela</a> .

<font size="5"><b>Features</b></font><br>

<table border="0">
<tr><td><b><u>Event Execution Features</u></b>
<tr><td valign="top">
<LI><I>Event Execution of Disabled / Commented Controls </I>
<LI><I>Event Execution of Invisible Controls (When the Event Validation is OFF)</I>
<LI><I>Event Execution of Invisible Controls (When the Viewstate MAC is OFF)</I>
<LI><I>Manual Event Execution of Optional Events (MAC/Validation is OFF)</I>

<tr><td><b><u>Additional Features</u></b>
<tr><td valign="top">
<LI><I>Error-Based Control Name Enumeration </I>
<LI><I>Viewstate/EventValidation Reconstruction (Assist in Control Value Manipulation)</I>

<tr><td><b><u>Technology Support</u></b>
<tr><td valign="top">
<LI><I>ASP.net postbacks / Viewstate 2</I>
<LI><I>Upcoming: Support for Mono / Callbacks / Viewstate 1</I>

<tr><td><b><u>Integration Support</u></b>
<tr><td valign="top">
<LI><I>Integration With ZAP's 'Resend Request' Feature</I>
<LI><I>Upcoming: Integration With Diviner's Diff Method to support Blind Event Enumeration</I>
<br>
