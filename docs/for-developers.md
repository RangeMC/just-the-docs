---
layout: default
title: Для разработчиков
nav_order: 6
---

# Для разработчиков

В данном разделе описана документация по API нашего сайта.

---

## Получить данные об игроке
{: .d-inline-block }

GET
{: .label .label-green }

Данный метод позволяет получать данные об игроке по никнейму.

URL для запроса: `https://rangemc.ovh/api/user/:login`

- Параметр `login` необходимо заменить на логин зарегистрированного игрока.

#### Запрос
{: .no_toc }

```yaml
https://rangemc.ovh/api/user/AlexxxlYT
```

#### Ответ
{: .no_toc }

```json
{
  "id": 7,
  "username": "AlexxxlYT",
  "rank": "admin",
  "coins": 150,
  "uuid": "2adaebb2-12e0-11eb-88e2-5255000bf042",
  "skin": "https://rangemc.ovh/skin/AlexxxlYT.png",
  "cloak": "https://rangemc.ovh/cloak/AlexxxlYT.png"
}
```

#### Таблица прав

| Ранг в API | Название | Префикс | Цвет | Цвет в HEX |
|:-----------|:---------|:--------|:-----|:-----------|
| default | Игрок | PLAYER | §7§l | <span style="background-color: #AAAAAA" class="d-inline-block p-2 mr-1 v-align-middle"></span> #AAAAAA |
| premium | Премиум | PREMIUM | §6§l | <span style="background-color: #FFAA00" class="d-inline-block p-2 mr-1 v-align-middle"></span> #FFAA00 |
| legend | Легенда | LEGEND | §b§l | <span style="background-color: #55FFFF" class="d-inline-block p-2 mr-1 v-align-middle"></span> #55FFFF |
| ultra | Ультра | ULTRA | §d§l | <span style="background-color: #FF55FF" class="d-inline-block p-2 mr-1 v-align-middle"></span> #FF55FF |
| sponsor | Спонсор | SPONSOR | §e§l | <span style="background-color: #FFFF55" class="d-inline-block p-2 mr-1 v-align-middle"></span> #FFFF55 |
| youtube | Ютубер | YOUTUBE | §c§l | <span style="background-color: #FF5555" class="d-inline-block p-2 mr-1 v-align-middle"></span> #FF5555 |
| builder | Билдер | BUILDER | §a§l | <span style="background-color: #55FF55" class="d-inline-block p-2 mr-1 v-align-middle"></span> #55FF55 |
| helper | Хелпер | HELPER | §a§l | <span style="background-color: #55FF55" class="d-inline-block p-2 mr-1 v-align-middle"></span> #55FF55 |
| moder | Модер | MODER | §9§l | <span style="background-color: #5555FF" class="d-inline-block p-2 mr-1 v-align-middle"></span> #5555FF |
| stmoder | Ст. Модер | STMODER | §9§l | <span style="background-color: #FF55FF" class="d-inline-block p-2 mr-1 v-align-middle"></span> #FF55FF |
| devel | Разраб | DEVEL | §6§l | <span style="background-color: #FFAA00" class="d-inline-block p-2 mr-1 v-align-middle"></span> #FFAA00 |
| admin | Админ | ADMIN | §c§l | <span style="background-color: #FF5555" class="d-inline-block p-2 mr-1 v-align-middle"></span> #FF5555 |

## Получить скин игрока
{: .d-inline-block }

GET
{: .label .label-green }

Данный метод позволяет получать скин игрока по никнейму.

URL для запроса: `https://skins.rangemc.ovh/body/:login.png`

- Параметр `login` необходимо заменить на логин зарегистрированного игрока.
- Если не указывать никнейм игрока или указать его неверно, сервер вернёт стандартный скин.

#### Запрос
{: .no_toc }

```yaml
https://skins.rangemc.ovh/body/AlexxxlYT.png
```

#### Ответ
{: .no_toc }

<code style="display: block;"><img src="https://i.imgur.com/mKLakfS.png"></code>

## Получить плащ игрока
{: .d-inline-block }

GET
{: .label .label-green }

Данный метод позволяет получать плащ игрока по никнейму.

URL для запроса: `https://skins.rangemc.ovh/cape/:login.png`

- Параметр `login` необходимо заменить на логин зарегистрированного игрока.
- Если не указывать никнейм игрока или указать его неверно, сервер вернёт стандартный плащ.

#### Запрос
{: .no_toc }

```yaml
https://skins.rangemc.ovh/cape/AlexxxlYT.png
```

#### Ответ
{: .no_toc }

<code style="display: block;"><img src="https://i.imgur.com/KvedTQx.png"></code>