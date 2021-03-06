[Поведенческие шаблоны](../#readme) / Интерпретатор

# Интерпретатор (Interpreter)

## ![](../../ui/info.svg) Описание паттерна

Прежде всего связан с разбором некоторого языка/грамматических правил (например, языка программирования).

Определяет представление грамматики для заданного языка и интерпретирует его предложения.

Каждое **грамматическое правило** редставлено в виде отдельного класса и может быть составным (то есть ссылаться на другие правила) или терминальным (окончательным).

## ![](../../ui/code.svg) Примеры

* Музыкант интерпретирует музыкальный язык - ноты, описывающие тональность и продолжительность звуков.
* [Римские числа](./roman#readme)
* [Математические операции](./math#readme)

## ![](../../ui/interaction.svg) Взаимодействие с другими паттернами

* [Компоновщик (Composite)](../../structural/composite#readme) помогает составить синтаксическое дерево интерпретатора
* [Итератор (Iterator)](../iterator#readme) может использоваться для обхода узлов дерева
* [Приспособленец (Flyweight)](../../structural/flyweight#readme)
