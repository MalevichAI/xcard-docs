---
title: Установка и запуск
slug: setup
---

# Установка и запуск

## Установка

### Клонирование репозитория

Первым шагом нужно склонировать репозиторий документации с GitHub. Сделать это можно следующей командой:

```
git clone https://github.com/MalevichAI/xcard-docs.git
```

:::warning Установка Git

Если у вас еще нет **Git**, вы можете установить его [здесь](https://git-scm.com/downloads).

:::

### Установка зависимостей

Помимо репозитория, необходимо так же установить **Node.js** и **NPM**:

* **Windows**:
    Скачайте и запустите установщик [Node.js](https://nodejs.org/dist/v22.14.0/node-v22.14.0-x64.msi)
* **Ubuntu**:
    ```shell
    sudo apt install nodejs
    sudo apt install npm
    ```
* **MacOS**:
    ```shell
    brew install node
    brew install npm
    ```

:::note Проверка установки

После установки стоит проверить корректность установки следующими командами:

```shell
node -v # вывод должен быть похож на "v22.xx.xx"
npm -v # вывод должен быть похож на "10.x.x"
```

:::

## Запуск

Перейдите в корневую папку репозитория `xcard-docs` и запустите из командной строки следующую команду:

```shell
npm start
```

Вывод должен выглядеть следующим образом:

```shell
> xcard-docs@0.0.0 start
> docusaurus start

[INFO] Starting the development server...
[SUCCESS] Docusaurus website is running at: http://localhost:3000/xcard-docs/

✔ Client
  Compiled successfully in 754.40ms

client (webpack 5.98.0) compiled successfully
```

Готово! По ссылке [`http://localhost:3000/xcard-docs/`](http://localhost:3000/xcard-docs/) будет располагаться документация, собранная с помощью Docusaurus. 

:::tip

Все изменения в файлах будут автоматически синхронизироваться на странице после сохранения файлов.

:::
