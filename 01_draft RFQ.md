# Statement of Objectives for GSA SmartPayⓇ Agile Development Services

## Issued by: Office of Professional Services and Human Capital Categories (PSHC) Office of Contract Operations (QRAD) for the GSA Center for Charge Card Management (CCCM)

### 1.0 Background and Purpose

The GSA Center for Charge Card Management (hereinafter “CCCM”) administers the GSA SmartPay Program, which  is the world’s largest government charge card and commercial payment solutions program. Providing services to nearly 600 federal government agencies, organizations, and Native American tribal governments, GSA SmartPay payment solutions enable authorized government employees to make purchases to support agency and organization missions.

#### 1.1	Purpose
This program has interfaced and provided support to its [users](https://github.com/GSA/smartpay-website/wiki/GSA-SmartPay%C2%AE-%7C-User-Types) and program through various technology tools: (1) GSA SmartPay main website and (2) GSA SmartPay training website.
##### 1.1.1 Current state
(1) The GSA SmartPay main website is available at https://smartpay.gsa.gov and is:
- Built on a Drupal version 9 with PHP programming.
- Hosted on Red Hat Enterprise Linux version 8 servers.

The website received more than 1.8 million visitors (mobile & web) in FY22. Based on current content and development in progress, the government anticipates that traffic will be driven by state sales tax content and visits to the Section 889 Representations tool.

Section 889 of the 2019 National Defense Authorization Act prohibits purchases from certain banned telecommunication and video surveillance equipment in an effort to protect national security. The Section 889 Representations tool (currently expected to go live in March 2023) searches for company 889 status with Unique Entity Identifier (UEI), company name, or Commercial and Government Entity code (CAGE) number via the SAM.gov Entity Management application programming interface (API). The current 889 Representation tool is:
- Built on GSA’s instance of Google Cloud Platform.
- Developed with Python (back-end) and Vue.js (front-end). 

(2) The GSA SmartPay training website provides training to card holders and agency coordinators, which is available at https://training.smartpay.gsa.gov and includes mandatory training as required by law and policy. This offering is optional for agencies to use (some prefer to host their own content in their learning management systems). The current GSA SmartPay training website:
- Is built on a Drupal version 9 with PHP programming.
- Hosted on Red Hat Enterprise Linux version 8 servers.
- Uses a MariaDM database.
- Has five on-demand, HTML-based training courses, which include:
  - Purchase Training for Account Holders/AOs
  - Travel Training for Account Holders/AOs
  - Purchase Training for A/OPCs
  - Travel Training for A/OPCs
  - Fleet Training for A/OPCs

Certificates are issued after the completion of a multiple question quiz with a passing score of 75%. There are more than 800,000 current accounts and just under 600,000 visitors in FY22.

All information posted on the GSA SmartPay main website and GSA SmartPay training website is public. The government owns all code, data, image licenses, user information, and domain names.

##### 1.1.2 Minimally Viable Products

Currently, the CCCM program has partnered with the GSA Service Delivery team on building a minimally viable product (MVP) of the main website and training website using an iterative and user-centered delivery cadence. The Service Delivery team expects the MVP to be delivered by summer 2023 and will work with the Contractor to transition the project. 

The new GSA SmartPay website (GitHub) will:
Be hosted on Cloud.gov Pages (formerly known as Federalist).
Leverage the static site generator, Eleventy.
Incorporate the U.S. Web Design System. 

Note: the information above for the 889 representation tool will remain the same post-MVP. 

The new GSA SmartPay training website (GitHub) will be a combination of static web content and a custom training application with a database component. We expect the website will be hosted on Cloud.gov. 

##### 1.1.3 Future state

The CCCM is seeking a Contractor to take over the MVP and future development. The Contractor will continue to build off the open source code developed by the Service Delivery team and enhance functionality based on user needs, programmatic needs, and changes in policy. The Contractor will need to continue to add content and functionality using GitHub and support the CCCM’s ability to update content using front-end tools, such as Decap content management system (formerly known as Netflify). 

The Service Delivery team is available to support transition. 

Implementation and documentation is ongoing — current specifications are published to the Github repos. These repositories include supplementary information to this RFQ (see also Wikis found here and here).


#### 1.2	Problems

The current GSA SmartPay website is difficult for users to navigate intuitively. CCCM has challenges keeping content current and ensuring content is accessible to all audiences. 
The current GSA SmartPay training website suffers from performance issues, which cause users to time-out in the middle of quizzes or experience random crashes. Since users login so infrequently, they often forget their passwords and need manual assistance in some cases to reset passwords which is a drain on CCCM resources. Reporting is limited and only available at the agency level; for large agencies, this is too untenable to track, and they’re requiring users to email agency coordinators their certificates to manually check them off a list. 


### 2.0 Scope
### 3.0 Objectives
### 4.0 Contract Place of Performance and Contract Type
### 5.0 Operating Constraints (Non-functional Requirements)
### 6.0 Instructions and Evaluation
