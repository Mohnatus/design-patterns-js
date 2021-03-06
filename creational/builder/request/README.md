[Порождающие шаблоны](../../#readme) / [Строитель](../#readme) > Сборка объекта запроса

# Сборка объекта запроса (паттерн Строитель)

## ![](../../../ui/info.svg) Описание

Объект запроса (`Request`) имеет несколько параметров:

* адрес
* метод
* полезная нагрузка (передаваемые данные)

Для удобной сборки запросов используется `Строитель` `RequestBuilder`. Каждый параметр настраивается с помощью отдельного метода.

Из каждого метода возвращается `this`, что позволяет объединить вызовы в одну цепочку.

***
***

**Сборка объекта запроса**: [index.js](./index.js)

**Команда для запуска кода**

```
npm run builder:request
```
