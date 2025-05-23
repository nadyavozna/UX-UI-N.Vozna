# Оптимізація зображень за допомогою Squoosh

## Виконала:
**Возна Надія**  
**Група:** ІПЗ-2.03

---

## Опис вихідних зображень

| Зображення                    | Формат | Вага       | Розмір     |
|-------------------------------|--------|------------|------------|
| Графічне зображення з текстом | JPG    | 140 061 байт (136 КБ) | 1063 х 591 |
| Фотографія                    | JPG    | 2 528 797 байт (2,41 МБ) | 3024 х 4032  |
| Скріншот                      | PNG    | 563 892 байт (550 КБ) | 1284 х 2778|

### Вага
![image](https://github.com/user-attachments/assets/9f03377e-d062-494b-92ec-f86a26e4bb26)
### Розміри
![image](https://github.com/user-attachments/assets/1919d332-1fb3-4c2b-802c-dd7514130ba9)

## Оригінальні файли
Оригінальне графічне зображення з текстом
![graphic-text](https://github.com/user-attachments/assets/7b79b4a5-83af-4f3c-b9fc-f5e7d1eb021c)

Оригінальна фотографія
![photo](https://github.com/user-attachments/assets/b79773d1-64f7-4753-b0e3-53871ce10fe9)

Оригінальний скріншот
![screen](https://github.com/user-attachments/assets/7547651b-e239-4541-85dc-3a24cdebdb35)

---
## Порівняння після різних типів стиснення
### PNG (Lossless)

| Зображення                    | Формат | Оригінальна вага | Вага після стиснення |Розмір      |
|-------------------------------|--------|------------------|----------------------|------------|
| Графічне зображення з текстом | JPG    | 136 КБ           | 134 КБ               | 1063 х 591 |
| Фотографія                    | JPG    | 2,41 МБ          | 13,2 МБ              | 3024 х 4032|
| Скріншот                      | PNG    | 550 КБ           | 579 КБ               | 1284 х 2778|

![image](https://github.com/user-attachments/assets/91843f4b-336a-4583-9945-857307e4ee52)

### PNG (Lossless) файли
PNG (Lossless) графічне зображення з текстом
![graphic-text](https://github.com/user-attachments/assets/0d45334b-5d31-4fe8-bb48-cf5f606ff91f)

PNG (Lossless) фотографія
[![PNG (Lossless) фотографія](images/PNG%20%28Lossless%29/photo.png)](images/PNG%20%28Lossless%29/photo.png)

PNG (Lossless) скріншот
![screen](https://github.com/user-attachments/assets/1f1b303c-3338-4f01-9d03-aae14eeac1b6)

## Висновок:
Стиснення PNG lossless неефективне, оскільки файли або збільшуються в розмірі, або зменшуються незначно. Найкращий результат показав формат зображення «Графічне зображення з текстом», але лише на 1.47%, що майже нічого не змінило

---
### WebP (Lossless)

| Зображення                    | Формат | Оригінальна вага | Вага після стиснення |Розмір      |
|-------------------------------|--------|------------------|----------------------|------------|
| Графічне зображення з текстом | JPG    | 136 КБ           | 65,4 КБ               | 1063 х 591 |
| Фотографія                    | JPG    | 2,41 МБ          | 6,58 МБ              | 3024 х 4032|
| Скріншот                      | PNG    | 550 КБ           | 288 КБ               | 1284 х 2778|

![image](https://github.com/user-attachments/assets/c9d4ec56-ab72-4d4b-8551-8d6943a3f502)

### WebP (Lossless) файли
WebP (Lossless) графічне зображення з текстом
![image](https://github.com/user-attachments/assets/54a61d19-c6e3-4dfa-ac30-81b40b56dba9)

WebP (Lossless) фотографія
[![WebP (Lossless) фотографія](images/WebP%20%28Lossless%29/photo.webp)](images/PNG%20%28Lossless%29/photo.webp)

WebP (Lossless) скріншот
![image](https://github.com/user-attachments/assets/0b65b3fc-b201-4591-b264-7bf2e8502b9d)


## Висновок:

Формат WebP відмінно підходить для «Графічного зображення з текстом» і «Скріншота», але для фотографії він збільшує вагу.

---

**Висновки PNG та WebP (Lossless):** Для того, щоб зменшити вагу зображення типу «Скріншот» і «Графічне зображення з текстом», змінивши його формат без втрати якості, найкраще підійде варіант «WebP» з його середнім показником різницею у вазі до і після стиснення в 49.78%.

---


### MozJPEG (Lossy)
## Графічне зображення з текстом
| Формат | Якість | Оригінальна вага | Вага після стиснення |Розмір      |
|--------|--------|------------------|----------------------|------------|
| MozJPEG| 100%   | 136 КБ           | 113 КБ               | 1063 х 591 |
| MozJPEG| 75%    | 136 КБ           | 20,7 КБ              | 1063 х 591 |
| MozJPEG| 50%    | 136 КБ           | 14,4 КБ              | 1063 х 591 |

![image](https://github.com/user-attachments/assets/c08e3d6a-5a4b-40a9-a8a5-0edaa107dfed)

## Фотографія
| Формат | Якість | Оригінальна вага | Вага після стиснення |Розмір       |
|--------|--------|------------------|----------------------|-------------|
| MozJPEG| 100%   | 2,41 МБ          | 4,22 МБ              | 3024 х 4032 |
| MozJPEG| 75%    | 2,41 МБ          | 601 КБ               | 3024 х 4032 |
| MozJPEG| 50%    | 2,41 МБ          | 286 КБ               | 3024 х 4032 |

![image](https://github.com/user-attachments/assets/332b028a-aa15-4f28-ac66-a88f97197179)

## Скріншот
| Формат | Якість | Оригінальна вага | Вага після стиснення |Розмір       |
|--------|--------|------------------|----------------------|-------------|
| MozJPEG| 100%   | 550 КБ           | 530 КБ               | 1284 х 2778 |
| MozJPEG| 75%    | 550 КБ           | 105 КБ               | 1284 х 2778 |
| MozJPEG| 50%    | 550 КБ           | 74,2 КБ              | 1284 х 2778 |

![image](https://github.com/user-attachments/assets/54b61c27-bf86-483b-9b22-672b2d707f6f)

## MozJPEG (Lossy) 100% файли
![graphic-text100](https://github.com/user-attachments/assets/dd22b8c5-43ac-4f1c-9f1a-06e54c47b727)
![photo100](https://github.com/user-attachments/assets/57d0cd08-ce58-4165-9e90-46151a90eb8b)
![screen100](https://github.com/user-attachments/assets/c6f8c541-cf76-4e47-a64b-c4ab98b70ac2)

## MozJPEG (Lossy) 75% файли
![graphic-text75](https://github.com/user-attachments/assets/7c3d957b-21b3-42c3-9056-465bfb1d1144)
![photo75](https://github.com/user-attachments/assets/c6ce36e0-7afc-4cca-b481-a96a9c2c1478)
![screen75](https://github.com/user-attachments/assets/40e1106c-85aa-4a54-a93a-1e9b2a22a1ce)

## MozJPEG (Lossy) 50% файли
![graphic-text50](https://github.com/user-attachments/assets/9964040b-1540-4541-9914-af49b2be9a7f)
![photo50](https://github.com/user-attachments/assets/62c3bcfe-d2fc-4383-87ce-dc157d9fec15)
![screen50](https://github.com/user-attachments/assets/b8a5eca4-16e8-4611-834c-526231b3e350)

## Висновки MozJPEG (Lossy) 100% / 75% / 50%
# “Графічне зображення з текстом” показники:
● Якість 100% - вага зменшилася на 16.91%

● Якість 75% - вага зменшилася на 84.78%

● Якість 50% - вага зменшилася на 89.41%

Якість на 50% і 75% погіршилася. Навіть без зумування зображення можна помітити зміни в гірший бік.

---

# “Фотографія” показники:
● Якість 100% - вага *збільшилася* на 75.17%

● Якість 75% - вага зменшилася на 75.63%

● Якість 50% - вага зменшилася на 88.40%

Якість на 50%, 75% і 100% зображення знаходиться приблизно на одному рівні.
Що з приводу ваги, то найкращий результат, як не дивно, показала якість 50%.
Якщо враховувати, що вага зменшилася приблизно на 88.40%, то це досить приємно.

**Хороший формат** для зображення типу «Фотографія», але при 100% якості – вага збільшилася приблизно на 75.17%, що досить неприємно.

---

# “Скріншот” показники:
● Якість 100% - вага зменшилася на 3.64%

● Якість 75% - вага зменшилася на 80.91%

● Якість 50% - вага зменшилася на 86.51%

Якість на 50% і 75% зображення перебуває приблизно на одному рівні,
але якщо почати зумувати, то стає помітно зміни у якості тексту, як і на зображенні типу «Графічне зображення з текстом».
**Добре** підійде для зображень типу «Скріншот».

---
## Загальний висновок:
Цей формат найкраще підходить для зображення типу «Фотографія».
Не так добре показав себе цей формат під час роботи з будь-яким текстом або графічними об'єктами.

---
### WebP (Lossy)
## Графічне зображення з текстом
| Формат | Якість | Оригінальна вага | Вага після стиснення |Розмір      |
|--------|--------|------------------|----------------------|------------|
| WebP| 100%   | 136 КБ           | 37,1 КБ              | 1063 х 591 |
| WebP| 75%    | 136 КБ           | 13,1 КБ              | 1063 х 591 |
| WebP| 50%    | 136 КБ           | 10,9 КБ              | 1063 х 591 |

![image](https://github.com/user-attachments/assets/8ca038b4-6c2a-4c4a-9d58-179c472ddfd0)

## Фотографія
| Формат | Якість | Оригінальна вага | Вага після стиснення |Розмір       |
|--------|--------|------------------|----------------------|-------------|
| WebP| 100%   | 2,41 МБ          | 3,09 МБ              | 3024 х 4032 |
| WebP| 75%    | 2,41 МБ          | 342 КБ               | 3024 х 4032 |
| WebP| 50%    | 2,41 МБ          | 200 КБ               | 3024 х 4032 |

![image](https://github.com/user-attachments/assets/e591867d-5c60-4db2-8469-4635ba41d0fd)

## Скріншот
| Формат | Якість | Оригінальна вага | Вага після стиснення |Розмір       |
|--------|--------|------------------|----------------------|-------------|
| WebP| 100%   | 550 КБ           | 189 КБ               | 1284 х 2778 |
| WebP| 75%    | 550 КБ           | 66,6 КБ              | 1284 х 2778 |
| WebP| 50%    | 550 КБ           | 54,1 КБ              | 1284 х 2778 |

![image](https://github.com/user-attachments/assets/0a928895-611f-495b-afe0-3b7442cb8223)

## WebP (Lossy) 100% файли
![image](https://github.com/user-attachments/assets/bb59eceb-39d3-414f-98fd-af50c1438cce)
[![WebP (Lossy) фотографія](images/WebP%20%28Lossy%29/photo100.webp)](images/PNG%20%28Lossy%29/photo100.webp)
![image](https://github.com/user-attachments/assets/e9826d64-6cb2-4121-a778-b43853005058)

## WebP (Lossy) 75% файли
![image](https://github.com/user-attachments/assets/33e89ce8-b2ae-4342-a88c-a99abe07e37d)
[![WebP (Lossy) фотографія](images/WebP%20%28Lossy%29/photo75.webp)](images/PNG%20%28Lossy%29/photo75.webp)
![image](https://github.com/user-attachments/assets/d3f08273-67a4-4c7a-99e3-39d0b1e702bf)

## WebP (Lossy) 50% файли
![image](https://github.com/user-attachments/assets/e8abdee7-d2f3-4b05-b677-5d2eb80f55e6)
![image](https://github.com/user-attachments/assets/46f00214-ef2a-4825-929a-7d8b2989ac92)
![image](https://github.com/user-attachments/assets/53fb8751-8ae0-4cfe-be08-e29f3781f8e3)

## Висновки WebP (Lossy) 100% / 75% / 50%
# “Графічне зображення з текстом” показники:
● Якість 100% - вага зменшилася на 72,72%

● Якість 75% - вага зменшилася на 90,37%

● Якість 50% - вага зменшилася на 91,98%

Якість на 50% і 75% погіршилася. Навіть без зумування зображення можна помітити зміни в гірший бік. Але в усіх випадках вага зменшилася білше ніж на 70%.

---

# “Фотографія” показники:
● Якість 100% - вага *збільшилася* на 28,34%

● Якість 75% - вага зменшилася на 86,13%

● Якість 50% - вага зменшилася на 91,89%

Якість на 50%, 75% і 100% зображення знаходиться приблизно на одному рівні.
Що з приводу ваги, то найкращий результат, як не дивно, показала якість 50%.
Якщо враховувати, що вага зменшилася приблизно на 91,89%, то це досить приємно.

**Хороший формат** для зображення типу «Фотографія», але при 100% якості – вага збільшилася приблизно на 28,34%, що досить неприємно.

---

# “Скріншот” показники:
● Якість 100% - вага зменшилася на 65,64%

● Якість 75% - вага зменшилася на 87,89%

● Якість 50% - вага зменшилася на 90,18%

Якість на 50% і 75% зображення перебуває приблизно на одному рівні,
але якщо почати зумувати, то стає помітно зміни у якості тексту, як і на зображенні типу «Графічне зображення з текстом».
100% показав хороший результат, тим що без втрати якості стиснув вагу зображення більше ніж на 65%.
**Добре** підійде для зображень типу «Скріншот».

---
## Загальний висновок:
Цей формат найкраще підходить для зображення типу «Фотографія».
Не так добре показав себе цей формат під час роботи з будь-яким текстом або графічними об'єктами. Але якщо зображення типу “Скріншот”, то це ідеальний варіант у якості 100%.

---

### AVIF (Lossy)
## Графічне зображення з текстом
| Формат | Якість | Оригінальна вага | Вага після стиснення |Розмір      |
|--------|--------|------------------|----------------------|------------|
| AVIF| 100%   | 136 КБ           | 32,6 КБ              | 1063 х 591 |
| AVIF| 75%    | 136 КБ           | 12,1 КБ              | 1063 х 591 |
| AVIF| 50%    | 136 КБ           | 7,84 КБ              | 1063 х 591 |

![image](https://github.com/user-attachments/assets/b502ce0e-b7c8-4374-b3e4-65a11d9ea01a)

## Фотографія
| Формат | Якість | Оригінальна вага | Вага після стиснення |Розмір       |
|--------|--------|------------------|----------------------|-------------|
| AVIF| 100%   | 2,41 МБ          | 2,61 МБ              | 3024 х 4032 |
| AVIF| 75%    | 2,41 МБ          | 677 КБ               | 3024 х 4032 |
| AVIF| 50%    | 2,41 МБ          | 110 КБ               | 3024 х 4032 |

![image](https://github.com/user-attachments/assets/0fe940fd-9ec0-4210-ae75-9fdbf2996f6b)


## Скріншот
| Формат | Якість | Оригінальна вага | Вага після стиснення |Розмір       |
|--------|--------|------------------|----------------------|-------------|
| AVIF| 100%   | 550 КБ           | 194 КБ               | 1284 х 2778 |
| AVIF| 75%    | 550 КБ           | 70,4 КБ              | 1284 х 2778 |
| AVIF| 50%    | 550 КБ           | 40,6 КБ              | 1284 х 2778 |

![image](https://github.com/user-attachments/assets/ebc84952-9865-44c1-b634-addf2b6e2eeb)

## AVIF (Lossy) 100% файли
[![AVIF (Lossy)](images/AVIF%20%28Lossy%29/graphic-text100.avif)](images/AVIF%20%28Lossy%29/graphic-text100.avif)
[![AVIF (Lossy)](images/AVIF%20%28Lossy%29/photo100.avif)](images/AVIF%20%28Lossy%29/photo100.avif)
[![AVIF (Lossy)](images/AVIF%20%28Lossy%29/screen100.avif)](images/AVIF%20%28Lossy%29/screen100.avif)

## AVIF (Lossy) 75% файли
[![AVIF (Lossy)](images/AVIF%20%28Lossy%29/graphic-text75.avif)](images/AVIF%20%28Lossy%29/graphic-text75.avif)
[![AVIF (Lossy)](images/AVIF%20%28Lossy%29/photo75.avif)](images/AVIF%20%28Lossy%29/photo75.avif)
[![AVIF (Lossy)](images/AVIF%20%28Lossy%29/screen75.avif)](images/AVIF%20%28Lossy%29/screen75.avif)

## AVIF (Lossy) 50% файли
[![AVIF (Lossy)](images/AVIF%20%28Lossy%29/graphic-text50.avif)](images/AVIF%20%28Lossy%29/graphic-text50.avif)
[![AVIF (Lossy)](images/AVIF%20%28Lossy%29/photo50.avif)](images/AVIF%20%28Lossy%29/photo50.avif)
[![AVIF (Lossy)](images/AVIF%20%28Lossy%29/screen50.avif)](images/AVIF%20%28Lossy%29/screen50.avif)

## Висновки AVIF (Lossy) 100% / 75% / 50%
# “Графічне зображення з текстом” показники:
● Якість 100% - вага зменшилася на 76.03%

● Якість 75% - вага зменшилася на 91.10%

● Якість 50% - вага зменшилася на 94.24%

Щодо елементів, які є на зображенні, то ідеал – це 75% якості,бо за 50% якості деякі об'єкти втрачають свою форму (розпливаються).Якщо потрібно більше якості, то варіант зі 100% підійде краще,оскільки якість у цього варіанту як в оригіналу.

---

# “Фотографія” показники:
● Якість 100% - вага *збільшилася* на 8,41%

● Якість 75% - вага зменшилася на 72.54%

● Якість 50% - вага зменшилася на 95.54%

Щодо елементів, які є на зображенні, то ідеал – це 75% якості, бо за 50% якості елементи розпливаються при зумі зображення. Якщо потрібно більше якості, то варіант зі 100% підійде краще, оскільки якість у цього варіанту як в оригіналу, але вага більше ніж в оригіналу на 8,41%.

---

# “Скріншот” показники:
● Якість 100% - вага зменшилася на 65,64%

● Якість 75% - вага зменшилася на 87,89%

● Якість 50% - вага зменшилася на 90,18%

Найкращий результат. Усі варіанти добре. Найкраще використовувати варіант зі 100% якістю зображення, оскільки вага зображення зменшилася більш ніж на 65%, а якість залишилася такою самою. Щодо варіантів із 50% і 75%, то за якістю вони трохи різняться під час масштабування зображення, а вага зменшилася практично на рівний відсоток.

---
## Загальний висновок:
Найкраще використовувати це розширення файлу для стиснення зображень типу «Скріншот», на другому місці – «Графічне зображення з текстом», і на останньому – «Фотографія».
Особисто я використовувала би цей формат для «Скріншотів», оскільки стиснення без втрати якості більше ніж в 2 рази дуже приваблює.

## Загальні висновки щодо lossless та lossy

### Lossless:
- Найкращим форматом для без втрати якості є WebP lossless, оскільки він суттєво зменшує вагу зображень типу «Скріншот» і «Графічне зображення з текстом» (до 64% від початкової ваги).
- PNG lossless показав гірші результати – у деяких випадках вага зображення навіть збільшувалася.

### Lossy:
AVIF lossy показав найкращі результати серед форматів зі стисненням із втратами.

● Найкраще підходить для «Скріншотів» (стиснення до 95% без суттєвої втрати якості).
● Оптимальний варіант для «Графічних зображень з текстом» – 75% якості.
  
WebP lossy добре підходить для «Фотографій» (стиснення до 80%), але погано справляється з текстом і тонкими деталями.

MozJPEG lossy добре стискає «Фотографії», але втрачає якість на «Скріншотах» і «Графічних зображеннях з текстом».

## Висновок:
● Без втрати якості – найкращий вибір WebP lossless.

● Стискання з втратами – оптимальний формат AVIF lossy (75% або 100% якості залежно від типу зображення).

● MozJPEG та WebP lossy варто використовувати лише для «Фотографій», але не для текстових або графічних зображень.

---

## Оптимізація розміру відповідно до цільового використання

### Для вебу: максимальна ширина 1200 px

| Зображення                    | Формат | Вага до стиснення|Вага після стиснення| Розмір до стиснення| Розмір після стиснення |
|-------------------------------|--------|------------------|--------------------|--------------------|----------------------|
| Графічне зображення з текстом | PNG    | 136 КБ           | 184 КБ             |1063 х 591          |1200 х 667            |
| Фотографія                    | PNG    | 2,41 МБ          | 2,47 МБ            |3024 х 4032         |1200 х 1600           |
| Скріншот                      | PNG    | 550 КБ           | 510 КБ             |1284 х 2778         |1200 х 2596           |

![image](https://github.com/user-attachments/assets/8f980eb7-d3a2-4bdf-af44-cfd4c58482d0)

![image](https://github.com/user-attachments/assets/f153497a-dbe1-49e5-8524-542708b37613)

### Файли для вебу: максимальна ширина 1200 px

Графічне зображення з текстом

![graphic-text](https://github.com/user-attachments/assets/1916e557-36fa-4e73-9cf5-35eb40851163)

Фотографія

![photo](https://github.com/user-attachments/assets/11e4b720-b14b-4aea-a6fe-98403f51c969)

Скріншот

![screen](https://github.com/user-attachments/assets/fd613f92-d23d-43d9-89f0-dca7c1de8296)

---

### Для мобільних пристроїв: максимальна ширина 600 px

| Зображення                    | Формат | Вага до стиснення|Вага після стиснення| Розмір до стиснення| Розмір після стиснення |
|-------------------------------|--------|------------------|--------------------|--------------------|----------------------|
| Графічне зображення з текстом | PNG    | 136 КБ           | 64,6 КБ            |1063 х 591          |600 х 333             |
| Фотографія                    | PNG    | 2,41 МБ          | 733 КБ             |3024 х 4032         |600 х 800             |
| Скріншот                      | PNG    | 550 КБ           | 172 КБ             |1284 х 2778         |600 х 1298            |

![image](https://github.com/user-attachments/assets/12110a68-2dc7-4acf-9567-b595f12999e4)

![image](https://github.com/user-attachments/assets/695b6701-8115-46a7-9911-c3747cb4ee55)

### Файли для мобільних пристроїв: максимальна ширина 600 px

Графічне зображення з текстом

![graphic-text](https://github.com/user-attachments/assets/8ae7ed64-63d1-40ec-a02f-bbf8b69600cd)

Фотографія

![photo](https://github.com/user-attachments/assets/849f11d7-9406-4ce5-8abf-3ecea2820faa)

Скріншот

![screen](https://github.com/user-attachments/assets/111d0146-7053-4573-b992-c65b463920e3)

---

### Для Retina-дисплеїв: створіть 3x версію зображення

| Зображення                    | Формат | Вага до стиснення|Вага після стиснення| Розмір до стиснення| Розмір після стиснення |
|-------------------------------|--------|------------------|--------------------|--------------------|----------------------|
| Графічне зображення з текстом | PNG    | 136 КБ           | 798 КБ             |1063 х 591          |3189 х 1773           |
| Фотографія                    | PNG    | 2,41 МБ          | 65,9 МБ            |3024 х 4032         |9072 х 12096          |
| Скріншот                      | PNG    | 550 КБ           | 2,73 МБ            |1284 х 2778         |3852 х 8334           |

![image](https://github.com/user-attachments/assets/78eede03-0461-48a6-98bd-32a3504706bc)

![image](https://github.com/user-attachments/assets/e4b2101f-f8ef-43e7-99a6-20343ba50e69)

### Файли для Retina-дисплеїв: створіть 3x версію зображення

Графічне зображення з текстом

![graphic-text](https://github.com/user-attachments/assets/0f329e91-372b-4284-84f4-9062654ae543)

Фотографія

Оскільки файл надто великий також і для додавання в папку, залишаю посилання на зображення на Гугл Диск.
https://drive.google.com/file/d/1SstcgSqGQJkAd1DWUhxNVZPTUvVb8ifH/view?usp=sharing

Скріншот

![screen](https://github.com/user-attachments/assets/b35e7839-8aec-4b7f-92c7-e00406ae3485)

## Висновки щодо оптимізації зображень

### Для вебу (максимальна ширина 1200 px):

Стиснення зображень дало різні результати:

- **Графічне зображення з текстом** *збільшилося* в розмірі на 35%.
- **Фотографія** також трохи *збільшилась* (+2,5%), що свідчить про неефективність PNG при масштабуванні чи збереженні з високою якістю.
- **Скріншот** показав незначне зменшення ваги (-7%), що є позитивним, хоча й не суттєвим.

Загалом, PNG не забезпечує ефективного стиснення для вебу при таких параметрах, краще використовувати WebP або AVIF.

---

### Для мобільних пристроїв (максимальна ширина 600 px):

Стиснення виявилося ефективним:

- **Графічне зображення з текстом** зменшилось на 53%, що робить його ідеальним для мобільного перегляду.
- **Фотографія** зменшилася на 70%, значно знижуючи навантаження на трафік і пам’ять.
- **Скріншот** зменшився на 69%, що також є чудовим показником оптимізації.

Це демонструє ефективність адаптації зображень до мобільного формату зменшеної ширини, навіть у форматі PNG.

---

### Для Retina-дисплеїв (3x версія):

Збільшення розміру зображень для підтримки високої щільності пікселів має значний вплив:

- **Графічне зображення з текстом** *збільшилось* на 487%, що є очікуваним при масштабуванні до 3x.
- **Фотографія** зросла в розмірі більш ніж у 27 разів (+2635%), до 65,9 МБ — це вимагає обережного використання та, можливо, альтернативного формату.
- **Скріншот** збільшився на 396%, що менш критично, але теж ДУЖЕ суттєво.

Підтримка Retina-дисплеїв значно підвищує вимоги до обсягу даних. Варто використовувати формати з кращим стисненням (WebP/AVIF) і контролювати розміри, щоб уникати перевантаження сторінок.

---

**Загальний висновок:**  
Для адаптивного веб-дизайну критично обирати правильні формати і оптимізувати розміри залежно від цільового пристрою. PNG не завжди забезпечує ефективне стиснення, особливо для високоякісних зображень і Retina-дисплеїв. Рекомендується застосовувати сучасні формати з високим рівнем стиснення.
