---
title: Создание сезонных правил ценообразования
layout: article
excerpt: Part of a post
category: net-rates
lang: ru
permalink: "/ru/:name/"
ref: creating-a-new-pricing-seasonal-rules
cat: some
---

## **Шаг 1**

Перейти в “Manage > My rates”.

## **Шаг 2**

Выбрать тип тарифов в выпадающем меню:
- “Standard rates”;
- “Special rates”;
- “Create new…”.

![Creating_a_new_pricing_seasonal_rules1](/assets/images/creating_a_new_pricing_seasonal_rules1.png)

## **Шаг 3**

Кликнуть на кнопку “+ New Seasonal Rules”.

![Creating_a_new_pricing_seasonal_rules2](/assets/images/creating_a_new_pricing_seasonal_rules2.png)

## **Шаг 4**

Выбрать “Date” - период, в который будут действовать правила ценообразования.

![Creating_a_new_pricing_seasonal_rules3](/assets/images/creating_a_new_seasonal_rules3.png)

## **Шаг 5**

Настроить следующие функции:
- “Prices & Rates” - в данном разделе отображаются туры с тур. опциями. Ниже расположены 3 колонки:
- “Participants” - название категории участников (с возрастом);
- “Selling price” - стоимость тура для данной категории участников, для компаний типа Agent, кто создал этот прайс-лист;
- “Net Rate/Commission” - выпадающее меню с выбором “$” или “%”;
- “Special Rates”;
- “Extras” - функции аналогичны разделу “Prices & Rates”. Поле “Net Rates” не может быть пустым;
- “Fees” - сборы для данного прайс-листа;
- “Taxes” - налоги для данного прайс-листа;
- “Pick-ups” - если настроены цены для трансферов "Round trip"/"Pick-up only"/"Drop-off only"/"No Transfer", тогда в данном разделе можно отключить экстра;
- “Payment Rules” - в данном разделе можно изменить способ оплаты тура:
    - “customer will pay to Agent” - 2 значения: 
        - “Send invoice to Agent” - необходимо выбрать “before the tours start/after the tour started/after the booking was created/on fixed weekdays/on fixed days of months”;
        - “Request payment from Agent” - необходимо выбрать день “after invoice was sent”;
    - “customer will pay to Supplier”- 2 значения:
        - “Send invoice to Agent” - необходимо выбрать “before the tours start/after the tour started/after the booking was created/on fixed weekdays/on fixed days of months”;          - “Pay the commission to Agent” - необходимо выбрать день “after invoice was sent”;
    - “do not track payment” - следующие изменения для турагентов:
        - нет разрешения отслеживать клиентские платежи;
        - не показываются цены за трансфер;
        - в ваучере не отображается строка “Total Paid”;
        - в модалке “Checkout” не показываются данные, связанные с ценой;
        - при авторизации на "White Label" туроператора скрываются все цены.
- “Cancellation” - формирование задолженности для турагента; 
- “Terms & Conditions” - в режиме просмотра отображается текст, в режиме редактирования - текстовое поле, которое изменяется, как в настройке тура в “Additional Description”.

![Creating_a_new_pricing_seasonal_rules4](/assets/images/creating_a_new_pricing_seasonal_rules4.png)

## **Шаг 6**

Кликнуть на кнопку “Save”.
