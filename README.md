# Attribute Change Service #
Attribute Change Service is an open-source project for managing changes to identity data 
across interconnected information systems. 

The project aims to provide a way to record what changed, determine what verification is required, 
maintain version history, and track the distribution of approved changes to identity attributes 
across systems. it is being developed with interoperable public-sector infrastructure and 
digital public infrastructure ecosystems in mind. 

The project is currently at an early stage of development and is focused on defining the core 
domain model and architecture. 

# Progress

## Phase 1
[X] Project scaffolding
[X] User and Role
[X] Person model
[ ] AttributeDefinition: An attribute in the deployment with its trust tier
[ ] AttributeChange: One requested change to one attribute of one person
[ ] RelyingSystem: A system that needs to hear about changes, with delivery channel and contact
[ ] PersonIdentifier: A person's identifier in one relying system
[ ] ChangePropagation: one change for one relying system with status, timestamps, and who confirmed it
[ ] PersonAttribute: a versioned current value of an attribute for a person

## Phase 2
Notification, backend workers, escalation, reminders

# ENUMS
TrustTier: SELF_ASSERTED, AUTHORISATION_REQUIRED, HIGH_RISK
ChangeStatus: PENDING, VERIFIED, APPROVED, REJECTED
PropagationStatus: PENDING, NOTIFIED, APPLIED, REJECTED, FAILED
AcknowledgementMethod: MANUAL, AUTOMATIC
DeliveryChannel: WEBHOOK, EMAIL, PULL

## Background ##
I'm Dr. Katherine Wyers, a software engineer and researcher specialising in identity data, 
interoperability, and digital public infrastructure. 

Attribute Change Service addresses a common challenge in identity and service-delivery systems, 
managing changes to identity data in a way that preserves the history of the update, supports 
appropriate verification, and enables the reliable exchange of information between the various 
systems. 

The project is currently in the early stages of development. 
[Visit my website] [https://katherinewyers.com]
