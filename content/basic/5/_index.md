---
title: "5yz Permanent Negative Completion"
description: "Permanent Negative Completion - The requested action did not occur, and this condition is permanent"
source: "https://www.rfc-editor.org/rfc/rfc5321#section-4.2.1"
source-name: "RFC 5321, Section 4.2.1"
layout: "subsection-list"
---

The command was not accepted and the requested action did not occur.
The SMTP client SHOULD NOT repeat the exact request (in the same sequence).
Even some "permanent" error conditions can be corrected, so the human user may want to direct the SMTP client to reinitiate the command sequence by direct action at some point in the future (e.g., after the spelling has been changed, or the user has altered the account status).
