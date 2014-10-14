# Overview

"A Zest of Python" is a library for working wth the [Zest Domain Specific Language](https://developer.mozilla.org/en-US/docs/Zest). Zest itself is a DSL that can be
used for scripting security testing; the reference implementation is written in Java, and is part of OWASP's Zed Attack Proxy (ZAP).

# Rationale

 I've wanted a format that I could use for storing & replaying security tests, esp. as a part of another project I'm working on for scanning browser's history
files in a fashion similar to the passive scanner in tools like Burp or ZAP. Zest fits the bill nicely: it's a relatively easy format to parse (it uses JSON
internally), has decent support for features that matter to security and QA testers alike, and is relatively well documented. In addition to that, it supports
storing request & response objects, timing, size, and the like. So, not only can it be used for storing requests, but it can be used for replaying them in
future tests. 

 ... which is all fine and good save for that I often use Python for client projects, and Zest is currently implemented in Java (tehre is a JS implementation
as well). A Zest of Python seeks to fix that by providing a useable & pythonic interface to Zest, replete with the usual tests & documentation.
