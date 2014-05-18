---
layout: post
title: "The hardest part about software development is to decide what to develop - Part 2"
modified: 2014-04-21 14:30:43 -0400
tags: [non-functional requirements, system design]
image:
  feature: post-4-pic.jpg
  credit:  NASA
  creditlink: http://photojournal.jpl.nasa.gov/jpegMod/PIA17041_modest.jpg
comments: true
share: true 
---
> #### "A designer makes things... Typically his making process is complex. There are more variables, kinds of possible moves, norms and interrelationships of these than can be represented in a finite model.” – Donald A Schon.

Last  time, [I discussed the importance of understanding the problem domain](http://techieslikeme.com/the-hardest-part-about-software-development-is-to-decide-what-to-develop/) and capturing  relevant functional requirements for large scale software development projects. This time, I would like to highlight system or non-functional requirements for a software. Often, these non-functional requirements comes as an afterthought when it often too late,  the highly publicized  performance and scalability  issues with [heathcare.gov website](https://www.healthcare.gov/) is perhaps a very good example. Therefore it is essential to include these system level requirements from the very beginning and allocate enough time and effort in the overall software development plan.


[This list is also available in github, so feel free to add any new aspects I may have missed](https://github.com/smtechnocrat/softwaredevelopmentproblem/blob/master/System-Level-Requirements.md). The following list is presented in alphabetical order.

### Non-functional System Level Requirements.

1. <b>Availability</b> - Desired up-time during which the system and data are available for use. What are the availability requirements?

2. <b>Batch Processing and feeds</b> - Is there any requirement for batch processing or nightly data feeds from other systems?

3. <b>Communications Interfaces</b> - Any communication functions the system will use needs to be documented. (example – web browsers). [The system uses HTTP protocol to communicate with the servers. Users use HTTPS (secure site) to login to the system.]

4. <b>Configurability</b> - what aspects of the system can be configured? 
   * How will be configuration be managed?
   * Who can configure the system and when?

5. <b>Data Visibility</b> – What are the data visibility requirements ?

6. <b>Data Versioning and or temporal aspects</b> - 
   * Does the system need to answer time sensitive questions related to its state?
   * Does the data needs to be versioned? 

7. <b>Design and Implementation Constraints</b> – Issues that will restrict the options available to the development team, including the reason for the constraint (example – technology choice).

8. <b>Deployment Topology</b> – 
   * Where do we need to deploy the system to ? 
   * What are the deployment constraints, procedures and support ? 
   * What will be the proposed deployment topology ? 
   * Do we need a Content Delivery Network?

9. <b>Documentation</b> - Describe the purpose, desired contents, level of detail, and formatting (User Manuals, Installation Guides, Online Documentation and Help Systems and Labeling and Packaging

10. <b>Efficiency</b> - How well the system utilizes resources such as memory, disk space, etc.

11. <b>Entitlements</b> - what features of the system needs to be entitled?

12. <b>Failover and Recovery</b> – How will the system recover from hardware failure,  software failure, load and peak loads? 

13. <b>Flexibility</b> - How much effort is needed to add new capabilities to the product? 

14. <b>Hardware Interfaces</b> - The characteristics of each interface between the software system and the hardware components of the system. 

15. <b>Interoperability</b> - How easily the system can interact with other systems?

16. <b>Logical Database Requirements</b> - Requirements for any information that is to be placed into a database, including data models, field types, frequency of use, integrity constraints and accessing capabilities.

17. <b>Look and Feel</b> - General requirements that capture how the system will appear? [The User Interface will utilize web pages and adhere to the standards already in place among the web-based applications.]

18. <b>Maintainability</b> - How easy it is to fix a defect or change a requirement in the system after it is deployed? [The system will follow all IT Change Management procedures when maintenance is required.]

19. <b>Memory Constraints</b> - Any constraints on the system based on memory usage? For mobile applications, this aspect will be more relevant.

20. <b>Operations</b> - Any operations required by the user? (example – client/user or content management). 

21. <b>Performance</b> - Include requirements placed on the software performance or on performance of the human interaction with the software. Describe throughput requirements. 
   * What kind of load can the system handle ( how many concurrent users/request ? )
   * How does the system perform during peak loads? 
   * Does the system fail gracefully?
   * What is the breaking point? 

22. <b>Portability</b> - How easily the system can be migrated from one platform to another or one machine to another ?

23. <b>Reference Data</b> – What are the reference data requirements for the system ? Where do we get this data from ?

24. <b>Reliability</b> - Probability of the software executing without failure for a period of time

25. <b>Reusability</b> - How easily a component of the system can be used by another system?

26. <b>Robustness</b> - How well the system needs to function when there is invalid data, defects, or unexpected errors?

27. <b>Security</b> - Specify the factors that would protect the software from accidental or malicious access, use, modification, destruction, or disclosure. [e.g. Any file uploads using protocols such as FTP shall be secured using 128 bit encryption.]

28. <b>Site Adaptation Requirements</b> – Requirements specific to where the product software failure, load and peak loads ? will be installed (example – globalization requirements). [e.g. All timestamps shown by the system shall be translated into the local time where the system is installed]

29. <b>Software Interfaces</b> - The use of other required software products and interfaces with the system. [The system must accept orders from other external/internal systems that has different formats, or uses different protocols etc.]

30. <b>Software Licensing and Approvals</b> – What third party software ( both open source and vendor products ) does the system use ? What kind of licenses does each one of these software require ? Note: Open source software licenses also needs to examined since there are major restrictions of use

31. <b>Support</b> - What kind of support will be needed once the system is rolled out ? If deployed globally, how do we organize support teams ?( L1, L2 and L3 )

32. <b>Testability</b> - Ease with which the system can be tested for defects. 

33. <b>Tools</b> - What support tools needs to be built ? [ Eg: a tool to add new users ] This is perhaps one of the most important aspects of software development. 
 * Software Development Lifecycle Management tools
 * Automated testing tools ( functional, performance, load, failure or break  testing
 * Metrics gathering tools
 * Application management tools



34. <b>Usability</b>
 * How easy is to use for the end users?  
 * What kind of adoption challenges will the user face?
