# Неформальний підмодуль  

Група файлів, що не розповсюджується із <code>will-файлом</code>. Для такого підмодуля можливо створити <code>will-файлом</code> самостійно.  

Під імпортом непрямим шляхом розуміється те, що підмодуль створено без використання утиліти `willbe`, тому, для підключення такого підмодуля потрібно створити його експортну конфігурації і помістити посилання на локальний експортований файл в секцію `submodule`.  

![submodule.informal.png](./Images/submodule.informal.png)

На рисунку показано загальну послідовність створення неформального підмодуля. `Will-файл` неформального підмодуля об'єднує операції завантаження файлів з віддаленого сервера та експорту локального підмодуля. `Will-файл` модуля імпортує експортований локальний підмодуль.  
Перевагою цього способу є можливість автоматичної побудови і оновлення неформального підмодуля.
