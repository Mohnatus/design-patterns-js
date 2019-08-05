[Главная](../../..) / [Структурные шаблоны](../..) / [Декоратор](..)

# Кофе с добавками (паттерн Декоратор)

## Команда для запуска кода

```
npm run decorator:coffee
```

## Описание

Компонент - это конкретная кофейная смесь, например, `Эспрессо` или `Кофе без кофеина`.
Декораторами могут выступать всевозможные добавки к кофе (`сливки`, `карамель`, `молоко`).

У исходной кофейной смеси есть собственная стоимость. Добавки увеличивают ее на определенную величину. Условно эспрессо стоит 30 рублей, добавка карамели - 5 рублей. На выходе получится 35 рублей.

Исходную смесь можно **оборачивать в любое количество декораторов** по необходимости (а можно вообще не оборачивать). Полученный продукт будет иметь ровно тот же самый интерфейс, так что у клиента не возникнет проблем при взаимодействии с ним.