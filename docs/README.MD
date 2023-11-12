# Установка и настройка TypeScript

### Обновление Linux

```
sudo apt update
```
```
sudo apt upgrade -y
```
##### Установка CURL
```
sudo apt install curl -y
```

### Установка  и активация Node Version Manager (NVM)
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
```
```
source ~/.bashrc
```
##### Установка последней LTS версии Node.js
```
nvm install --lts
```
##### Выбираем версию Node.js, которая будет использоваться по умолчанию
```
nvm alias default <18.18.2>
```
##### Проверяем какая версия Node.js установлена
```
node -v npm -v
```

### Установка TypeScript

##### Устанавливаем
```
npm install -g typescript
```

##### Проверяем версию
```
tsc --v
```
##### Устанавливаем компилятор в виде модуля ts-node глобально
```
npm install -g ts-node
```

### Запуск файлов TypeScript
##### компиляция в app.js файл
```
tsc app.ts
```
##### и последующий запуск
```
node app.js
```
##### или сразу одной командой оба действия
```
ts-node app.ts
```

### Настраиваем проект TypeScript
[Рекомендации Влада Миленина](https://vladilen.notion.site/Node-js-TypeScript-2023-d08eba5fe4eb43fa8687ce7755a53bf0)

##### Инициализируем проект (появляется файл package.json)
```
npm init -y
```


##### Устанавливаем TypeScript локально. В папку проекта добавляется директория node_modules.
```
npm i -D typescript
```
##### Устанавливаем типизацию для node.js
```
npm i @types/node -D
```
Они добавляются в package.json как зависимости для разработки.





##### Инициализация. В папке проекта выполняем:
```
tsc --init
```
или
```
npx tsc --init
```
создается дефолтный tsconfig.json
