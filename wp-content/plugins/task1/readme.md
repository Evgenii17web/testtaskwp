### Description

Плагін додає динамічний шорткод, за допомогою якого ви можете отримати назви продуктів. Ви можете обирати категорію та кількість назв. Перед активацієй плагіна активуйте плагін woocommerce, якщо він не активований. В плагіні є перевірка на те щоб woocommerce був ввімкненим перед активацією цього плагіну для корректної роботи.

### How to create a shortcode

1. Створити плагін
2. В коді плагіна використовується хук
   `add_shortcode('bags_products', 'bags_products');`, який реєструє шорткод у системі.
3. `bags_products()` - це функція-обробник, яка повертає дані, які будуть відображені на сторінці. Код можна знайти у файлі `wp-content/plugins/task1/add-shortcode-bags_products.php`

Також реєструвати шорткоди можна в файлі теми functions.php.


### How to get a list of products with custom parameters
За допомогою функції `wc_get_products` ми отримуєм від бази даних імена продуктів які можемо вивести на сторінку за допомогою шорткоду.

Використовуючи шорткод ми можемо передати атрибути `category` та `limit`, тобто вибрати категорію та кількість товарів. Якщо ви використовуєте дамп бази даних то побачити шорткод можно на головній сторінці.