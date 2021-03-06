# Section <code>exported</code>

Секція <code>out-will-файла</code>, програмно генерується при експортуванні модуля, містить перелік всіх експортованих файлів та використовується при імпортуванні даного модуля іншим.  
Головне призначення - інформаційна карта для імпорту.   

### Поля ресурсів секції `exported`   

| Поле                     | Опис                                   |
|--------------------------|----------------------------------------|
| version                  | версія модуля, експортується з секції `about`                         |
| description              | опис експортованого модуля - призначення, ліцензія, автори та ін.     |
| criterion                | критеріони, експортовані з секції `build` при виконанні збірки експорту (див. [критеріон](Criterions.md)) |
| inherit                  | наслідування, яке експортується з секції `build` при виконанні збірки |
| exportedReflector        | рефлектор, за яким побудовано експорт модуля, генерується утилітою    |
| exportedFilesReflector   | рефлектор на експортовані файли, генерується утилітою                 |  
| exportedDirPath          | експортовані директорії, що експотуються                              |
| exportedFilesPath        | шляхи до файлів, генерується утилітою                                 |
| archiveFilePath          | шлях до архівованих файлів створеного модулю                          |

Приклад секції `exported`:

![section.exported.png](./Images/section.exported.png)
