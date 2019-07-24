# Приспособленец

Он же `Кэш`, он же `Легковесный элемент`

## Команда для запуска кода

```
npm run flyweight
```

## Что делает и зачем нужен?

Экономит оперативную память, **вычленяя общее состояние различных объектов и разделяя его между ними**. Объекты при этом могут быть совершенно разными.

Шаблон часто используется при работе с большим количеством мелких объектов (частиц).

## Реализация

В классе хранятся *только неизменяемые данные и методы* (**внутреннее состояние**), в которые передаются *изменяющиеся данные* (**внешнее состояние**), вынесенные за пределы `Приспособленца`.

Это позволяет *повторно использовать* одни и те же объекты, не создавая новые.

Важно обеспечить **неизменяемость внутреннего состояния** `Приспособленца` (отсутствие сеттеров и публичных полей).

## Пример из жизни

Разнообразные частицы в игре: пули, снаряды, осколки от взрывов и т. д.

У каждой частицы собственные координаты, скорость и вектор движения - это внешнее изменяемое состояние. 

Но есть и неизменяемые данные, например, спрайт картинок. Он общий для всех частиц и нет смысла дублировать его в разных классах (учитывая его, скорее всего, приличный вес). Подобные неизменяемые данные, общие для разных объектов называются внутренним состоянием.

## Взаимодействие с другими шаблонами

* [Фабричный метод](../../creational/factoryMethod)

Когда необходимо получить новый объект, Фабричный метод ищет подходящий среди уже созданных (с подходящим внутренним состоянием) и использует его. 