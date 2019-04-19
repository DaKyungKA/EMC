# Поточний модуль

Модуль відносно якого виконуються операції. За замовчуванням цей модуль завантажується із файла <code>.will.yml</code> поточної директорії.

Іншими словами, це `will-файл`, по відношенню до якого виконуються команди в командній оболонці системи.
Наприклад, директорія має наступну структуру файлів:  

```
 .
 ├── proto
 │     ├── files
 │     │     ├── one.will.yml
 │    ...    ├── two.will.yml
 │          ...
 ├── .will.yml  
 ├── all.will.yml
 ├── release.will.yml
 └── super.will.yml

 ```

 При виконанні команд без фраз `.with` i `.each` поточним модулем буде файл `.will.yml`. Для того, щоб поточним модулем був іменований `will-файл` потрібно виконати команду `.with` з указанням імені файлу, наприклад, при виконанні `will .with release .build` поточним буде модуль з файлом `release.will.yml`. При виконанні команди `.each` в директорії кожен із модулів буде поточним (наприклад, `will .each . .build`), а при виконанні команди `.each` відносно підмодулів - `will-файл` з указаними підмодулями.  
 Якщо `will-файл` запускає побудову в іншому `will-файлі`, то він залишається поточним.