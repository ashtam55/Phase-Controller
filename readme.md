## 3 Phase Controller - SOW
Document prepared by Ashtam Singh

## Table of Content

* Executive Summary
* Project Definition
* Devices
* Web/Soft-ware
* Maintenance
* Exclusions
* Deliverables
* Customer Responsibilities
* Investment and Cost
* Acceptance Criteria
* Assumptions
* IPR
* Approvals


## Executive Summary
This documentation is to serve as a 'Statement of Work' or SOW for the software development of 3 Phase Controller POC to enable home user to control and monitor electric appliances. 

The advancement in the field of IoT  Networks, Computing and Data Science has made possible Integrated systems which enable new experiences and solutions possible in the Automation space.
Such a system would include a means to capture, catalogue and analyze data, along with tools to enforce 'business logic'.

This SOW summarizes the Software development of 3 Phase Controller system which can be directly managed via end user application, these `on-premise` Hardware devices running 3 Phase Controller Software(aka edge device firmware) which would include (at least) the following:
* WIFI Provisioning with reconnect routine.
* Autonomous monitoring of Voltage & Current to trigger the relay when Voltage/Current goes min-max threshold values.
* Local Potential Free as Input to triggers the relay.


Akriya Technologies will work with 3 Phase Controller to:

* Software Development of the `on-premise` Edge Devices.
* End User mobile application.
* Provide documentation of the new system
* Knowledge Transfer/Integrate 

Akriya Technologies proposes to design, develop and provide installation of v1.0 of the proposed system to cater for 1 `on-premise` device.
This activity will require 4-6 weeks. The estimated cost for this activity would be 1.50 lakhs INR plus additional charges including travel, server rental and hardware costs (if any).


The Value Proposition of using Akriya Technologies for this project are:
* Proven engineering techniques for making Integrated systems.
* Leveraging our experience in working with IoT toolkit (ESP).
* Data Architecture and Solution experience
* Using our subject matter experts to complete the project quickly. Rapid project completion minimizes disruptions and allows organizations to realize cost-saving quickly.

## Project Definition
The 3 Phase Controller project is broken down into the following 5 modules, which would be developed in the course of this work.
These modules are abstracted based on functional and operating hardware (cloud functions, user functions and on-premise functions).

### 1.1 Wifi Provisioning H/W 
This module is the Hardware device function running to ensure isDeviceConnected to wifi provided via the Mobile App using BLE.
The module regularly check the Wifi connectivity and reconnects if not connected. This module needs to be triggered via app or manually by pressing a button for 5 second.

### 1.2 Autonomous Monitoring H/W
This module is responsible for collecting and storing current and voltage on three phases.

### 1.3 Real-time User Switching H/W
The module is responsible for taking Real-time decisions of which relay to trigger, based on threshold values of Current & Voltage set by default.

This would include:
* Implementations and deployment of Communication channel for devices (MQTT).
* User account management ( Firebase ).

### 1.4 Mobile Application S/W
This module is a running on end-user machines which includes
* Start the Device in Online mode or Offline mode.
* In Offline mode, User device should be on same network for monitoring and controlling devices.
* In Online mode, User trigger the module 1.1 on device and device gets connected to Internet.
* Dashboard Homepage to use the `on-premise` devices.

## Delivery Scope
### Devices/HW

* On-Premise Module 

```
Data to Capture:    Live Current , Potential Difference , Local Potential Free Input

```


## Web/Software
* Data SDK / APIs for 3 Phase Controller Telemetry
We will be recording and cataloguing the real-time telemetry of the 3 Phase Controller on-premise devices and Users.
This would include a query endpoint, to query this set.

* User App

## Maintenance
To be maintained for 1 months and then rediscuss based on new requirements and learnings.

## Exclusions
The followings are excluded from the project scope
* The packages used and maintained by Akriya Technologies for interfacing with IoT Devices.
* Open Source Software means publicly available software that may be utilized pursuant and subject to the terms of an "open source" or similar license, including without limitation the "Ruby License," the "MIT License," the "Apache License" and the "GNU General Public License." Company understands and agrees that Consultant may, at Consultant's discretion, make use of libraries from various Open Source Software products during the course of work. We may submit back to such libraries any improvements ("patches") made to the Open Source Software during the course of work, as long as the submission of such patches violates neither the conditions in this Section nor the Confidentiality provisions.

