---
title: Уведомления по подписке
layout: article
excerpt: Part of a post
category: notifications
subcategories:
    notifications: pending-requests
tags:
- billing
lang: ru
permalink: "/ru/:name/"
ref: subscription-notifications
cat: some
---

### **Уведомления об истечении срока подписки, ожидающие действий**

За 10 дней до истечения срока подписки для владельца и сотрудников компаний отображается уведомление в "Top menu > Pending Requests".

Для владельца компании такое уведомление отображается с кнопкой "Update", по клику на которую пользователь перенаправляется в раздел "Billing & Payments", и кнопкой "Take credit period" для возможности взять кредитный период на 10 дней.

![Subscription_notifications1](/assets/images/subscription_notifications1.png)

![Subscription_notifications2](/assets/images/subscription_notifications2.png)

Для менеджера и других сотрудников отображается только уведомление без кнопок, поскольку сотрудники не могут оплатить подписку.

![Subscription_notifications3](/assets/images/subscription_notifications3.png)

### **Отображение уведомлений при завершенной подписке**

Если компания заблокирована из-за не оплаченной подписки, то новые букинги внутри системы и уведомления приходят в "Pending Requests".

Если у компании закончился 10-ти дневный срок для оплаты и компания становится заблокирована, сообщения в "Top menu > Messages" не приходят. После того, как подписку оплатят, сообщения в "Messages" снова отобразятся.

### **Сообщения о подтверждении оплаты по подписке**

После того, как админ подтвердит или отклонит банковский перевод, у пользователя в "Top menu > Messages" отобразится соответствующее сообщение.

Если его платеж подтвержден, отображается "Your subscription payment was confirmed".

![Subscription_notifications4](/assets/images/subscription_notifications4.png)

Если его платеж отклонен, отображается "Your subscription payment was declined".

![Subscription_notifications5](/assets/images/subscription_notifications5.png)

При клике на сообщение, пользователя перенаправляет на соответствующую страницу "Pay via bank transfer".
