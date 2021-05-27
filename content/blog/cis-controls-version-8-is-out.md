+++
author = "team_members/tero.md"
date = 2021-05-26T10:00:00Z
description_markdown = "CIS Controls version 8 was released 18th of May. We'll have a quick look at the new shiny."
image = "/uploads/cis-is-releasing-their-revised-top-20-critical-security-controls.jpg"
tags = ["cis", "controls", "compliance", "framework"]
title = "CIS Controls Version 8"
weight = 1
[link]
URL = "https://learn.cisecurity.org/cis-controls-download"
label = "Download CIS Controls Here"

+++
Center for Internet Security (CIS) security controls have, for a long while, been seen as the "easy to use" IT-security framework, offering best practice advice in reasonably actionable, easy to understand and cheap format - so no pesky ISO 27000 document purchases required.

In many ways the recently (18th of May) released update to version 8 continues on this track – it is still a collection of IT-Security best practices. However, as the framework grows, so does the documentation and complexity.

Let's  have a quick look at the changes and discuss the goods, the bads and the uglies.

### CIS 20 is dead! Long live CIS 18!

We're down to 18 controls from the traditional 20. It'll be a while before I get used to referring to it as "18 controls". If you're familiar with the previous versions, you'll feel right at home with many of them, they haven't changed much.

As with version 7, the controls are divided with three implementation groups (IG) which try to reflect the required maturity of the control implementation (IG1 representing basic security hygiene).

Initially the new numbering of the controls might be a bit confusing. CIS is careful to point out that the order of the controls has nothing to do with implementation priority – it should be treated as a holistic process.

Here's the whole list – with an attempt to illustrate the change of order.

 1. Inventory and Control of Enterprise Assets
 2. Inventory and Control of Software Assets
 3. Data Protection (moved from 13)
 4. Secure Configuration of Enterprise Assets and Software (merged from 5 and 11)
 5. Account Management (moved from 16)
 6. Access Control Management (merged from 4 and 14)
 7. Continuous Vulnerability Management (moved from 3)
 8. Audit Log Management (moved from 6)
 9. Email and Web Browser Protections (moved from 7)
10. Malware Defences (moved from 8)
11. Data Recovery (moved from 10)
12. Network Infrastructure Management (**new!**)
13. Network Monitoring and Defence (**new!**)
14. Security Awareness and Skills Training (moved from 17)
15. Service Provider Management (**new!**)
16. Application Software Security (moved from 18)
17. Incident Response Management (moved from 19)
18. Penetration testing (moved from 20)

For an old dog, it's a bit unclear why the list has been re-ordered, learning new tricks requires quite a lot of (seemingly) unnecessary brain power.

All in all, it is 18 controls which contain 146 specific "best practice" actions (the framework refers to these as "Safeguards"). It's not a bad start by any means, if you're looking for a "simple" framework to start with.

A word of warning though – even though the outlining is quite simple, the difficulty of implementing some of the controls varies wildly. For example, the first three Safeguards for IG1 (basic hygiene) for Control 8, Audit Log Management are:

1. Establish and Maintain an Audit Log Management Process
2. Collect Audit Logs
3. Ensure Adequate Audit Log Storage

That's relatively easy and actionable, right?  Now, compare this to implementing same IG1 level for Control 3, Data Protection:

1. Establish and Maintain a Data Management Process
2. Establish and Maintain a Data Inventory
3. Configure Data Access Control Lists

My feeling is that this requires quite a bit higher digital maturity than the previous control and there's far fewer companies out there with Data Management projects than there are companies doing Audit Log projects.

So just be aware that some of the difficulty in implementing the controls is a bit deceptive and if you're going to use CIS controls as your framework, it's probably a good idea to assess how ready your business is to implement each of the controls, before plunging into them head first.

### The New Stuff

Starting from 2013, the CIS team has worked with the [Verizon Data Breach Investigations Report (DBIR)](https://www.verizon.com/business/resources/reports/dbir/) (by the way, new blog about the latest DBIR coming up soonish) team to map the results of their large-scale data analysis directly to the CIS Controls, as a way to match their summaries of attacks into a standard program for defensive improvement.

Even though the idea of mapping actual verifiable breach data to Safeguard evaluation is still work in progress, this is starting to show up in the new controls.

The three new controls are:

1. Network Infrastructure Management
2. Network Monitoring and Defence
3. Service Provider Management

#### Network Infrastructure Management

This is about securing network infrastructure against attacks. Network infrastructure includes devices such as physical and virtual gateways, firewalls, wireless access points, routers, switches and the control focuses on addressing architecture and configuration (e.g. default configs and passwords).

Given the situation with COVID, the recent VPN vulnerabilities and most of the workforce working remotely, this has of course been a "hot potato" during 2020.

#### Network Monitoring and Defence

This one is naturally related to the control above and focuses on being able establish and maintain comprehensive network monitoring and defence against security threats across the enterprise’s network infrastructure and user base. Being proactive with threat detection.

This one is quite interesting, because the subject matter lands very much in our Squared Circle backyard! Let us know if you'd like to know how to implement this one :)

#### Service Provider Management

And of course we must have the Supply Chain and Cloud represented. This one is all about developing processes to evaluate service providers who hold sensitive data, or are responsible for enterprise critical IT platforms or processes, to ensure these providers are protecting the platforms and data appropriately.

I think it's a good start, but we have a long, long way to go before this control can be considered "easily actionable".  And towards that point, there's actually only one Safeguard on IG1 basic hygiene level (Establish and Maintain an Inventory of Service Providers). The rest require quite a bit more maturity from your organization.

### Final Thoughts

The CIS group has also released a lot of "companion tools" – like mappings towards other popular frameworks (NIST, CSA, CMMC etc.) so those are probably also worth a download if you're currently wading knee-deep in the framework jungle.

To me personally, the CIS Controls have always lived in that juxtaposition of best practice “good things to do” and "accredited audit framework" – and I think that's where it should live. We have a shortage of "easy to pick up, easy to implement" frameworks and it would be shame to have it completely disappear into compliance auditing world and lose its history in "hands-on" IT-security.

Only the future will tell where it will end up, but I do like the growing focus of building the controls with open and verifiable methods and data. Looking forward to the future efforts of bringing [MITRE Att&ck](https://attack.mitre.org/) connections into the framework through Safeguards.