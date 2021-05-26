+++
author = "team_members/tero.md"
date = 2021-05-31T22:00:00Z
description_markdown = "CIS Controls version 8 was released 18th of May. We'll have a quick look at the new shiny."
draft = true
image = "/uploads/cis-is-releasing-their-revised-top-20-critical-security-controls.jpg"
tags = []
title = "CIS Controls Version 8"
weight = 1
[link]
URL = "https://learn.cisecurity.org/cis-controls-download"
label = "Download CIS Controls Here"

+++
Center for Internet Security (CIS) security controls have, for a long while, been seen as the "easy to use" IT-security framework, offering best practice advice in reasonably actionable, easy to understand and cheap format - so no pesky ISO 27000 document purchases required.

In many ways the recently (18th of May) released update to version 8 continues on this track - it is still a collection of IT-Security best practices. However, as the framework grows, so does the documentation and complexity.

Let's  have a quick look at the changes and discuss the goods, the bads and the uglies.

### A quick overview

We're down to 18 controls instead of the traditional 20. It'll be a while before I get used to referring to it as "18 controls".  If you're familiar with the previous versions, you'll feel right at home with many of them, they haven't changed much.

As with version 7, the controls are divided with three implementation groups (IG) which try to reflect the required maturity of the control implementation (IG1 representing basic security hygiene). 

Initially the new numbering of the controls might be a big confusing. CIS is careful to point out that the order of the controls has nothing to do with implementation priority - it should be treated as a holistic process. 

Here's the whole list - and attempt to illustrate the change of order.

 1. Inventory and Control of Enterprise Assets
 2. Inventory and Control of Software Assets
 3. Data Protection (moved from 13)
 4. Secure Configuration of Enterprise Assets and Software (merged from 5 and 11)
 5. Account Management (moved from 16)
 6. Access Control Management (merged from 4 and 14)
 7. Continuous Vulnerability Management (moved from 3)
 8. Audit Log Management (moved from 6)
 9. Email and Web Browser Protections (moved from 7)
10. Malware Defenses (moved from 8)
11. Data Recovery (moved from 10)
12. Network Infrastructure Management (**new!**)
13. Network Monitoring and Defense (**new!**)
14. Security Awareness and Skills Training (moved from 17)
15. Service Provider Management (**new!**)
16. Application Software Security (moved from 18)
17. Incident Response Management (moved from 19)
18. Penetration testing (moved from 20)

It's a bit unclear why the list has been re-ordered, being an old dog, learning new tricks requires quite a lot of (seemingly) unnecessary brain power.

All in all, it's 18 controls which contain 146 specific "best practice" actions (the framework calls these "Safeguards"). It's not a bad start by any means, if you're looking for a "simple" framework to start with.

A word of warning though - even though the outlining in is quite simple, the difficulty of implementing some of the controls varies wildly. For example the first three Safeguards for IG1 (basic hygiene) for Control 8, Audit Log Management are:

1. Establish and Maintain an Audit Log Management Process
2. Collect Audit Logs
3. Ensure Adequate Audit Log Storage

That's relatively easy and actionable list, right?  Now, compare this to implementing same IG1 level for Control 3, Data Protection:

1. Establish and Maintain a Data Management Process
2. Establish and Maintain a Data Inventory
3. Configure Data Access Control Lists

My feeling is that this requires quite a bit higher digital maturity than the previous control and there's far fewer companies out there with Data Management projects than there are companies doing Audit Log projects.

So just be aware that some of the difficulty in implementing the controls is a bit deceptive and if you're going to use CIS controls as your framework, it's probably a good idea to assess how ready your business is to implement each of the controls, before plunging into them head first.