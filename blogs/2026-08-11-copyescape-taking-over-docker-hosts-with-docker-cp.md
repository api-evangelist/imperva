---
title: "CopyEscape: Taking Over Docker Hosts with docker cp"
url: "https://www.imperva.com/blog/copyescape-taking-over-docker-hosts-with-docker-cp/"
date: "2026-08-11"
author: "Ron Masas"
feed_url: "https://www.imperva.com/blog/feed/"
---
Imperva Red Team uncovered CVE-2026-17106, a container-to-host arbitrary file-write vulnerability in Docker’s docker cp command. Docker later confirmed that the same CVE also affected sbx cp when copying files out of Docker Sandboxes. A malicious container or sandbox could exploit the copy process to create or overwrite files outside the destination selected by the user, […] The post CopyEscape: Taking Over Docker Hosts with docker cp appeared first on Blog .
