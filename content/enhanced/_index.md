---
title: Enhanced Status Codes
description: The enhanced SMTP status codes giving more specific information in addition to the basic reply codes.
---

The Enhanced Mail System Status Codes are defined in [RFC 3463](https://www.rfc-editor.org/rfc/rfc3463.html) except as noted.

> In combination with other information provided in the Delivery Status Notification (DSN) delivery report, these codes facilitate media and language independent rendering of message delivery status.

## Structure

### Class Sub-code

#### 2.XXX.XXX Success

Success specifies that the DSN is reporting a positive delivery action.
Detail sub-codes may provide notification of transformations required for delivery.

#### 4.XXX.XXX Persistent Transient Failure

A persistent transient failure is one in which the message as sent is valid, but persistence of some temporary condition has caused abandonment or delay of attempts to send the message.
If this code accompanies a delivery failure report, sending in the future may be successful.

#### 5.XXX.XXX Permanent Failure

A permanent failure is one which is not likely to be resolved by resending the message in the current form.
Some change to the message or the destination must be made for successful delivery.
