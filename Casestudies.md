#### Case Study :1 

-----

Introducing Mutual Fund Investors Club  (Mutual Fund Investors Club) is a Mutual Fund Purchase  and Advisory agency that was created to change the way people make decisions about  purchasing Mutual fund  and other related services around the world. To do so, they are developing an online service where every detail of a  Mutual Fund purchase  will be assisted by a club of experts specifically selected for each Mutual Fund. 
The concept of this platform is that you user can be both a Purchaser and a Mutual Fund  expert at the same time. The more you participate as an expert in a Mutual Fund  Type , the higher the points you will score. These points can be redeemed to pay SIP.
The customer came with the following requirements for the platform. 

##### Common user view:

- Promotional Mutual Fund  Info on the home page
- Search for Mutual Funds
- Details for Each Mutual Fund
  - Buy a Mutual Fund
  - Buy a Mutual  with a club of experts included:
    - Comment on your experience
    - Ask an expert
    - Evaluate an expert
- Register as a common user
- Mutual Fund expert view:
  - The same view as the common user view
  - Answer the questions asking for  Mutual Fund expertise
- Manage the points you scored answering questions:
  - Exchange points for SIP
- Administrator view:
  - Manage Mutual Funds
  - Manage common users
  - Manage Mutual Fund Experts



#### Case Study : 2

-------------------

The Feature Mesh software system will be a Cloud native feature store . This system will be designed to maximize the Data Scientists productivity by providing a platform to assist in feature engineering where the push and the pull of features from the platform is provided as a service along with other value-added functionality described later in the document. By maximizing the data scientist’s and Data Engineer’s work efficiency and production the system will meet their needs while remaining easy to understand and use.

##### UseCases

- The Data Scientist accesses the platform and publishes the built feature on the platform

  - The user specifies metadata for the features that would be used while searching.
  - The user leverages the GUI or the library to push the developed feature onto the platform.
  - The system displays the status message of the push operation to the user.

- The Data Scientist accesses the platform and searches for the intended feature from the platform.

  - The user chooses to search by feature name, keyword, timestamp etc.
  - The system displays the choices to the user.
  - The user selects the desired feature from the search results.
  - The system presents the abstract of the feature to the user.
  - The user chooses to re-use the feature.
  - The system provides the requested feature.

   

-  The Data Scientist accesses the platform and uses the published feature for model training using the offline store within the platform. 

  - The user leverages the built library from featuremesh to get the values of a feature for training the analytical model in his environment (i.e: Jupyter-Notebook etc)
  -    The query parameters for the library call would include the feature Name and any other associated meta-data of the feature.
  -  The system responds back with either a success status with associated feature value or an Error
  -  The user has to program to catch any exceptions/errors thrown by the platform.
  -  The workload for Offline store typically would involve Batch processing.

   

-  Platform that facilitates real time feature consumption for inferencing done by the analytical model deployed in production.

- Develop a Library and/or use GUI is built in to the platform for Data Scientists to use.

 ·   

#### Case Study : 3

----

