+++
date = "2016-05-27T12:08:01-07:00"
draft = true
link = "https://www.ampproject.org/docs/guides/validate.html"
tags = ["AMP", "XHTML"]
title = "Google AMP and XHTML"
topics = ["Web"]

+++

I've been pushing myself to learn a little bit about Google's Accelerated Mobile Pages (AMP) initiative. My initial reaction is mixed but one particular part seems misguided:

> If the AMP validation service detects that there’s something wrong with your page, it won’t get discovered and distributed by third party websites and won’t appear in the Google AMP Cache.

In other words you get the same "yellow screen of death" that browsers would present to befuddled users in the earl 2000s when it became mildly fashionable to serve HTML web content as `application/xhtml+xml`.

I've been around the Internet a block a few times and have yet to see a solid counterargument to [Postel's Law][1]:

> be conservative in what you do, be liberal in what you accept from others

[1]: http://bitworking.org/news/There_are_no_exceptions_to_Postel_s_Law_
