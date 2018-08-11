---
layout: default
title: Метод Newsfeed.AddBan
permalink: newsfeed/addBan/
comments: true
---
# Метод Newsfeed.AddBan
Запрещает показывать новости от заданных пользователей и групп в ленте новостей текущего пользователя.

Страница документации ВКонтакте [newsfeed.addBan](https://vk.com/dev/newsfeed.addBan).

## Синтаксис
``` csharp
public bool AddBan(IEnumerable<long> userIds, IEnumerable<long> groupIds)
```

## Параметры
+ **userIds** - Перечисленные через запятую идентификаторы друзей пользователя, новости от которых необходимо скрыть из ленты новостей текущего пользователя. список целых чисел, разделенных запятыми
+ **groupIds** - Перечисленные через запятую идентификаторы групп пользователя, новости от которых необходимо скрыть из ленты новостей текущего пользователя. список целых чисел, разделенных запятыми

## Результат
После успешного выполнения возвращает **true**.

## Пример
``` csharp
var addBan = _api.Newsfeed.AddBan();
```

## Версия Вконтакте API v.5.44
Дата обновления: 28.01.2016 13:09:42