# Statement of Objectives for GSA SmartPayⓇ Agile Development Services

## Issued by: Office of Professional Services and Human Capital Categories (PSHC) Office of Contract Operations (QRAD) for the GSA Center for Charge Card Management (CCCM)

### 1.0 Background and Purpose

The GSA Center for Charge Card Management (hereinafter “CCCM”) administers the GSA SmartPay Program, which is the world’s largest government charge card and commercial payment solutions program. Providing services to nearly 600 federal government agencies, organizations, and Native American tribal governments, GSA SmartPay payment solutions enable authorized government employees to make purchases to support agency and organization missions.

#### 1.1	Purpose
This program has interfaced and provided support to [users](https://github.com/GSA/smartpay-website/wiki/GSA-SmartPay%C2%AE-%7C-User-Types) through: (1) GSA SmartPay main website, and (2) GSA SmartPay training website.

##### 1.1.1 Current state
(1) The GSA SmartPay main website is available at [https://smartpay.gsa.gov](https://smartpay.gsa.gov/) and is:
- Built on a Drupal version 9 with PHP programming.
- Hosted on Red Hat Enterprise Linux version 8 servers.

The website received more than 1.8 million visitors (mobile & web) in FY22. Based on current content and development in progress, the government anticipates that traffic will be driven by state sales tax content and visits to the Section 889 Representations tool.

Section 889 of the 2019 National Defense Authorization Act prohibits purchases from certain banned telecommunication and video surveillance equipment in an effort to protect national security. The [Section 889 Representations tool](https://889.smartpay.gsa.gov/#/) searches for company 889 status with Unique Entity Identifier (UEI), company name, or Commercial and Government Entity code (CAGE) number via the SAM.gov Entity Management application programming interface (API). The current 889 Representation tool is:
- Built on GSA’s instance of Google Cloud Platform.
- Developed with Python (back-end) and Vue.js (front-end). 

(2) The GSA SmartPay training website, which is available at https://training.smartpay.gsa.gov/, provides mandatory training to card/account holders, approving officials (AOs), and agency/organization program coordinators (A/OPCs), as required by law and policy. This offering is optional for agencies to use (some prefer to host their own content in their learning management systems). The current GSA SmartPay training website:
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

The above-mentioned 889 tool will be migrated from Google Cloud Platform to Cloud.gov and Cloud.gov Pages before launch of the new GSA SmartPay main website.

The new GSA SmartPay training website ([GitHub](https://github.com/GSA/smartpay-training)) will be a combination of static web content and a custom training application with a database component. The training website will be hosted on Cloud.gov and Cloud.gov Pages.

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
- As a system administrator, I need to remediate vulnerabilities based on authenticated scans, to comply with monthly security deliverable requirements.
- As a system administrator, I need the System Security Plan to be updated, to reflect a significant change in the system.


#### 3.2 List of Deliverables with Quality Assurance Surveillance Plan (QASP)
The following chart sets forth the performance standards and quality levels the code and documentation provided by the Contractor must meet, and the methods CCCM will use to assess the standard and quality levels of that code and documentation.


| Deliverable | Performance Standard(s) | Acceptable Quality Level | Method of Assessment |
| --- | --- | --- | --- |
| Tested Code | Code delivered under the order must have substantial test code coverage | Minimum of 90% test coverage of all code. All areas of code are meaningfully tested | Combination of manual review and automated testing |
| Properly Styled Code | [GSA 18F Coding Styles](https://engineering.18f.gov/frontend/#js-style) Reference Guide | 0 linting errors and 0 warnings | Combination of manual review and automated testing |
| Accessible | Web Content Accessibility Guidelines 2.1 AA standards | 0 errors reported using an automated scanner and 0 errors reported in manual testing | Combination of manual review and automated testing (such as [pa11y](https://github.com/pa11y/pa11y)) |
| Deployed | Code must successfully build and deploy into staging environment | Successful build with a single command | Combination of manual review and automated testing |
| Documented | Summary of user stories completed every sprint. All dependencies are listed and the licenses are documented. <br>Major functionality in the software/source code is documented. Individual methods are documented inline in a format that permits the use tools such as JSDoc. System diagram is provided. <br>Relevant security controls are documented and kept up to date. | Combination of manual review and automated testing, if available | Manual review |
| Secure | Code is free of known static and runtime vulnerabilities | Code submitted must be free of medium- and high-level static and dynamic security vulnerabilities | Tests free of medium- and high-level vulnerabilities from a static testing SaaS (such as Snyk or npm audit), from dynamic testing tools like OWASP ZAP (with documentation explaining any false positives), and ongoing code review informed by OWASP or similar standards |


### 4.0 Contract Place of Performance and Contract Type
The Contractor may choose the location(s) from which to perform the required software development services so long as the work is performed in the Contiguous United States (CONUS). CONUS is defined as the 48 contiguous States and the District of Columbia. CCCM’s core customer service hours are 8:00 am - 4:00 pm ET; we expect the software development team would be available 11:00 am - 4:00 pm ET, but we would need an assigned point of contact outside those hours if urgent matters arise. 

CCCM intends to issue a time and materials task order under an existing contract under the Multiple Award Schedule (“Schedules”) Technology's Special Item Number (SIN) 54151S for IT Professional Services, and all quotes must be submitted on that basis. CCCM will not consider quotes that include fees for licenses or subscriptions. 


### 5.0 Operating Constraints (Non-functional Requirements)

#### 5.1	Environment
- Software development services will occur in the GSA SmartPay Github environment(s).
- Website usage will be tracked with the [Digital Analytics Program](https://digital.gov/guides/dap/). 
- Hosting will be on Cloud.gov Pages for building and serving front-end static assets and Cloud.gov for serving APIs and hosting the database and other backend services. Services are provided through an intra agency agreement that CCCM has in place with Cloud.gov.
- Current coding languages are Python for the back-end and JavaScript (Astro and Vue.js) for the front-end. The government is not prescribing that these must be the coding language(s) moving forward.

#### 5.2	Design
- Software development services shall leverage the [U.S. Web Design System](https://designsystem.digital.gov/).
- Content development will follow CCCM [style guide](https://github.com/GSA/smartpay-website/wiki/GSA-SmartPay%C2%AE-%7C-Style-Guide-for-the-Website-and-Training-Platform).

#### 5.3 	System Access 
- All Contractor personnel working under the task order will need to be U.S. citizens. 
- Homeland Security Presidential Directive 12 (HSPD-12) applies to Contractor development personnel as such performance requires access to internal Government information technology (IT) systems.  As a result of HSPD-12 applicability to the requirements of this document, the Government will perform all required background investigations for Contractor personnel, and the Contractor shall ensure their personnel requiring physical access to Federally- controlled information technology systems have identification that complies with HSPD-12 policy. Immediately upon award the credential process shall commence. All identified Contractor personnel must complete a GSA Form 850 – Contractor Information Worksheet (CIW) to be provided with the proposal submission. The Contractor will not be given the Notice to Proceed (NTP) to start work until all Contractor personnel have the proper identification to satisfy this requirement.
- Medium risk security clearance (Tier 2) shall be required
- [NIST](https://www.nist.gov/itl/smallbusinesscyber/guidance-topic/multi-factor-authentication) phishing resistant multi-factor authentication (MFA) shall be required for privileged and non-privileged users where login is required.  

#### 5.4	Security
The Contractor shall comply with the technology security requirements in the Federal Information Security Management Act (FISMA) (44 .S.C. 3544); the applicable National Institute of Standards and Technology; GSA IT security policies, standards and guidelines; and other Government-wide laws and regulations for protection and security of IT. The required policies and regulations are specified in Security and Privacy Requirements for IT Acquisition Efforts CIO-IT Security-09-48 ([Attachment A](https://github.com/GSA/SmartPay-RFI/blob/main/Attachment%20A_Security%20and%20Privacy%20Requirements%20for%20IT%20Acquisition%20Efforts%20CIO-IT%20Security-09-48.pdf)) or latest version and Managing Enterprise Cybersecurity Risk CIO-IT Security-06-30 or latest version ([Attachment B](https://github.com/GSA/SmartPay-RFI/blob/main/Attachment%20B_Managing%20Enterprise%20Cybersecurity%20Risk%20CIO-IT%20Security-06-30.pdf)). 

Security compliance will be continuous through DevSecOps practices and via user stories issued in sprint planning. Additional information about security and confidentiality requirements can be found in the current version of CIO_21001N_GSA_Information_Technology_Security_Policy ([Attachment C](https://github.com/GSA/SmartPay-RFI/blob/main/Attachment%20C_CIO_21001N_GSA_Information_Technology_Security_Policy.pdf)).

##### 5.4.1 Specific Security Requirements
The Contractor shall have all staff members complete a confidentiality agreement prior to starting contract performance. 

#### 5.5	Personnel Skills and Knowledge
_Key Personnel_ – The Contractor must designate both a Project Manager (PM) and a Technical Lead (or labor category equivalent) as Key Personnel for this project. The PM will be a direct liaison to the CCCM product team, and will be responsible for the supervision and management of all of the Contractor’s personnel. The Technical Lead must have a full understanding of the technical approach to be used by the Contractor’s development team and will be responsible for ensuring that the Contractor’s development team follows that approach.

_Key Personnel Substitution_ – Key Personnel substitutions must be approved by CCCM in writing. Contractor requests for a substitution of Key Personnel must include a detailed explanation of the justifying circumstances, and a complete résumé for the proposed substitute or addition, including skills, experience, education, training, and security level. 

_Teaming Arrangements_ – No teaming will be permitted.

#### 5.6	Special Clauses
_Data Rights and Ownership of Deliverables_ – CCCM intends that all software and documentation delivered by the Contractor will be owned by CCCM and committed to the public domain. This software and documentation includes, but is not limited to, data, documents, graphics, code, plans, reports, schedules, schemas, metadata, architecture designs, and the like; all new open source software created by the Contractor and forks or branches of current open source software where the Contractor has made a modification; and all new tooling, scripting configuration management, infrastructure as code, or any other final changes or edits to successfully deploy or operate the software.

To the extent that the Contractor seeks to incorporate any software that was not first produced in the performance of this task order in the software delivered under this task order, CCCM encourages the Contractor to incorporate either software that is in the public domain, or free and open source software that qualifies under the Open Source Definition promulgated by the Open Source Initiative. The Contractor must obtain written permission from CCCM before incorporating into the delivered software any software that is subject to a license that does not qualify under the Open Source Definition promulgated by the Open Source Initiative. If CCCM grants such written permission, then the Contractor’s rights to use that software must be promptly assigned to CCCM.

If software delivered by the Contractor incorporates software that is subject to an open source license that provides implementation guidance, then the Contractor must ensure compliance with that guidance. If software delivered by the Contractor incorporates software that is subject to an open source license that does not provide implementation guidance, then the Contractor must attach or include the terms of the license within the work itself, such as in code comments at the beginning of a file, or in a license file within a software repository.

#### 5.7 Invoicing/Payment

##### 5.7.1 Invoices
Invoices for services and/or travel expenses must be submitted to the address (physical or e-mail) specified below. In addition to the requirements defined in sections 5.7.3 and 5.7.4, to constitute a proper invoice, the billing document must include the following information and/or attached documentation:
<br>(1) Name of Contractor and Contractor’s Taxpayer Identification Number;
<br>(2) Period covered by invoice and invoice date;
<br>(3) Purchase order number;
<br>(4) All invoices for services must set forth in detail the following:
   <br>(i) Individual performing service each day by hour and quarter of an hour;
   <br>(ii) Type of services performed each day by hour and quarter of an hour; and
   <br>(iii) Hourly rate for each service so detailed;
<br>(5) Any applicable payment discount terms; and
<br>(6) Total amount billed.

##### 5.7.2 Procedures for Payment
The government intends to make payment to the Contractor via charge card as outlined in accordance with (IAW) FAR 52.232-36, Payment by Third Party. Pursuant to IAW FAR 32.1108(b)(2)(ii), the contracting officer shall not authorize the Governmentwide commercial purchase card as a method of payment during any period the System for Award Management (SAM)  indicates that the Contractor has delinquent debt subject to collection under the TOP. In such cases, payments under the contract shall be made in accordance with the clause at 52.232-33, Payment by Electronic Funds Transfer-System for Award Management, or 52.232-34, Payment by Electronic Funds Transfer-Other Than System for Award Management, as appropriate (see FAR 32.1110(d)).

##### 5.7.3 Payment by Governmentwide commercial purchase card
The Contractor shall submit invoices not more frequently than once per month. Payment shall be made in accordance with the clause found at FAR 52.232-36, Payment by Third Party. The Contractor shall make payment requests through a charge to the Government account with the third party, at the time and for the amount due in accordance with those clauses of this contract that authorize the Contractor to submit invoices, contract financing requests, other payment requests, or as provided in other clauses providing for payment to the Contractor.

On each invoice, the Contractor shall provide a summary of each billed CLIN. The summary shall include by each invoiced CLIN: CLIN number and description, as well as the invoiced amount. The invoice shall also provide a total amount, across all CLINs, billed to date. The Contractor shall not bill, nor be reimbursed, for any charges that are not specifically stated in this task order or incorporated via a written modification issued by the CO.

Please note, the payment via purchase card is rescinded should the Contractor's System for Award Management (SAM) registration indicate that the Contractor has delinquent debt that is subject to collection under the Treasury Offset Program (TOP).

##### 5.7.4 Electronic Funds Transfer Method
The Contractor shall submit invoices not more frequently than once per month. Payment shall be made in accordance with the clause found at FAR 52.212-4 Contract Terms and Conditions – Commercial Items (Nov 2021), paragraph(g), following receipt of properly executed invoices prepared in accordance with the requirements of this task order.

On each invoice, the Contractor shall provide a summary of each billed CLIN. The summary shall include by each invoiced CLIN: CLIN number and description, as well as the invoiced amount. The invoice shall also provide a total amount, across all CLINs, billed to date. The Contractor shall not bill, nor be reimbursed, for any charges that are not specifically stated in this task order or incorporated via a written modification issued by the CO.

The Contractor has the option to submit an electronic or hard copy original invoice for payment to GSA Financial Information & Operations Division.

Electronic Invoices are encouraged and may be submitted to the following address:
https://vcss.ocfo.gsa.gov/

Invoices may also be submitted in lieu of electronic submission to:

USDA-OCFO
<br>Financial Information & Operations Division
<br>Financial Operations & Disbursement Branch
<br>2300 Main Street – 2SE
<br>Kansas City, MO 64108
<br>Tel: (800) 676-3690/(816) 926-7287
<br>Fax: (816) 926-5189

A duplicate electronic invoice with supporting documentation shall be sent electronically to the COR and CO. The COR will confirm performance made against the invoiced line items to ensure that the correct amounts have been billed and will document any price deductions. The COR will then certify and provide a signature indicating that the invoice is valid for payment. Invoices are authorized for payment upon the Government’s receipt and acceptance of deliverables specified in the task order and the receipt of a valid invoice. Invoices shall be rendered no later than the 15th calendar day of the month following performance and must be accompanied by all status reports submitted during that period. The COR must receive a copy of the invoice and all supporting documentation (i.e. list of daily hours worked by each of the vendor’s employees (also summed up as weekly and monthly for each person) before or at the same time as the GSA Finance Office. All final invoices must be submitted no later than thirty (30) calendar days after the last day of the month for which the charges, either labor and/or ODCs, were incurred. The Contractor may invoice only for hours, travel, and/or unique services ordered by GSA and actually used in direct support of the program office for this task order.

Invoices must include the following:
<br>(1) Name and address of the Contractor
<br>(2) Invoice date and number
<br>(3) GSA Multiple Award Schedule (MAS) Information Technology Professional Services Contract Number, line item number and, if applicable, the order number
<br>(4) Description, quantity, unit of measure, unit price and extended price of the items delivered
<br>(5) Shipping number and date of shipment, including the bill of lading number and weight of shipment if shipped on a Government bill of lading
<br>(6) Terms of any discount for prompt payment offered
<br>(7) Name and address of official to whom payment is to be sent
<br>(8) Name, title, and phone number of person to notify in event of defective invoice
<br>(9) Taxpayer Identification Number (TIN). The Contractor shall include its TIN on the invoice only if required elsewhere in this contract
<br>(10) Electronic funds transfer (EFT) banking information

Note: Failure to comply with the procedures outlined above may result in the invoice being rejected, or your payment being delayed.

#### 5.8 Limitation of Funds 

The Contractor shall notify the CO in writing when it has reason to believe that the costs it expects to incur under this contract in the next 60 days, when added to all costs previously incurred, will exceed 75 percent of (1) the total amount so far allotted to the contract by the government. The notice shall state the estimated amount of additional funds required to continue performance for the period specified in the contract. 

Sixty days before the end of the period specified in the contract, the Contractor shall notify the CO in writing of the estimated amount of additional funds, if any, required to continue timely performance under the contract or for any further period specified in the contract or otherwise agreed upon, and when the funds will be required.

### 6.0 Instructions and Evaluation

#### 6.1	Submission Instructions

##### 6.1.1 	Before submitting a quote - Questions and Answers 
**Questions**
<br>Submit all questions concerning this RFQ through this Google form. All questions must be submitted by the deadline provided on page 1 of this RFQ.

Questions should clearly express the Contractor’s issues or concerns and must follow the format provided in the Google form. Statements expressing opinions, sentiments, or conjectures are not considered valid inquiries and will not receive a response. Further, Contractors are reminded that the government will not address hypothetical questions aimed at receiving a potential “evaluation” decision.

Answers will be provided as an amendment to the solicitation three business days after the deadline for questions. 

##### 6.1.2 Submission checklist
All responses must be submitted using this Google form and include the following materials:

**Technical Submission:**
- [ ] Technical approach - **4 pages** maximum, including diagrams, 12-point font
- [ ] Maximum of 2 code repositories with a short description about the project for each code repository 
- [ ] Staffing plan - **3 pages** maximum, including diagrams, 12-point font
- [ ] Resumes and letters of intent from designated key personnel (if not currently employed by Contractor)
- [ ] User research plan if not included in the code repository
- [ ] Conflict of Interest (form to sign)
- [ ] FAR 52.204-24 Provision (checkbox on Google form)

**Price:** 
Price responses must be submitted using the google form provided) and include the following materials:
- [ ] Price Quote (spreadsheet)

**Interviews:**
The government reserves the right to hold oral interviews.  If the decision is made to hold interviews, Contractors will be notified and held in accordance with “Interviews” under **6.2 Instructions for Proposals** The oral interview does not require Contractors to submit any materials.
Applies to all phases: **Only submit information explicitly requested in this RFQ.** Do not include assumptions, caveats, or exceptions in any part of your submission. Failing to follow these instructions may result in removal from consideration for the award.


#### 6.2	Instructions for Proposals
##### 6.2.1 Technical Submissions
Technical submissions must consist of a technical proposal of no more than four (4) pages, a staffing plan of no more than three (3) pages plus resumes and signed letters of intent to participate, and references to two source code samples, preferably open source. Technical proposals and staffing plans must be submitted using 12-point type.

The technical proposal must set forth the Contractor's proposed approach to providing the services required, including programming language(s) the Contractor proposes to use. The technical proposal must also make clear that the Contractor understands the details of the project requirements. The technical proposal must also identify potential obstacles to efficient development and include plans to overcome those potential obstacles. The technical proposal must also include a description of the Contractor's plans, if any, to provide services through a joint venture, teaming partner, or subcontractors.

The staffing plan must set forth the Contractor's proposed approach to staffing the requirements of this project, including the titles of each of the labor categories proposed and proposed level of effort for each member of the Contractor's development team. The staffing plan must also identify the proposed Project Manager and proposed Technical Lead by name, and include a resume for each. Those resumes must include a brief description of the experience and capability for each individual, but cannot exceed one (1) page in length each. Contractors proposing Key Personnel who are not currently employed by the Contractor or a teaming partner must include a signed letter of intent from the individual proposed as Key Personnel that they intend to participate in this project for at least one (1) year. The staffing plan must also set forth the extent to which the proposed team for this project was involved in the development of the source code referred to in the next paragraph.

The staffing plan must set forth and explain the extent to which the Contractor will provide individuals with experience in at least each of the following areas:
- Agile development practices
- Automated (unit/integration/end-to-end) testing
- Continuous Integration and Continuous Deployment
- Application Protocol Interface (API) development and documentation
- Open-source software development
- Cloud deployment
- Building and testing public facing sites and tools

The references to one or more source code samples must be either links to Git repositories (either credentialed or public) or to equivalent version-controlled repositories that provide CCCM with the full revision history for all files. If an Contractor submits a link to a private Git repository hosted with GitHub, CCCM will provide the Contractor with one or more GitHub user identities by email, and the Contractor will be expected to promptly provide the identified user(s) with access to the private Git repository.

The source code samples should be for projects that are similar in size, scope, and complexity to the project contemplated here. The source code must have been developed by either (i) the Contractor itself, (ii) a teaming partner that is proposed in response to this RFQ, or (iii) an individual that is being proposed as Key Personnel for this project. 

##### 6.2.2 Price Submissions
Price submissions must set forth a single dollar amount that represents the Contractor's estimate of the total cost to CCCM for the development services for a base 12 month and 2 option periods. [Instructions on providing price proposal, typically an excel workbook, will be included in the final RFQ]. CCCM expects that the labor categories and staffing levels set forth by the Contractor in the Excel workbook will be consistent with the Contractor's staffing plan.

The Contractor will be compensated at loaded hourly rates. CCCM intends to evaluate proposals and award based on initial proposals, and therefore the Contractor's initial proposal should contain the Contractor's best terms. 

#### 6.2.3 Interviews
Each interview will be conducted remotely via video connection and/or teleconference. CCCM will communicate with certain Contractors to schedule the dates and times of interviews.

Each interview will include an unstructured question and answer session, during which Contractors will be asked questions about the technical aspects of their proposal and their approach to software development. CCCM expects these interviews will assist CCCM to assess the technical abilities of the proposed development team and to better understand the proposed technical approach described in the Contractor's written submission. Both of the Contractor's proposed Key Personnel must participate in the interview.

The Introductions phase of each interview will last approximately 5 minutes, during which the Contractor and CCCM interview team members will introduce themselves.

The Open Technical Session of each interview will last approximately 45 minutes, during which the Contractor interview team will respond to CCCM’s questions related to the technical aspects of the Contractor's proposal. Contractors will NOT be able to use or present any slides, graphs, charts, or other written presentation materials, including handouts. There will be no follow-up session for further questions after this part of the interview.

The Closing Remarks phase of each interview will last approximately 5 minutes, during which the Contractor may make a short presentation summarizing the Contractor's responses to CCCM’s questions.
Interviews will not constitute discussions. Statements made during an interview will not become part of the agreement.

#### 6.2.4 Basis of Award and Evaluation Factors
Each submission received by CCCM will be evaluated for technical acceptability. Submissions that are determined to not be technically acceptable after the Contractor has been given the opportunity for a clarification will not be evaluated further.

Quotes must be realistic with respect to technical approach, staffing approach, and total price. Quotes that indicate a lack of understanding of the project requirements may not be considered for award. Quotes may indicate a lack of understanding of the project requirements if the staffing plan does not use a realistic mix of labor categories and hours, or if any proposed hourly labor rates are unrealistically high or low.

CCCM will evaluate quotes that are technically acceptable on a competitive best value basis using a trade-off between technical and price factors. Technically acceptable submissions will be evaluated based on four (4) evaluation factors. These factors are:
<br>(1) technical approach,
<br>(2) staffing approach, 
<br>(3) similar experience, and 
<br>(4) price. 

<br>The three (3) technical, non-price evaluation factors, when combined, are significantly more important than price. CCCM may make an award to an Contractor that demonstrates an advantage with respect to technical, non-price factors, even if such an award would result in a higher total price to CCCM. The importance of price in the evaluation will increase with the degree of equality between Contractors with respect to the non-price factors, or when the Contractor's price is so significantly high as to diminish the value to CCCM of the Contractor's advantage in the non-price factors.

#### 6.2.5 Technical Approach
In evaluating a Contractor's technical approach, CCCM will consider (a) the quality of the Contractor's plans to provide the open source, agile development services required, (b) the extent of the Contractor's understanding of the details of the project requirements, and (c) the extent to which the Contractor has identified potential obstacles to efficient development, and has proposed realistic approaches to overcome those potential obstacles.

#### 6.2.6 Staffing Approach
In evaluating a Contractor's staffing approach, CCCM will consider (a) the skills and experience of the Key Personnel and other individuals that the Contractor plans to use to provide the required services, (b) the mix of labor categories that will comprise the Contractor's proposed development team, and (c) the Contractor's proposed number of hours of services to be provided by each member of the Contractor's proposed development team.

#### 6.2.7 Similar Experience
In evaluating a Contractor's similar experience, CCCM will consider the extent to which the Contractor has recently provided software development services for projects that are similar in size, scope, and complexity to the project described in this RFQ, and the quality of those services. In evaluating the quality of those services, CCCM will consider, among other things, the revision history for all files in the source code samples provided. In considering a Contractor's similar experience, CCCM may also consider information from any other source, including Contractor's prior customers and public websites.

#### 6.2.8 Price
In evaluating a Contractor's price, CCCM will consider the total of the Contractor's estimated costs for the development services for the base and two option periods.

