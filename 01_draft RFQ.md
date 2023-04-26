# Statement of Objectives for GSA SmartPayⓇ Agile Development Services

## Issued by: Office of Professional Services and Human Capital Categories (PSHC) Office of Contract Operations (QRAD) for the GSA Center for Charge Card Management (CCCM)

### 1.0 Background and Purpose

The GSA Center for Charge Card Management (hereinafter “CCCM”) administers the GSA SmartPay Program, which is the world’s largest government charge card and commercial payment solutions program. Providing services to nearly 600 federal government agencies, organizations, and Native American tribal governments, GSA SmartPay payment solutions enable authorized government employees to make purchases to support agency and organization missions.

#### 1.1	Purpose
This program has interfaced and provided support to [users](https://github.com/GSA/smartpay-website/wiki/GSA-SmartPay%C2%AE-%7C-User-Types) through: (1) GSA SmartPay main website, and (2) GSA SmartPay training website.

##### 1.1.1 Current state
(1) The GSA SmartPay main website is available at [https://smartpay.gsa.gov and is:](https://smartpay.gsa.gov/)
- Built on a Drupal version 9 with PHP programming.
- Hosted on Red Hat Enterprise Linux version 8 servers.

The website received more than 1.8 million visitors (mobile & web) in FY22. Based on current content and development in progress, the government anticipates that traffic will be driven by state sales tax content and visits to the Section 889 Representations tool.

(2) Section 889 of the 2019 National Defense Authorization Act prohibits purchases from certain banned telecommunication and video surveillance equipment in an effort to protect national security. The [Section 889 Representations tool](https://889.smartpay.gsa.gov/#/) searches for company 889 status with Unique Entity Identifier (UEI), company name, or Commercial and Government Entity code (CAGE) number via the SAM.gov Entity Management application programming interface (API). The current 889 Representation tool is:
- Built on GSA’s instance of Google Cloud Platform.
- Developed with Python (back-end) and Vue.js (front-end). 

The GSA SmartPay training website, which is available at https://training.smartpay.gsa.gov/, provides mandatory training to card/account holders, approving officials (AOs), and agency/organization program coordinators (A/OPCs), as required by law and policy. This offering is optional for agencies to use (some prefer to host their own content in their learning management systems). The current GSA SmartPay training website:
- Is built on a Drupal version 9 with PHP programming.
- Is hosted on Red Hat Enterprise Linux version 8 servers.
- Uses a MariaDM database.
- Has five on-demand, HTML-based training courses, which include:
  - Purchase Training for Card/Account Holders/AOs
  - Travel Training for Card/Account Holders/AOs
  - Purchase Training for A/OPCs
  - Travel Training for A/OPCs
  - Fleet Training for A/OPCs

Certificates are issued after the completion of a multiple question quiz with a passing score of 75%. There are approximately 700,000 current accounts and just under 600,000 visitors in FY22.

All information posted on the GSA SmartPay main website and GSA SmartPay training website is public. The government owns all code, data, image licenses, user information, and domain names.

##### 1.1.2 Minimally Viable Products

Currently, CCCM program has partnered with the [GSA Service Delivery](https://github.com/GSA/service-delivery) team to build a minimally viable product (MVP) of the main website and training website using an iterative and user-centered delivery cadence. The Service Delivery team expects the MVP for each website to be delivered by summer 2023 and will work with the Contractor to transition the project. 

The new GSA SmartPay main website ([GitHub](https://github.com/GSA/smartpay-website)) will:
- Be hosted on [Cloud.gov Pages](https://cloud.gov/pages/) (formerly known as Federalist).
- Leverage the static site generator, [Eleventy](https://www.11ty.dev/).
- Incorporate the [U.S. Web Design System](https://designsystem.digital.gov/). 

The above-mentioned 889 tool will be migrated from Google Cloud Platform to Cloud.gov before launch of the new GSA SmartPay main website.

The new GSA SmartPay training website ([GitHub](https://github.com/GSA/smartpay-training)) will be a combination of static web content and a custom training application with a database component. The training website will be hosted on Cloud.gov. 

##### 1.1.3 Future state

CCCM is seeking a Contractor to take the MVP of each website and continue future development. The Contractor will continue to build off the open source code developed by the Service Delivery team and develop enhanced functionality based on user needs, programmatic needs, and changes in policy. The Contractor will need to continue to add content and functionality using GitHub and support CCCM’s ability to update content using front-end tools, such as [Decap content management system](https://www.netlifycms.org/) (formerly known as Netflify). 

The Service Delivery team is available to support transition. 

Implementation and documentation is ongoing — current specifications are published to the Github repos. These repositories include supplementary information to this RFQ (see also Wikis found [here](https://github.com/GSA/smartpay-website/wiki) and [here](https://github.com/GSA/smartpay-training/wiki)).


#### 1.2	Problems
The current GSA SmartPay main website is difficult for users to navigate intuitively. CCCM has challenges keeping content current and ensuring content is accessible to all audiences.

The current GSA SmartPay training website suffers from performance issues, which cause users to time-out in the middle of quizzes or experience random crashes. Since users login so infrequently, they often forget their passwords and need manual assistance in some cases to reset passwords which is a drain on CCCM resources. Reporting is limited and only available at the agency level; for large agencies, this is too untenable to track, and they’re requiring users to email agency coordinators their certificates to manually check them off a list.


### 2.0 Scope

CCCM seeks agile software development services. The services to be provided will include all aspects of the software development process, including planning, design, software development and coding, prototyping, documentation, and testing. The services also include support of GSA security documentation and testing. 

CCCM intends that the software delivered under this task order will be committed to the public domain. The Contractor will have to obtain CCCM’s permission before delivering software under this task order that incorporates any software that is not free and open source. The Contractor must post all developed code to a GitHub repository designated by CCCM.

#### 2.1	Product Vision

Make it easier for GSA SmartPay users to find the information they need and to comply with government-wide and agency requirements.

#### 2.2	Anticipated Period of Performance, Budget, and Ceiling Price

The period of performance (PoP) shall be one year, with options to extend up to two additional years. GSA may, by written notice issue and at least 60 days prior to the expiration of the initial term, extend the period of performance for additional option years. The PoP is expected to begin on or around Aug 1, 2023.

The not to exceed ceiling on this contract will be $840,000 for the first period of performance (52.232-22 Limitation of Funds applicable) and up to an additional $550,000 for each of the two option periods. Contractors are expected to submit a quote reflective of its solution to fulfill the government’s requirements.

The government may require continued performance of any services within the limits and at the rates specified in the task order in accordance with FAR Subpart 52.217-8 - Option To Extend Services, evaluation will be accomplished by using the prices offered for the last option period to determine the price for a 6-month option period, which will be added to the base and other option years to arrive at the total price. Evaluation of options will not obligate the Government to exercise the option(s).

### 3.0 Objectives

#### 3.1	Backlog

The set of preliminary user stories set forth below will be the starting point for the development of software to be provided by the Contractor under this task order. These preliminary user stories are provided only for illustrative purposes, and do not comprise the full scope or detail of the project. CCCM expects that the Contractor will work closely with CCCM Product Owner(s) to develop and prioritize a full gamut of user stories as the project progresses.

Individual user stories may be modified, added, retracted, or reprioritized by CCCM at any time, and CCCM expects that the user stories will be continuously refined during the development process. 

**Programmatic data**
- As an Agency / Organization Program Coordinator (A/OPC), I want information relevant for agency spend, so I can provide this to agency Chief Financial Officers as requested.
- As an A/OPC, I want access to travel spend by region, so I can understand regional spend trends for travel.

**Training reporting**
- As an A/OPC, I want users to be sent automatic reminders for training, so that certification requirements are automatically managed by the training platform.
- As a Level 1 A/OPC, I want to have reports automatically sent to me at indicated time frames, so I can have regular access to reports without having to access the system.
- As an A/OPC and administrator, I want to have customizable reports, so I have the ability to further analyze data.

**Administrative functions**
- As a system administrator, I want to perform periodic database purges for users who exist in the system but have not completed any quizzes so I can keep the database up-to-date and reduce storage requirements.
- As an administrator, I want to be able to post system messages, so I can alert users to website status.
- As an administrator, I want a user friendly maintenance interface, so I can easily make content changes.
- As an administrator, I want to be able to modify a user’s profile in the database, so that I can correct incorrect or out-of-date information.

**Email usage/monitoring**
- As an administrator, I want to be able to confirm what emails were sent to whom and when, so that we can ensure users are being properly notified.
- As an administrator, I want to monitor email bouncebacks, so that I can take corrective action (as needed) to ensure users are being properly notified.
- As an administrator, in the event of important information / notification, I need the ability to send emails to all users.

**Other**
- As an A/OPC and card holder, I want access to interactive content, so I can engage with the content in the forum I feel most comfortable.
- As an A/OPC and card holder, I want quick access to GSA SmartPay’s social media accounts, so that I can stay apprised of program information / announcements.
- As the GSA SmartPay program, we want to implement Google Tag Manager, in order to have more transparency into how our users are using our main website and training website.

**Security**
- As the system administrator, I need [a specific system vulnerability] that was discovered during penetration testing to be remediated, to ensure the training website remains secure.
- As the system administrator, I need [a specific item] to be updated, to comply with updated GSA IT security policies, standards and guidelines.
- As a system administrator, I need the System Security Plan to be updated, to reflect a change in the system [because of a specific reason].

#### 3.2 List of Deliverables with Quality Assurance Surveillance Plan (QASP)
The following chart sets forth the performance standards and quality levels the code and documentation provided by the Contractor must meet, and the methods CCCM will use to assess the standard and quality levels of that code and documentation.


| Deliverable | Performance Standard(s) | Acceptable Quality Level | Method of Assessment |
| --- | --- | --- | --- |
| Tested Code | Code delivered under the order must have substantial test code coverage | Minimum of 90% test coverage of all code. All areas of code are meaningfully tested | Combination of manual review and automated testing |
| Properly Styled Code | [GSA 18F Coding Styles](https://frontend.18f.gov/#js-style) Reference Guide | 0 linting errors and 0 warnings | Combination of manual review and automated testing |
| Accessible | Web Content Accessibility Guidelines 2.1 AA standards | 0 errors reported using an automated scanner and 0 errors reported in manual testing | Combination of manual review and automated testing (such as [pa11y](https://github.com/pa11y/pa11y)) |
| Deployed | Code must successfully build and deploy into staging environment | Successful build with a single command | Combination of manual review and automated testing |
| Documented | Summary of user stories completed every sprint. All dependencies are listed and the licenses are documented. <br>Major functionality in the software/source code is documented. Individual methods are documented inline in a format that permits the use tools such as JSDoc. System diagram is provided. <br>Relevant security controls are documented and kept up to date. | Combination of manual review and automated testing, if available | Manual review |
| Secure | Code is free of known static and runtime vulnerabilities | Code submitted must be free of medium- and high-level static and dynamic security vulnerabilities | Tests free of medium- and high-level vulnerabilities from a static testing SaaS (such as Snyk or npm audit), from dynamic testing tools like OWASP ZAP (with documentation explaining any false positives), and ongoing code review informed by OWASP or similar standards |


### 4.0 Contract Place of Performance and Contract Type
### 5.0 Operating Constraints (Non-functional Requirements)
### 6.0 Instructions and Evaluation
