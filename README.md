# bitrix-lang
Makes work with Bitrix lang messages better

---

## Недостатки системы языковых сообщений bitrix
1. Огромное множество языковых файлов: отдельные файлы для компонентов, шаблонов компонентов, шаблонов сайта, модулей.
2. Неудобный формат языкового файла: `$MESS['msg_code'] = 'Some message'`.
3. Отсутствие поддержки множественных форм: 1 комментарий, 2 комментария, 5 комментариев.

Такой подход к языковым сообщениям неудобен и требует участия программиста при составлении переводов сайта.

## Общее решение
Собрать все сообщения для одного языка в едином файле, например: `/local/lang/ru.php`.

Упростить формат языкового файла. Пример:

```
    company.name Креативное агентство «Агентство креатива»
    company.slogan Полет фантазии, фантазии полет
```
    
Добавить поддержку множественных форм. Пример языкового файла:
    
```    
    comments.num %number% комментарий | %number% комментария | %number% комментариев
    comments комментарий | комментария | комментариев
```

Также должна быть предусмотрена совместимость со стандартной bitrix-функцией GetMessage().

## Использование
### Установка
С помощью Composer.

### Публичные методы
Coming soon.

### Подробное описание формата языковых файлов
Coming soon.

