# .NET Zuid public website

We currently have a website at http://www.dotnetzuid.nl/, which we want a new version of.

This repository will become the new version of the website. 
Yes, it is empty at the moment, which means you have a lot of freedom to create!

We would like a simple website that at least does the following:
* Allow usergroup attendees to authenticate to identify themselves
* Allow usergroup attendees to register for events
* Allow usergroup attendees to cancel their registration for an event
* Allow usergroup organizers to authenticate to identify themselves
* Allow usergroup organizers to create, edit and delete events

These requirements will be fleshed out more as issues for this repository.

We encourage everyone to contribute.
All contributions, large and small, are welcome!

PS: If you contribute, you could win a one-year JetBrains license!

### Groundrules

You have full freedom to create a new website, but we do have some technical requirements:

* The website will run in Azure
* The website is going to run at the URL dotnetzuid.nl
* We will use CloudFlare as a proxy in front of the website, which will provide us security and performance benefits
  * By using CloudFlare, we also get an SSL certificate, which will force all communications over HTTPS
* We want to leverage Azure services, so if you use a database, it will be one that lives in Azure
* All infrastructure should be coded and documented
  * It should be very easy to deploy the complete setup somewhere, so that conttributers can get started easily
* The solution should be easy to update by means of Continuous Delivery
* User credentials will not be stored in a database. They should live in a service that is built for that, like Azure Active Directory
* Use Micosot oriented technologies that are easy to understand for other contributors
* Keep it simple! 
