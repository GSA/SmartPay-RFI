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

The website received more than 1.8 million visitors (mobile & web) in FY22. Based on current content and development in progress, the government anticipates that traffic will be driven by state sales tax content and visits to the Section 889 Representations tool).

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
