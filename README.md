Viewport-Action
===============
Плагин для создания эффектых лейдинг страниц.
Добавляет динамику для элементов при появлении их в области просмотра.

### Использование
1. Подключить jQuery
2. Подключить файлы плагина jquery.viewportaction.js и effect.css
3. Вызвать плагин, где elem - ваш элемент
`$('elem').viewportaction({})`

#### Деление страницы на блоки соответсвующие области видимости
1. Объединить элемент единым классом, например .row
2. Вызвать плагин с параметром oneRowViewport в значении true
`$('.row').viewportaction({ oneRowViewport: true})`

#### Создание навигации по блокам
1. Для блоков добавить служебный атрибут data-nav-viewport со значением true
`data-nav-viewport="true"` 
2. Для блоков добавить атрибут data-nav-viewport-title со значением, которые вы хотите видеть в качестве текста в навигации к текущему блоку
` data-nav-viewport-title="Секрет успеха"` 

(Навигации работает только при если параметр oneRowViewport установлен в true.)

### Параметры
Список доступных параметров:
<table>
    <tr>
      <th>Параметр</td>
      <th>Описание</th>
      <th>Тип</th>
    </tr>
    <tr>
      <td>effect</td>
      <td>Эффект, который будет применен к элементу</td>
      <td><i>Строка</i></td>
    </tr>
    <tr>
      <td>offsetTop</td>
      <td>На сколько px элемент должен войти в область просмотра, чтобы начать анимацию</td>
      <td><i>Число</i></td>
    </tr>
    <tr>
      <td>repeat</td>
      <td>Будет ли анимация повторятся, если скролить страницу несколько раз</td>
      <td><i>Boolean</i></td>
    </tr>
    <tr>
      <td>customClass</td>
      <td>Пользовательский класс для более гибкой настройки анимации</td>
      <td><i>Строка</i></td>
    </tr>
    <tr>
      <td>oneRowViewport</td>
      <td>Деление страницы на блоки соответсвующие области видимости</td>
      <td><i>Boolean</i></td>
    </tr>
    <tr>
      <td>viewportNav</td>
      <td>Включить навигацию по блокам страницы</td>
      <td><i>Boolean</i></td>
    </tr>
    <tr>
      <td>scrollSpeed</td>
      <td>Скорость скролла по блокам страницы</td>
      <td><i>Число</i></td>
    </tr>
</table>

### Доступные эффекты
Список доступных эффектов:
<table>
    <tr>
      <th>Эффект</td>
      <th>Описание</th>
    </tr>
    <tr>
      <td>fade</td>
      <td>Плавное появление элемента</td>
    </tr>
    <tr>
      <td>fadeTop</td>
      <td>Плавное появление элемента сверху</td>
    </tr>
    <tr>
      <td>fadeBottom</td>
      <td>Плавное появление элемента снизу</td>
    </tr>
    <tr>
      <td>fadeLeft</td>
      <td>Плавное появление элемента слева</td>
    </tr>
    <tr>
      <td>fadeRight</td>
      <td>Плавное появление элемента справа</td>
    </tr>
</table>

### Демонстрация

Пример смотреть <a href="http://m-ulyanov.github.io/viewport-аction/">здесь</a>

