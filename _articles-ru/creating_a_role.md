---
title: Создание роли
layout: article
excerpt: Part of a post
category: getting-started
subcategories:
    getting-started: employees
lang: ru
permalink: "/ru/:name/"
ref: creating-a-role
cat: some
---

### **Шаг 1**

Перейти в "Manage > Employees > Roles & Permissions".

### **Шаг 2**

Кликнуть на кнопку "Add Role".

![Creating_a_role1](/assets/images/creating_a_role1.png)

### **Шаг 3**

Заполнить требуемое поле:

"Job name" - название роли.

### **Шаг 4 (не обязательный)**

Заполнить поля:
- "Description" - описание роли;
- "General Settings".  

![Creating_a_role2](/assets/images/creating_a_role2.png)

### **Шаг 5 (не обязательный)**

Настроить "General Settings".

Более подробно о том как настроить ограничения для роли в "General Settings" в статье [*"Как настроить ограничения для роли?"*]({% link _articles-ru/how_to_setup_permissions_for_a_role.md %}).

Запрещено создавать системные роли, такие как "Manager" и "Owner". Если попытаться создать роль, которая уже существует, отобразится ошибка: "Role name [name] has already been taken.". Если попытаться создать роль с системным названием, отобразится ошибка: "This is a system role name.".
