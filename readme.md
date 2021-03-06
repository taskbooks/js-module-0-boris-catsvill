## Налаштування інфраструктури для розробки

### Система контролю версій (Git)

Git - це [розподілена система контролю версій](https://uk.wikipedia.org/wiki/Git). Git ми будемо використовувати у зв'язці з [Github](https://github.com/) щоби максимально    
наближити навчання до реальної розробки.  
Переконайтесь що Git втасновлений на вашому PC, якщо ні - використайте посилання нижче.

[Install Gіt](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

### NodeJs

[NodeJS](https://nodejs.org/) - це платформа яка дозволяє запускати код за межами браузера. 
Nodejs нам знадобиться для автоматизації збірки, запуску тестів та автоматизації деяких задач.

[Install Nodejs](https://nodejs.org/en/download/)

### Редактори коду

З редакторів коду ми рекомендуємо WebStorm, але підійде будь який інший редактор,
наприклад, VSCode.

[Install Webstorm](https://www.jetbrains.com/webstorm/)  
or  
[Install VSCode](https://code.visualstudio.com/)

## Налаштування задачника

### Перший крок - втановлення залежностей

В першу чергу потрібно встановити npm пакети які використовуються в данному проекті.  
Це можно зробити наступною командою, зупустивши її в корні проекта:

```bash 
npm install
```

### Запуск тестів

В кожному модулі знаходиться декілько задач разом з тестами, ціль яких перевірити  
коректність виконаного завдання. Тести можно запускати як всі разом, так і окремо для  
кожної задачі або модуля.

#### Як запустити всі тести:
  
В корні проекта виконати команду:  

  ```bash 
  npm test
  ```  
 
#### Як запустити тести з певної директорії:

В корні проекта виконати команду:  

  ```bash
  npm test -- --findRelatedTests <path>
  ``` 

  * `<path>` це шлях до директорії

#### Як запустити один тест:

  ```bash 
  npm test -- -t "<describeString> <itString>"
  ```

  * `describeString` - це ім'я "describe" блоку, 
  * `itString` -це ім'я "it" блоку

Більше деталей по запуску тестів можно отримати за посиланням: [Jest](https://jestjs.io/docs/en/cli.html#--testnamepatternregex)
