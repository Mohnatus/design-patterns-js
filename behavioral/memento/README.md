# Хранитель

## Команда для запуска кода

```
npm run memento
```

## Что делает?

**Фиксирует внутреннее состояние объекта** для его последующего *восстановления*. При этом *не нарушается инкапсуляция* объекта.

## Реализация

`Создатель` (Originator) - объект с некоторым внутренним состоянием. 

`Опекун` (Caretaker) может совершать какие-то действия, но при этом должна быть возможность откатить состояние `Создателя` до исходного. 

Состояние сохраняется в объекте `Хранителя` (Memento), который не может быть изменен `Опекуном`.

Возможно более жесткое ограничение доступа `Опекуна` к `Создателю`. 