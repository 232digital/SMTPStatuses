---
title: "4yz Transient Negative Completion"
description: "Transient Negative Completion - The requested action did not occur, but this is a temporary condition"
source: "https://www.rfc-editor.org/rfc/rfc5321#section-4.2.1"
source-name: "RFC 5321, Section 4.2.1"
layout: "subsection-list"
---

The command was not accepted, and the requested action did not occur.
However, the error condition is temporary, and the action may be requested again.
The sender should return to the beginning of the command sequence (if any).
It is difficult to assign a meaning to "transient" when two different sites (receiver- and sender-SMTP agents) must agree on the interpretation.
Each reply in this category might have a different time value, but the SMTP client SHOULD try again.
A rule of thumb to determine whether a reply fits into the 4yz or the 5yz category (see below) is that replies are 4yz if they can be successful if repeated without any change in command form or in properties of the sender or receiver (that is, the command is repeated identically and the receiver does not put up a new implementation).