## Deliverables
The deliverables are listed below.
* Device. 
Hardware Device ( provided by the client ) with 3 Phase Controller Firmware installed.

* Software
Access top-level Git repositories for the SDK, on-premise firmware, and mobile app package.

* Documentation and graphical depictions of the new proposed 3 Phase Controller system.


## Customer Responsibilities
* The nature of this engagement dictates that Akriya Technologies receive a frequent and enthusiastic response from the appropriate personnel.
* A weekly review between the Akriya Technologies consultant and the Verteon Renewables (I) Pvt. Ltd project lead or his designate will ensure that the expectations of this engagement are met.
* Client will assign a key contact who will be responsible for providing Akriya Technologies with information, access to personnel, and facility access.
* Client will provide a work area space with desk, chair, Internet access for use by Akriya Technologies to conduct project business while working on-site.

## Investment and Cost (revised)
* Time required: 4-6 weeks: 1.50 lakh INR (estimated 140 man-hours)

* Hardware cost (if required) to be paid by Client
    
* Server/Web hosting charges:
    * 60$ / month = 4000 INR

* Bill separately for travel costs will be billed at actual cost and will not exceed 10,000 INR for the entire project for movement within NCR. (upto 10 meetings)

 * Payment Schedule

| Milestone                                 | Percentage    | Amount    | Time period from Start
| -------------                             |:-------------:| -----:    | ----- | 
| Requirement Finalization + SOW acceptance                 | 50%            | 75,000 INR| 0 day | 
| Module 1.1 - 1.2          | 25%           | 37,500 INR| 15 days |  
| Modele 1.3 - 1.4                 | 25%          | 37,500 INR| 28 days |


Devices cost to be paid on the day of installation.
Server cost to be paid directly or at the start of each month.
Travel reimbursements as and when declared.

## Acceptance Criteria
At the conclusion of this evaluation, all deliverables for this phase will be presented to Verteon Renewables (I) Pvt. Ltd for review.

Verteon Renewables (I) Pvt. Ltd or its representative will have five business days from the date of delivery of any document that is a deliverable to review it and request any changes.  If Akriya Technologies does not receive notification of any required changes within this period, the document will be deemed to have been accepted without modification and will be reissued as a final copy.

If Akriya Technologies is notified by Verteon Renewables (I) Pvt. Ltd, within the above time frame, of any changes required, Akriya Technologies will within two business days of such notification implement those changes as have been agreed between the parties.  A final copy of the document will then be submitted to Verteon Renewables (I) Pvt. Ltd.

## Assumptions
* General
    * All documentation created for this project will be available in hard copy and electronic format.
    * Any modifications to the scope of work will be handled through a change control process and will be agreed to by both parties.

* Commercial
    * Additional costs may be incurred where any delay not under the control of Akriya Technologies that causes Akriya Technologies personnel to not fulfil their scheduled tasks.
    * An authorized delegate of Verteon Renewables (I) Pvt. Ltd will be available at the time of completion of the build phase so that all documentation can be accepted and signed.
    * Additional costs may be incurred where any work scheduled to be undertaken by Akriya Technologies is postponed by Verteon Renewables (I) Pvt. Ltd after 24 hours of its commencement.
    * All changes to the schedule or technical requirements must be provided to Akriya Technologies in written format. Email is included as written format. Receipt of all correspondence should be confirmed by phone wherever possible.
    * Verteon Renewables (I) Pvt. Ltd has accepted the costs/times estimate as detailed in this document
    * Verteon Renewables (I) Pvt. Ltd has accepted the Akriya Technologies standard terms and conditions linked.
    * Any deviationns, technical or commercial , shall be mutually discussed and agreed before implementation.

## Intellectual Property
Unless otherwise agreed in writing, Verteon Renewables (I) Pvt. Ltd acknowledges that all intellectual property rights attaching to the products or arising out of the provision of services are and will remain the property of Akriya Technologies (or its suppliers, where such rights are owned by that supplier).

The software will be licensed to Verteon Renewables (I) Pvt. Ltd on the terms of the relevant license agreement provided with the product or as otherwise agreed between Akriya Technologies and Verteon Renewables (I) Pvt. Ltd in writing.


## Approved by
Name:   
Date:   
Position:   

[PhaseOperator system doc]()