# Diagraming Roles & Relationships

## Swimlane Diagrams 

The main value of swimlane diagrams (aka "cross-functional diagram") is "role" separation in a way that clearly sequences and allocates important functions and events to "people" (ie a human or organization).  For this purpose a "person" is any "legal" entity.  As a shortcut, you can ask whether an entity can sue and be sued in order to get a pretty good sense of whether it is a legal person or not.  A software system is not a legal person but a software system vendor or software system implementer or software system user, etc probably is a legal person.  "HTML" and "Javascript" and "Ethereum Node" and "Wallet" and "Database" are important items to diagram in order to illustrate some aspects of a system but not for a swimlane diagram intended for the purposes of identifying business/legal entity "cross-functional" roles.  

So - we'd expect something including roles like: 
* User (client or credit union member etc); 
* Third party (or merchant or seller, etc); 
* App provider (lawyer or credit union etc)

## Example Roles of Legal/Business Entities

The following exampes illustrate how to map functions, actions and other events to business and/or legal roles of "entities" for this type of diagram: 

### Context: Expense Report
* Roles: Consultant; Accountant; Payroll, etc from [http://www.agilemodeling.com/style/activityDiagram.htm](http://www.agilemodeling.com/style/activityDiagram.htm):

<img src="https://github.com/mitmedialab/CoreID/blob/master/diagrams/expenses.png">

### Context: Sales Flow

* Roles: Customer; Sales; Legal; etc from [http://www.modernanalyst.com/Careers/InterviewQuestions/tabid/128/ID/1804/What-is-a-Swimlane-Diagram.aspx](http://www.modernanalyst.com/Careers/InterviewQuestions/tabid/128/ID/1804/What-is-a-Swimlane-Diagram.aspx)

<img src="https://github.com/mitmedialab/CoreID/blob/master/diagrams/sales.png">

### Context: Student Registration

*  Roles: Faculty Advisor, Student; Admin; etc, from [https://www.yworks.com/actions/imageviewer.php?img=studentRegistrationColors2.e03efb32.png&album=yfiles&maxWidth=800&maxHeight=760](https://www.yworks.com/actions/imageviewer.php?img=studentRegistrationColors2.e03efb32.png&album=yfiles&maxWidth=800&maxHeight=760): 

<img src="https://github.com/mitmedialab/CoreID/blob/master/diagrams/registration.png">

## Use Same Approach for Legal Roles 

A given person (Alice, Bob, ACME Co, etc) will have a primary role in any given "business" context (business is just used to connote the "thing people are trying to do" and is sometimes also known as "operations" or "workflow" etc).  For instance, the roles "customer" or "prospect" or "trusted partner" may be examples of how business people think and talk about the role of a party in the context of a given transaction or system.  This is the role to use in a swimlane diagram depicting that transaction or system.  That same person will also exist in a "legal" context, such as "consumer" or "licensee" or "subsidiary" etc.  This frequently can be addressed as an aspect of the "business" role or can be treated as a unique "legal" role that may be very connected and somewhat overlapping with the "business" role of any given party.  Frequently the primary legal role of any given party is pretty clear and readily identifiable in commercial, governmental, education, healthcare, transportation and other common transaction or system contexts (eg "doctor" or "patient" or "student" etc). In certain situations, a given party may play more than one business role at a time or over a period of time, making the legal role or roles of any given party may be more difficult to pin down.   Sometimes the the key legal role or roles of any given party may be subtle and require an attorney or other legal professional with expertice in the relevant context in order to identify the most important role or roles. 

Which legal role or roles apply to a given person can determine the legal outcomes that will result from the use of technology. Combinations of circumstances outside of the technology can determine if or when a given party has changed legal roles (eg from "contractor" to "employee") even if all technical roles (eg "user") and business roles (eg "driver") have remained the same.  The legal roles and relationships and rules that apply in a given context can determine whether an action or event occuring through the use of technology will be considered "enforceable" or "unenforceable" or "admissible" or "inadmissible" or in "compliance" or "non-compliance" and so on.  

### Agency-Law Style "Triangle" of Roles

Agency law identifies the roles and relationships of a "principal" and "agent" and "third party".  Accurately identifying which of these three legal roles applies to any given party can enable correct prediction of the primary "rules" defining relevant rights and responsibilities of each party vis-a-vis each other party. This is another way of saying that accurate identification of the most important legal role of a given entity in the context of some technology (eg for a transaction or system) can reveal much more predictable legal outcomes resulting from the use or reliance upon that technology.  

Many digital signature, authorization and other identity related technologies exist within business and legal contexts that involve a "triangle" of agency law roles either directly, or partially.  The following excerpt is an example of how Massachusetts Legal Hackers has specifically attempted to apply business/legal role based designations to a scenario involving the use of StonePaper to execute a digital signature on a contract.

>  **[2017 April 25 LegalHackNight Project Notes](https://github.com/MassachusettsLegalHackers/BCID/wiki/2017-April-25-LegalHackNight-ProjectNotes)**

> The third hack night of our individual identity prototype series is shaping up to be a big milestone for the project:  We're hoping to have working versions of both the Bitcoin and Ethereum public blockchain implementations sufficiently customized to reflect a commercial "sale of goods" business and technology use case adopted by the group at our first hack of this 5-part series.  This will provide a sound foundation to walk through activities and interactions of each key party and start evaluating the best candidate approaches to establish legal rules, roles, relationships, rights, responsibilities covering the three key players:

> 1. The Individual Principal in their role as a party legally signing contracts and making other authorizations with their own blockchain-based identity by using the App to conduct transactions on the web;

> 2. The Fiduciary Agent in their role as a party who acts on behalf, at the behest and in the best interests of the Individual Principal as their Member or Client, respectively and and who provides or is responsible for platform or other business services in connection with the individual app; and

> 3. The Transacting Third Party user, in their role as a party who legally countersigns contracts and is a relying party on authorizations as a counterparty to transactions conducted by or for the Individual Principal.

> In the use case, the Fiduciary Agent will presumably be a US federally chartered, regulated and insured credit union providing services to and acting on behalf of an Individual Principal who is a Member of the Credit Union.  The Ethereum Stone Paper initial code base assumes the fiduciary is a hybrid between a Notary and a Licensed Attorney providing services to and acting on behalf of the Individual Principal who is a Client of their law practice.  For technical purposes, we aim to customize the technology to allow for a range of Fiduciary Agent and Individual Principal pair-wise relationships, while continuing to support, reflect and assume the full customary set of fiduciary duties exist as a legal foundation of the integrated business, legal and technical dimensions of our working prototype.  

## Common Web Context: OAuth 2 

For many reasons it is useful and instructive to understand the roles and sequences underlying OAuth 2.  When OAuth 2 (including OpenID Connect, UMA or any other protocol that uses OAuth 2) is part of an identity, authentication, authorization, signature or other use case, it is especially important to be able to identify, link, track and map the relationships between the OAuth 2 related and the Blockchain related roles of each legal or business entity involved in transactions or playing other relevant system roles. Here are some quick snapshorts of the key activity sequences with OAuth 2:  

**Mapping Blockchain-Enabled Identity to Roles and Flows the Common Broader Context of the Open Web**

* [https://tools.ietf.org/html/rfc6749](https://tools.ietf.org/html/rfc6749)

### High Level Protocol Flow

<img width="615" alt="fig1-highlevelprototcolflow" src="https://raw.githubusercontent.com/mitmedialab/CoreID/master/diagrams/Fig1-HighLevelPrototcolFlow.png">

### Token Refresh Flow

<img width="615" alt="Fig2-TokenRefresh" src="https://raw.githubusercontent.com/mitmedialab/CoreID/master/diagrams/Fig2-TokenRefresh.png">

### Authorization Explicit Grant Flow 

<img width="615" alt="Fig3-AuthFlow" src="https://raw.githubusercontent.com/mitmedialab/CoreID/master/diagrams/Fig3-AuthFlow.png">

### Implicit Authorization Flow 

<img width="615" alt="Fig4-ImplicitFlow.png" src="https://raw.githubusercontent.com/mitmedialab/CoreID/master/diagrams/Fig4-ImplicitFlow.png">

-------------

Now consider the following ["User Managed Access" diagram](https://www.websequencediagrams.com/files/render?link=gnYlOf_cwh605AwcO-9i): 

<img width="615" alt="fig1-highlevelprototcolflow" src="https://github.com/mitmedialab/CoreID/blob/master/diagrams/UMA-EarlySwimlane.png">

Note that in this particular version, the person making the diagram chose not to be clear about which legal party was going to be responsible for the "authorization server" and for the "resource server".  In other versions, we made swimlane diagrams for each key business/legal scenario that involved a different legal/business "role" responsible for providing the auth and/or resource services.  This simply required taking the auth and resource server functions and actions identified in the diagram above and allocating them to the identified legal/business "roles" for each key identified scenario.  

For context, in OAuth 2 and OIDC deployment scenarios, the same party may operates both the auth and resource servers and provides corresponding services to the resource owner, (such as with Google providing Google Docs and also the authorization services allowing Google users to grant third parties access of various types to see/change/etc Google Docs. Sometimes however these are services may be provided by different legal entities including one business unit of a "resource owner" company providing the service(s) to other business units of the same company.  

The legal and business entity responsible for providing the "client" (app) was not identified in the diagram version above.  The first column is for the "resource owner" who is the "user" of the "client" app but is almost certainly not the legal party responsible for providing and maintaining the client app (or apps) operated by the user as part of the UMA/OAuth 2/OIDC flow shown by the SwimLane diagram.  For more info on the fundamentals of these roles, take another look at the OAuth 2 role-designations I shared with you before, available here: https://github.com/mitmedialab/CoreID/blob/master/diagrams/README.md (see the "Token Refresh Flow" and "Authorization Explicit Grant Flow" diagrams on this page for good examples of how we track OAuth 2 "roles" to "functions" and "actions" as part of a simplified cross-functional role/activity sequence diagram.)


