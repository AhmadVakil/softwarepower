---
title: BBQSQL - A Blind SQL Injection Exploitation Tool
date: 2020-10-10
category:
  - Learning
comments: true
---
{% raw %}
<div class="l-section-h i-cf"><h2>Vulnerability Analysis - BBQSQL Package Description</h2>
<p style="text-align: justify;">Blind SQL injection can be a pain to exploit. When the available tools work they work well, but when they don’t you have to write something custom. This is time-consuming and tedious. BBQSQL can help you address those issues.</p>
<p>BBQSQL is a blind SQL injection framework written in Python. It is extremely useful when attacking tricky SQL injection vulnerabilities. BBQSQL is also a semi-automatic tool, allowing quite a bit of customization for those hard to trigger SQL injection findings. The tool is built to be database agnostic and is extremely versatile. It also has an intuitive UI to make setting up attacks much easier. Python gevent is also implemented, making BBQSQL extremely fast.</p>
<p>Similar to other SQL injection tools you provide certain request information.</p>
<p>Must provide the usual information:</p>
<ul>
<li>URL</li>
<li>HTTP Method</li>
<li>Headers</li>
<li>Cookies</li>
<li>Encoding methods</li>
<li>Redirect behavior</li>
<li>Files</li>
<li>HTTP Auth</li>
<li>Proxies</li>
</ul>
<p>Then specify where the injection is going and what syntax we are injecting.</p>
<p>Source: https://github.com/Neohapsis/bbqsql/<br>
<a href="https://github.com/Neohapsis/bbqsql/" variation="deepblue" target="_blank" rel="nofollow">BBQSQL Homepage</a> | <a href="https://gitlab.com/kalilinux/packages/bbqsql" variation="deepblue" target="_blank" rel="nofollow">Kali BBQSQL Repo</a></p>
<ul>
<li>Author: BBQSQL</li>
<li>License: BSD</li>
<li>Kali Source: <a href="https://tools.kali.org/vulnerability-analysis/bbqsql">See on Kali Tools Documentation</a></li>
</ul>
{% endraw %}