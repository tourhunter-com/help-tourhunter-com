---
title: Agent company
layout: article
excerpt: Part of a post
category: agents
tags:
- company-creation
lang: en
permalink: "/en/:name/"
ref: agent-company
cat: some
---

### **Definition**

Agent is one of two types of companies available in the system. Agent is a company selling tours formed by the tour provider - Supplier.

Agent can create tour bookings of other Suppliers, add Suppliers to "My Suppliers".

Agent have three standard types of a subscriptions there are: Agent Online, Agent Offline, Agent Premium.

![Agent's subscription](/assets/images/agent_company1.png)

### **Roles**

Participants in an Agent company are divided into managers and employees, depending on their roles.

List of roles in a Agent company:
- Manager:

1. Manager;
2. Booking manager;
3. Accountant.

- Employees:

1. Seller.

![Agent's employees](/assets/images/agent_company2.png)

In addition to these roles, owner has the ability to create new roles, name them at their discretion and assign them to the manager or employees group.

A new user can be invited to employees, for this a future employee is not required to be a user, he will register at the time of accepting the invitation. To invite employees, fill out the data in the "Add User" module in "Manage > Employees > Add New Employee" and send an invitation.

![Agent's subscription](/assets/images/agent_company3.png)

In the profile in edit mode for each employee there is the option to enable the checkbox "Show in company profile". If a company user has enabled checkbox, employee is displayed in the profile of this company in the "Team" block. Only those employees who are already registered in the system or accepted the invitation are displayed.

![Agent's subscription](/assets/images/agent_company4.png)

### **Agent bookings**

Agent can makes bookings for tours in the sections:
- "Bookings > Manifest view" (only for Agent Premium or Supplier-Agent, those companies who have added foreign tours to the section "My Tours");
- "Marketplace" ("Marketplace > List view" or "Marketplace > Point-of-sale");
- "White Label" (on personal "White Label" or on Supplier's "White Label" when those Agent have been autorized).

Agent’s bookings made from "Marketplace > List view" immediately go to Supplier for confirmation; bookings made from "Marketplace > Point-of-sale" appear first in the "Checkout" module window and then go to the Supplier for confirmation.

Any type of Agent company can see his bookings which made by himself in "Bookings > Booking view", and also those bookings where Agent was indicated in "Booked By". The Agent can also change the booking data, but only if he is allowed to do this (a Supplier has enabled the "Can modify bookings" checkbox in the Agent’s profile in editing module).

If the Agent Premium makes a tour booking added to "My Tours", then he can see this booking in "Bookings > Manifest view" and "Bookings > Booking view".

Bookings of other tours that are not added to "My Tours" are only may be seen by the Agent Premium in "Bookings > Booking View" section, just like the regular Agent (Agent Online or Agent Offline).

If the Agent Premium makes a booking from "Booking > Manifest view", then this booking immediately go to a Supplier for confirmation, without falling into the "Checkout" module.