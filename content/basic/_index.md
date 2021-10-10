---
title: Basic Reply Codes
description: The basic SMTP reply codes
---

The Basic SMTP Reply Codes are defined in [RFC 5321, Section 4.2](https://www.rfc-editor.org/rfc/rfc5321#section-4.2) except as noted. Please see the RFCs for more detailed information.

> Replies to SMTP commands serve to ensure the synchronization of requests and actions in the process of mail transfer and to guarantee that the SMTP client always knows the state of the SMTP server.
> Every command MUST generate exactly one reply.

## Structure

The three digits of the reply each have a special significance.
The first digit denotes whether the response is good, bad, or incomplete.
The second digit of the reply code narrows the meaning to a category:

x0z
: Syntax

x1z
: Information

x2z
: Connections

x5z
: Mail system

The third digit gives a finer gradation of meaning in each category specified by the second digit.
