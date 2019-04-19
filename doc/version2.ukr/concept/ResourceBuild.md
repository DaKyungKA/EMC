## Ресурс збірка

Послідовність і умови виконання процедур побудови модуля. При виконанні команди <code>.build</code> розробник має вказати збірку, яку хоче зібрати, однозначно вибравши одну по імені або по умовам вибірки.

Найважливішим полем збірки є `steps` - сценарій збірки. Сценарій збірки - послідовність кроків, що потрібно виконати для того щоб збірка вважалася побудованою.

### Приклад

![section.build.png](./Images/section.build.png)

Приклад має ...

Kos : звичайна збірка і опис треба

### Поля ресурсів секції `build`  

| Поле          | Опис                                                             |
|---------------|------------------------------------------------------------------|
| description   | опис для інших розробників                                       |
| criterion     | умова побудови модуля (див. [критеріон](Criterions.md))          |
| steps         | послідовність кроків, що потрібно виконати для того щоб збірка вважалася побудованою ви                  |
| inherit       | наслідування від іншої збірки                        |

### Збірка за замовчуванням

Модуль може мати збірку за замовчуванням. Для того щоб зробити якусь збірку такою потрібно вказати для неї критеріон `default : 1`.

### Ресурс експорт

Kos : опис

### Секція <code>build</code>

Ресурси секції (збірки) описують послідовність і умови виконання процедур створення модуля.  