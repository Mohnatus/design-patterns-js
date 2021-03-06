[Поведенческие шаблоны](../#readme) / Хранитель

# Хранитель (Memento)

## ![](../../ui/info.svg) Описание паттерна

**Фиксирует внутреннее состояние объекта** для его последующего *восстановления*. При этом *не нарушается инкапсуляция* объекта.

## ![](../../ui/gear.svg) Реализация паттерна

![Схема паттерна Хранитель](./scheme/scheme.png)

`Создатель` (Originator) - объект с некоторым внутренним состоянием.

`Опекун` (Caretaker) может совершать какие-то действия, но при этом должна быть возможность откатить состояние `Создателя` до исходного.

Состояние сохраняется в объекте `Хранителя` (Memento), который не может быть изменен `Опекуном`.

Возможно более жесткое ограничение доступа `Опекуна` к `Создателю`.

## ![](../../ui/code.svg) Примеры

* [Сохранение состояния](./base#readme)
