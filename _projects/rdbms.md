---
layout: project
title: AdTech Campaign Database System
subtitle: Data Modeling & Relational Design of a Normalized Ad Campaign Database
---
I built this SQL-based database system out of my interest in advertising technology and as part of Win'25 RDBMS Coursework. This project gave me hands-on experience with building a normalized relational database tailored for ad performance analytics. The goal was to design and implement a backend database that supports planning, tracking, and analyzing digital ad campaigns across formats and platforms. The system was designed from scratch following proper database normalization practices (up to 3NF) and includes entities such as Campaign, AdCreative, AudienceSegment, CreativeFormat, and PlatformData. The ERD was carefully structured to minimize redundancy while supporting key relationships such as campaign-to-creatives and platform-wise performance metrics.

For implementation, I wrote SQL DDL scripts to create and populate all core tables using INTEGER, VARCHAR, and DECIMAL data types, with appropriate use of PRIMARY KEY, FOREIGN KEY, and IDENTITY. I also wrote over a dozen SQL queries - covering SELECTs with aggregation, JOINs, INSERTs, UPDATEs, and DELETEs - to simulate realistic use cases like pulling campaign-level performance, analyzing impressions by platform, and managing creative assets.

<a href="https://github.com/jaivardhanschauhan/datamodel-rdbms-adtech" target="_blank" class="button">Code</a>
