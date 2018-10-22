## Логические блоки
1. "Хлебные крошки" `buildBreadcrumbs`
  * показывают HISTORY на списке коммитов
  * показывают урл на HISTORY при вызове с хэшем (переход в коммит)
  * показывают урлы на родительские директории при вызове с хэшем и путём (переход в файлы/папки)
2. "Взаимодействие с git" `executeGit`
  * возвращает результат выполнения git команды в виде строки
3. "История коммитов" `gitHistory`
  * возвращает массив объектов, хранящих информацию о коммитах
4. "Содержимое дерева" `gitFileTree`
  * возвращает массив js-объектов, хранящих информацию об объектах в заданном git-дереве

# Домашнее задание: автотесты

Вам дано приложение на JavaScript и нужно написать для него автотесты: интеграционные тесты на интерфейс и модульные тесты на серверную часть.

## Предметная область

Приложение отображает в браузере информацию из git репозитория: список коммитов, файловую систему для выбранного коммита, содержимое выбранного файла (поддерживаются только текстовые форматы). Для удобства навигации на каджой странице отображаются "хлебные крошки".

## Как запустить

```sh
git clone git@github.com:dima117/shri-testing-homework.git
cd shri-testing-homework.git
npm i
npm start
```

## Интеграционные тесты

Сценарии для интеграционных тестов

- на всех страницах (история коммитов, просмотр файловой системы, просмотр содержимого файла) правильно отображается правильное их содержимое;
- правильно работают переходы по страницам
  - из списка коммитов на список файлов
  - из списка файлов во вложенную папку
  - из списка файлов на страницу отдельного файла
  - переходы по хлебным крошкам

## Модульные тесты

- нужно добавить в README список логических блоков системы и их сценариев
- для каждого блока нужно написать модульные тесты
- если необходимо, выполните рефакторинг, чтобы реорганизовать логические блоки или добавить точки расширения