A global investment bank based in India, New York and Singapore trades (buys and sells) financial products with other banks (“*counterparties*"). When share prices on the stock markets move up or down, the bank either makes money or loses it. At the end of the working day, the bank needs to gain a view of how much risk of losing money they are exposed to, by running some calculations on the data held about their trades. The bank has an existing Trade Data System (TDS) and Reference Data System (RDS) but needs a new Risk System.

 

**Trade Data System (TDS)**

The Trade Data System maintains a store of all trades made by the bank. It is already configured to generate a file-based XML export on a network share of trade data at the close of business (5pm) in NewYork. The export includes the following information for every trade made by the bank: 

• Trade ID, Date, Current trade value in US dollars, Counterparty ID

**Reference Data System (RDS)**

The Reference Data System maintains all of the reference data needed by the bank. This includes

Information about counterparties; each of which represents an individual, a bank, etc. A file-based XML

Export is also available on a network share and includes basic information about each counterparty. A new organization-wide reference data system is due for completion in the next 3 months, with the current system eventually being decommissioned

 

The high-level requirements for the new Risk System are as follows.

 Import trade data from the Trade Data System and Import counterparty data from the Reference Data System. Join the two sets of data together, enriching the trade data with information about the Counterparty, for each counterparty, calculate the risk that the bank is exposed to. Generate a report that can be imported into Microsoft Excel containing the risk figures for all counterparties known by the bank.

 Distribute the report to the business users before the start of the next trading day (9am) in

Singapore. Provide a way for a subset of the business users to configure and maintain the external parameters used by the risk calculations.
Additional Requirements with Financial Risk System

a.    Risk reports must be generated before 9am the following business day in Singapore.

b.    The system must be able to cope with trade volumes for the next 5 years.

c.    The Trade Data System export includes approximately 5000 trades now and it is anticipated that there will be slow but steady growth of 10 additional trades per day

d.    The Reference Data System export includes approximately 20,000 counterparties and growth will be negligible

e.    There are 40-50 business users around the world that need access to the report.

f.     Risk reports should be available to users 24x7, but a small amount of downtime (less than 30 minutes per day) can be tolerated

g.    Manual failover is sufficient, provided that the availability targets can be met.

h.    This system must follow bank policy that states system access is restricted to authenticated and authorized users only

i.     Reports must only be distributed to authorized users

j.     Only a subset of the authorized users are permitted to modify the parameters used in the risk calculations

k.    Although desirable, there are no single sign-on requirements (e.g. integration with Active Directory, LDAP, etc)

l.     All access to the system and reports will be within the confines of the bank’s global network.

m.   The following events must be recorded in the system audit logs

​                                i.   Report generation

​                               ii.   Modification of risk calculation parameters

​                              iii.   It must be possible to understand the input data that was used in calculating risk.

n.    The system should take appropriate steps to recover from an error if possible, but all errors should be logged

o.    Errors preventing a counterparty risk calculation being completed should be logged and the process should continue

p.    All user interfaces will be presented in English only

q.    All reports will be presented in English only

r.    All trading values and risk figures will be presented in US dollars only

s.    A Simple Message trap should be sent to the bank’s Central Monitoring Service in the following circumstances

​                                i.   When there is a fatal error with a system component

​                               ii.   When reports have not been generated before 9am Singapore time

t.    Input files used in the risk calculation process must be retained for 1 year

u.    Interfaces with existing data systems should conform to and use existing data formats.

### Case Study : 4

---

NewYork City Corporation (NCC) is facing budget shortfalls and needs to cut costs. NCC Mayor has hired your team to streamline the NCC's Office of Management and Budget (OMB). When a NCC employee needs to purchase something for more than a few thousand INR, the OMB issues a Request for Proposals (RFP) in the local newspaper. Businesses bid on the RFPs and the OMB awards a contract based on the competitiveness of the bid and other factors. The OMB monitors more than 500 active contracts and RFPs for everything from toilet paper to medical supplies to basketballs. The OMB manages all this data in spreadsheets.
Mayor hopes modernizing the OMB will improve a few strategic areas.
• Over half of all RFPs have a single bid. The NCC is potentially overpaying for lower-quality services.
• Finalizing a contract takes months. Many businesses get lost in the multistep process.
• Publishing a new RFP takes up to 6 weeks. This process must be faster.

Mayor  hired your team and team report to him, but the Office of Management and Budget receives policy direction from both the mayor and NCC council.

Some local businesses rely on lawyers to navigate the Request for Proposal process. Different interaction patterns for the potential software might exist, which could influence the architecture.
The Office of Management and Budget (OMB) sits at the center of several key user interactions, but they aren’t paying the bills. We should talk to the OMB directly. It’s possible that the mayor and city council have budgeted for a system that does not solve the OMB’s real problems

There’s a small number of users, but when a user submits a question or problem system should  be able to respond quickly, within a business day. Releases happen at least once a month. Ideally, team will  ship code as it is ready. report errors.  We need to verify that the RFP index is built correctly. The verification should be automated. We need a new, permanent dev team to come up to speed quickly after the current team of contractors we’ve hired leaves

When the RFP database does not respond, System should log the fault and respond with stale data within 3 seconds. A user’s searches for open RFPs and receives a list  of RFPs 99% of the time on average over the course of the year. New servers can be added during a planned maintenance window (less than 12 hours). A user sees search results within 5 seconds when  the system is at an average load of 2 searches per second. Updates to RFPs should be reflected in the application within 24 hours of the change A user-initiated update (for example, starring an Low RFP) is reflected in the system within 5 seconds. The system can handle a peak load of 100 searches Low per second with no more than a 10% dip in average response times. Data growth is expected to expand at a rate of 5% Low annually. The system should be able to grow to handle this with minimal effort.

### Case Study 5

---

Britaan is a global cheese manufacturer and they sale the cheese brand named “Good Cheese” in Germany. Over the past one year, there has been more recalls in the “Good Cheese” brand. The major reason broadcasted in the news channels and newspapers is that the cheese packets manufactured outside Germany were only recalled. Britaan’s cheese factories outside Germany don’t have stringent quality check measures compared to the Britaan’s German cheese factories. The sale of “Good Cheese” in Germany have declined drastically over the past few months as the consumers don’t have the trust about where the cheese packets were manufactured. 

To regain the trust of the cheese consumers in Germany and re-establish their “Good Cheese” brand, Britaan wants to implement IT  solution. The IT solution will track the packed cheese products from the time it’s manufactured in the Britaan’s cheese factories till the time it’s delivered to the retail stores. The cheese packets reach to multiple different retail stores through the distributors. The distributors receive the cheese packets from Brittan by scanning the bar code on the cheese packets and takes the ownership of the packets with them. The retailers scans the barcode of the cheese packets from the distributors to transfer the ownership from the distributor to the retailer.

 The entire jouney of ownership transfers of the cheese packets from the Britaan’s factories to the retailers are tracked on IT solution to convince the German cheese consumers that the cheese they consume is indeed manufactured in Germany.



### Case Study 6

---

Meetup is an organization, plans to launch the Conference Management System, a new online service that will enable other companies or individuals to organize and manage their own conferences and events.

The Conference Management System application is one of the first innovative online services that Meetup wants to take to market. As a startup, Meetup wants to develop and launch these services with a minimal investment in hardware and IT personnel. Meetup wants to be quick to market in order to start growing market share, and cannot afford the time to implement all of the planned functionality in the first releases. Therefore, it is important that the architecture it adopts can easily accommodate changes and enhancements with minimal impact on existing users of the system. Meetup has chosen to deploy the application on Windows Azure in order to take advantage of its ability to scale applications as demand grows

Meetup plans to build an online conference management system that will enable its customers to plan and manage conferences that are held at a physical location. The system will enable Meetup’s customers to:

• Manage the sale of different seat types for the conference.

• Create a conference and define characteristics of that conference.

The Meetup Conference Management System will be a multi-tenant, cloud-hosted application. Busi­ness customers will need to register with the system before they can create and manage their confer­ences.

The business customer defines the number of seats available for the conference. The business cus­tomer may also specify events at a conference such as workshops, receptions, and premium sessions for which attendees must have a separate ticket. The business customer also defines how many seats are available for these events. The system manages the sale of seats to ensure that the conference and sub-events are not oversubscribed. This part of the system will also operate wait-lists so that if other attendees cancel, their seats can be reallocated. The system will require that the names of the attendees be associated with the purchased seats so that an on-site system can print badges for the attendees when they arrive at the conference.

A business customer can create new conferences and manage information about the conference such as its name, description, and dates. The business customer can also make a conference visible on the Meetup Conference Management System website by publishing it, or hide it by unpublishing it.

Additionally, the business customer defines the seat types and available quantity of each seat type for the conference.

Meetup also plans to enable the business customer to specify the following characteristics of a conference:

• Whether the paper submission process will require reviewers.

• What the fee structure for paying Meetup will be.

• Who key personnel, such as the program chair and the event planner, will be

The conference management system will be hosted in the cloud; one of the reasons Meetup chose a cloud platform was its scalability and potential for elastic scalability.

The market that the Meetup Conference Management System oper­ates in is very competitive, and very fast moving. In order to compete, Meetup must be able to quickly and cost effectively adapt the con­ference management system to changes in the market. This require­ment for flexibility breaks down into a number of related aspects:

• Meetup must be able to evolve the system to meet new requirements and to respond to changes in the market.

• The system must be able to run multiple versions of its software simultaneously in order to support customers who are in the middle of a conference and who do not wish to upgrade to a new version immediately. Other customers may wish to migrate their existing conference data to a new version of the software as it becomes available.

• Meetup intends the software to last for at least five years. It must be able to accommodate significant changes over that period.

• Meetup does not want the complexity of some parts of the system to become a barrier to change.

• Meetup would like to be able to use different developers for different elements of the system, using cheaper developers for simpler tasks and restricting its use of more expensive and experienced developers to the more critical aspects of the system.


