---
title: Transfers messages
layout: article
excerpt: Part of a post
category: notifications
subcategories:
    notifications: messages
tags:
- resource-settings
lang: en
permalink: "/en/:name/"
ref: transfers-messages
cat: some
---

### **Displaying messages about removing transfers**

If the booking has been moved to the transfer resource (at "Bookings > Transfer view > Pick-up" section) and the transfer type "pick-up only" is set in the booking module, and the transfer value in the booking module changes to "drop-off only", then the booking is deleted from the old transfer resource.

And in the "Top menu > Messages" the owner and employees of the Supplier company are shown an additional notification that the booking has been removed from the transfer resource.

![Transfer_messages1](/assets/images/transfer_messages1.png)

If the booking has been moved to the transfer resource (in "Bookings > Transfer view > Drop-off" section) and the transfer type "drop-off only" is set in the booking module, and the transfer value in the booking module changes to "pick-up only", then the booking is deleted from the old transfer resource.

And in the "Top menu > Messages" the owner and employees of the Supplier company are shown an additional notification that the booking has been removed from the transfer resource.

![Transfer_messages2](/assets/images/transfer_messages2.png)

### **Suggestions**

The notification is shown only in the case when the deletion occurred due to changes in the settings of the "Pick-up" block in the booking module: the type of transfer has changed or the location has been completely deleted.

If you directly delete from the transfer resource (in the transfer resource card, the menu item ellipsis "Remove"), a notification will not be displayed.

If there is a booking both in "Transfer view > Pick-up" section and in "Transfer view > Drop-off" section ("round trip" is indicated in the booking module), then when deleting the location at all or selecting "no transfer" in the booking module, two notifications at once.

When you click on a notification, a booking modal opens, as well as for other messages from the "Top menu > Messages" on bookings.