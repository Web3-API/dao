# PWV Consultants - Engagment 1
## Billing Summary
| Deliverable | Time Estimate | Hourly Rate | Billing Estimate |
|-|-|-|-|
| **Build Pipeline Audit** | 32 hrs | $165/hr | $5,280 |
| **Environment Variables Spec** | 36 hrs | $165/hr | $5,940 |

**Total Estimate: $11,220 for 68 hours**

## Scope Of Work
### Build Pipeline Audit
#### Summary
Assist with and audit a reproducible build system leveraging docker containers to ensure the environment is identical for each build. As there is a draft pull request for this functionality, PWV would provide a detailed audit based on that pull request. 

#### Detailed Deliverables
Code review, and audit will be combined into a report for review. The report includes the following elements:

* **Security**
    * Report of security issues involving container or software installed used.
    * Implementation doesn't leak any variables.
* **Developer Happiness**
    * Implementation follows industry best or common practices.
    * Implementation follows current established patterns used in the code base.
* **Docker**
    * Implementation using appropriate images for implementation.
    * Optimize docker build for smallest image size.
    * Identify issues that may arise from non-deterministic sources.
* **Future-Proof**
    * Identify Issues that may arise in current implementation.
    * Identify extensibility of current implementation for future development.
* **Alternate Solutions**
    * Identify cons and pros of other methods that could be used to achieve the same goal.

### Environment Variables Spec
#### Summary
There is a need to provide environmental variables that can be used for stateless WASM builds that currently require configuration in multiple code locations - ‘configuration hell’. The current thought is to provide access to these environmental variables by implementing their definition in the graph schema files, and then allowing the users to set these variables when initializing the APIs. This avoids the need to continue to send the same variable through arguments in each of the API methods. See https://github.com/Web3-API/monorepo/issues/140

#### Detailed Deliverables
Architecture Plan will be delivered along with estimates and paths for execution and development of the following features:

* **Environment Variables**
    * Known Requirements:
        * Implementation shall avoid 'configuration hell' - should only have to set variables at a high level without having to re-implement changes throughout the code.
        * Environmental variables can be configured to be required or optional.
        * Variables can be configured to be set at initialization, or at query time depending on configuration.

An architecture plan will lay the roadmap for further execution and development that includes the following elements:
* **Introduction**
    * This section will outline Background Context, Scope, and Requirements.
* **Technical Plan**
    * This section breaks down each component of the architecture of the project describing what and how and why.
* **System Diagram (network topology)**
    * This lays out the physical and cloud infrastructure components and how they relate to each other.
* **Component Diagram**
    * This lays out the individual components. For instance a Data Decryption component - where it lives within the system.
* **Component Flow**
    * Outlines how the components communicate with each other.
* **Sequence**
    * Lays out the literal steps in the processes from component to component via a real-world scenario(s).
* **Data Lifecycle Diagram**
    * This outlines the state the data is in.
* **Data Transfer Flow Diagram**
    * This will show the timing of how data flows around and through what protocols.
* **Tools/Stack/Protocols**
    * Shows inventory of all things being used, and what other alternate plans/methods were considered.
* **Reasoning and Determining**
    * Why we choose this path, usually related to pen and paper testing or scenario breakdowns.
* **Providers**
    * Third parties or vendors we source from (cloud/DC/physical).
* **Deployment/Release**
    * How this will get out into the real world as a POC.
* **Component/Time Breakdown**
    * Estimate of hours for each component of the technical plan.
* **Hard Cost Estimate Schedule**
    * Supplemental Document (usually a spreadsheet) as needed.
* **Delivery**
    * How deliverable of the real world POC will be delivered.
* **Questions:**
    * Any outstanding questions or known unknowns. Additional information and or sections are often added depending on the project needs as they develop. Plans are typically 30-150 pages depending on what is sufficient to document what needs to be understood to build the project. The plan is typically presented as a PDF that we review in at least one meeting and then discuss in further meetings and revise for specificity. We have and can on request also modify the plan into a brief slide deck that isolates most of the diagrams, lists, and schedules.

## Billing Details
$5,610 USDC due upfront, the remaining balance will be confirmed based on actual hours worked and paid out upon completion.

**Payment Address (USDC Only):** 0x663995638d14995cE862e5Aa8af5FC1B826Dc54b

## About You
### PWV Consultants
PWV Consultants is a boutique group of industry leaders and influencers which hail from the digital tech, security and design industries. We gravitate toward the complex. We have the ability to do almost anything in software-enabled technology. We aim to give our clients access to assets who might otherwise be unavailable to them, through our group of highly skilled US-based consultants.

### Managing Partner
Pieter VanIperen, Managing Partner at PWV Consultants, is a veteran software architect and security expert who is an industry authority and influencer providing thought leadership and execution to develop widely adopted processes, methodologies, and technologies that are at the forefront of digital innovation and software development.

As a 20-year software engineering veteran, he has founded or co-founded several companies, acted as trusted advisor and mentor to numerous early stage startups, held the titles of software executive and software security executive, consultant and professor. His expert consulting and advisory work spans several industries in finance, media, medical tech, and defense contracting. He authored the highly influential precursor HAZL (jADE) programming language as well.

Most recently, at PWV Consultants, Pieter leads a boutique group of industry leaders and influencers from the digital tech, security and design industries. Becoming trusted technical partners for many Fortune 500 companies, high-visibility startups, universities, defense agencies, and NGOs.

Formerly, Pieter held the title of SVP - Global Head of Cloud Security at a major media conglomerate, positions as Cloud and Security Consultant for a national consumer insurance company, national bank, and others. Prior to that he was a resident innovation and automation software architect, and a secure coding expert for a major online discount brokerage.

He is a Certified Penetration Testing Engineer/Ethical Hacker, Secure Web Application Engineer, Network Forensics Examiner, Cloud Security Officer, and Information Systems Security Officer.

Pieter also provides consulting services to multiple law enforcement institutions as an InfoSec expert on a volunteer basis and serves as an Adjunct Professor of Code Security at New York University (NYU) teaching Secure Coding for Coders.
