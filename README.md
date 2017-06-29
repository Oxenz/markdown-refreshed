Настоящий документ предназначен для ознакомления пользователя с функциональными возможностями языка разметки Markdown. Markdown – это облегченный язык разметки, который является инструментом преобразования кода в HTML. Главной особенностью данного языка является максимально простой синтаксис, который служит для упрощения написания и чтения кода разметки, что, в свою очередь, позволяет легко его корректировать. Теперь рассмотрим более подробно функции языка разметки Markdown.

Markdown не является заменой HTML. Синтаксис Markdown достаточно ограничен, и соответствует лишь небольшому подмножеству элементов HTML. 


# Расмотртим основные конструкции с примерами.
### Разделим основные конструкции логически на _частые_ и _редкие_  
#                                     ↓   Частые   ↓
 
# строка
***
1. **[ Пустая строка ]**
***
_(Заметка)  
Для того, чтобы создать параграф с использованием синтаксиса языка Markdown, достаточно отделить строки текста одной (или более) пустой строкой (пустой считается всякая строка, которая не содержит в себе ничего, кроме пробелов и символов табуляции)._

**Что бы получить отступ ввиде пустой строки, необходимо разделить части текста всего лишь пустой строкой**  

___пример 1___ **↷**

        тут находиться текст написаный в два строки без привычной разделяющий пустой строки  
        тут находиться текст написаный в два строки без привычной разделяющий пустой строки
        
___пример 1.1___ **↷**
 
        тут находиться текст написаный в два строки с разделяющей пустой строкой  
        
        тут находиться текст написаный в два строки с разделяющей пустой строкой

***        
2. **[ Перенос строки ]**  
***
_(Заметка)  
Для того, чтобы вставить видимый перенос строки используйте элемент `<br/>`  
или окончите строку двумя пробелами и нажатием клавиши перевода строки «Enter». Многие элементы синтаксиса Markdown выглядят и работают гораздо лучше в случае, когда их форматируют с помощью «жесткого перевода строк» (разделение строк, осуществленное самим пользователем, а не программой автоматически). К таким элементам относятся цитаты, списки и пр. В "блоках кода" не обязательно использовать 2-а пробела, можно ограничиться привычным способом, просто сразу использую клавишу «Enter»_

**Чтобы перейти на следующую строку юзай не мене 1-го таба или 2-ух пробелов  
c последующим нажатием «Enter»  
или стандартный тег `<br/>`**

___пример 2___ **↷**

    Зимняя ночь
                 Мело, мело по всей земле
                 Во все пределы.
                 Свеча горела на столе,
                 Свеча горела.

                                                                                                  Борис Постернак ©
        
***
3. **[ Разделитель ]**
***
_(Заметка)  
Для того чтобы создать горизонтальную линию с использованием синтаксиса языка Markdown, необходимо поместить три (или более) дефиса или звездочки на отдельной строке текста. Между ними возможно располагать пробелы. При использовании данного инструмента важно помнить, что после первой части текста и перед второй необходимо оставлять пустую строку. Данное правило необходимо соблюдать только при использовании дефисов. Если его не соблюдать, на экран будет выведен заголовок второго уровня и строка обычного текста. При использовании символа звездочки данным правилом можно пренебречь._  

**Что бы получить разделяющую линию аналогичную тегу `<hr/>` используем одноименный тег, *** или ---**

___пример 3___ **↷**

        <hr/>
        ***
        ---

___пример 3.1___ **↷**

***
---
<hr/>

  

***
4. **[ Заголовки ]**
***
_(Заметка)  
Язык разметки Markdown поддерживает 2 стиля обозначения заголовков: подчеркивание и выделение символом («#»). Выделение заголовков с помощью подчеркивания производится знаками равенства («=») в случае, если заголовок первого уровня, и дефисами («-») в случае, если заголовок второго уровня. Количество знаков подчеркивания не ограничивается. При выделении заголовков с помощью символа («#») используется от одного до шести данных символов, которые устанавливаются в начале строки (перед заголовком). В данном случае количество символов соответствует уровню заголовка. Кроме того, заголовок возможно снабдить закрывающимися символами («#»), хотя это и не является обязательным. Количество закрывающихся символов не обязано соответствовать количеству начальных символов. Уровень заголовка определяется по количеству начальных символов.
Заголовки первого и второго уровней, выполненные с помощью подчеркиванияф.

**Заголовок можно создать 2-мя способами подчеркивая и выделя с помощью символов `#` или (тире) `-`**  

___пример 4___ **↷**

    Заголовок1 =
    =========
    Заголовок2 -
    ----------
    # Заголовок3.1 #1 (Всегда почеркивается тонкой горизонтальной чертой)
    ## Заголовок4.2 ##2 (Всегда почеркивается тонкой горизонтальной чертой)
    ### Заголовок5.3 ###3 LEVEL
    #### Заголовок6.4 ####4 LEVEL
    ##### Заголовок7.5 #####5 LEVEL
    ###### Заголовок8.6 ######6 LEVEL (минимальный)
    ####### Заголовок8.7 #######7 Level (ошибка, так-как всего 6 тегов h ((h1-h6)) в html )    


___пример 4.1___ **↷**

Заголовок1 =
=========

Заголовок2 -
----------

# Заголовок3.1 # 1 Level 
## Заголовок4.2 ## 2 Level
### Заголвок5.3 ### 3 Level                           size: 20px
#### Заголвок6.4 #### 4 Level                                          size: 16px
##### Заголвок7.5 ##### 5 Level
###### Заголвок8.6 ###### 6 Level                                                     size: 13,6px
####### Заголвок8.7 #######7 (Ошибка)              size: 16px

***
5. **[ Блоки кода ]**
***
_(Заметка)  
Отформатированные блоки кода используются в случае необходимости процитировать исходный код программ или разметки. Для создания блока кода в языке Markdown необходимо каждую строку параграфа начинать с отступа, состоящего из четырех пробелов или одного символа табуляции. Блок кода продолжается до тех пор, пока не встретится строка без отступа (или конец текста). Внутри блока кода амперсанды («&») и угловые скобки («<» и «>») автоматически преобразуются в элементы HTML разметки. Кроме того, следует отметить, что внутри блоков кода обычный синтаксис Markdown не обрабатывается._  

**Что бы создать такой блок нужно начинать с новой строки используя миниму 4-е пробела или один символ табуляци**

___пример 5___ **↷**

    это написано в "блоке кода"
    тут пробелами можно                               делать необходимые                отступы
    в данных блоках не действует магия MarkDown
        данные 
            символы 
                не обрабатываются <> & * ! + - и т.д.
    и даже ссылки [пример](http://example.com)

***
6. **[ Подсветка кода ]**
***
_(Заметка)  
Блоки кода в GitHub являются частью спецификации Markdown, но подсветка синтаксиса не является ее частью, поэтому рендеры, такие как Github и Markdown Here, поддерживают подсветку синтаксиса highlightJS. В зависимости от указанного языка в специально конструкции состоящей из трёх подряд обратных кавычек ` ```указать язык` синтаксис подвсветки будет меняться, количестов поддерживаемых языков исчесляется десятками с перечнем которых можно ознакомиться на [highlightjs.org](https://highlightjs.org/static/demo/) ._  

**Создавая блок с подсветкоей синтаксиса сперва указывает язык ` ```Java`➝ перевод на новую строку с "Enter" ➝  
конструкцию кода ➝ закрыть с новой строки обратными кавычками ` ``` `**

___пример 6___ **↷**

    ```JavaScript
    function fancyAlert(arg) {
        if(arg) {
            $.facebox({div:'#JavaScript syntax highlighting'})
        }
    }
    ```
    
    ```Python
    s = "Python syntax highlighting"
    print s
    ```
    
___пример 6.1___ **↷**

```Javascript
function fancyAlert(arg) {
    if(arg) {
        $.facebox({div:'#JavaScript syntax highlighting'})
    }
}
```

```Python
s = "Python syntax highlighting"
print s
```

```html
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>MarkDown hilightjs</title>
</head>
<body>
	<div class="main-wrapper">
		<div class="main">
			<p>Параграф с номером 1</p>
			<p>Параграф с номером 2</p>
			<p>Параграф с номером 3</p>
			<p>Параграф с номером 4</p>
			<p>Параграф с номером 5</p>
		</div>
	</div>
</body>
</html>
```

```css
#css-style {
    font-family: Lato, Arial, Helvetica, sans-serif;
	font-size: 25px;
    letter-spacing: 3px;
	color: #d47e7e;
    position: absolute;
	border: none;
	background: none;
}
```

```Java
package l2f.java.syntax;

public abstract class L2Char extends L2Object {
  public static final Short ERROR = 0x0001;

  public void moveTo(int x, int y, int z) {
    _ai = null;
    log("Should not be called");
    if (1 > 5) { // wtf!?
      return;
    }
  }
}
```

***
7. **[ Списки ]**
***
_(Заметка)  
Markdown поддерживает упорядоченные (нумерованные) и неупорядоченные (ненумерованные) списки. Для формирования неупорядоченный списков используются такие маркеры, как звездочки, плюсы и дефисы. Все перечисленные маркеры могут использоваться взаимозаменяемо. Для формирования упорядоченных списков в качестве маркеров используются числа с точкой. Важной особенностью в данном случае является то, что сами номера, с помощью которых формируется список, не важны, так как они не оказывают влияния на выходной HTML код. Как бы ни нумеровал пользователь список, на выходе он в любом случае будет иметь упорядоченный список, начинающийся с единицы (1, 2, 3…). Эту особенность стоит учитывать в том случае, когда необходимо использовать порядковые номера элементов в списке, чтобы они соответствовали номерам, получающимся в HTML. Упорядоченные списки всегда следует начинать с единицы. Маркеры списков обычно начинаются с начала строки, однако они могут быть сдвинуты, но не более чем на 3 пробела. За маркером должен следовать пробел, либо символ табуляции. При необходимости в список можно вставить цитату. В этом случае обозначения цитирования ( «>» ) нужно писать с отступом._ 

**Создать список можно с помощью символов `+` `-` `*` и `N.` где N - лубая цифра.**

___пример 7___ **↷**

⋅⋅⋅ Список1 какой он будет
⋅⋅ Список2 какой он будет
⋅ Список3 какой он будет
⋅⋅* Unordered sub-list. 

<hr/>

1. First ordered list item
2. Another item
  * Unordered sub-list. 
1. Actual numbers don't matter, just that it's a number
  1. Ordered sub-list
4. And another item.  

Тестовый текст






















Добавление ссылки происходит с помощью такой конструкции 
[текст]notspace(http://exemple.com) [Позновательный проект](http://htmlbook.ru)
или можно использовать прямую ссылку с помощью такой конструкции 
<сайт с указанием протокола> <http://сайт.рф>

Выделение `афро` цветом
***
    dir /fonts
    dir /images
    dir /js

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

> Текст
> 
> Продолжение текста выделенного блока
> Завершение текста

> Текст цитаты
> 
>> Продолжение текста выделенного блока
> Завершение текста

    Для создания блока CODE нужно поставить 4 символа пробела && 2 символ табуляции
    it block code
    Example: Title1 | Title2 | Title3
    <> code &
    
    код чере пустую строку
    
    
    
    &

Для создание зебровой таблицы нужно:  
создать ЗАГОЛОВКИ разделенные символом " | " подчеркнув их символом(и) тире " ----- "  
и разделяя их в нужных местах логически тем же символом " | "

    Заголовок1 | Заголовок2 | Заголвоок3
    -|-|-
    текст1|Текст2|Текст3

Заголовок1 | Заголовок2 | Заголвоок3
-|-|-
текст1|Текст2|Текст3

Пример
***
    Aliance | Horde  | Альянс  | Орда 
    --------|--------|---------|--------
    Human   | Orc    | Люди    | Орки
    NElf    | BElf   | НЭльфы  | БЭльфы  
    Gnome   | Tauren | Гномы   | Таурены 
    Dwarf   | Troll  | Дворфы  | Тролли
    Worgen  | Undead | Воргены | Нежить
    Draenei | Goblin | Дренеи  | Гоблины
    Panda   | Panda  | Панды   | Панды

Aliance | Horde  | Альянс  | Орда 
--------|--------|---------|--------
Human   | Orc    | Люди    | Орки
NElf    | BElf   | НЭльфы  | БЭльфы  
Gnome   | Tauren | Гномы   | Таурены 
Dwarf   | Troll  | Дворфы  | Тролли
Worgen  | Undead | Воргены | Нежить
Draenei | Goblin | Дренеи  | Гоблины
Panda   | Panda  | Панды   | Панды

**Дополнительные символы** 
Используя обратный слеш « \ » можно экранировать спецсимволы, таким образом используемые символы будут восприниматься в буквальном а не служебном состоянии, все ниже приведенные символы экранированы по типу \` \* \_ \# за исключением списказ "не нуждающихся"

\` обратный апостроф;

\* звездочка;

\_ символ подчеркивания;

\#  символ решетки;

\+ плюс;

\- минус (дефис);

### Не нуждаються в экранировании ###

\ слеш;

! восклицательный знак;

| вертикальная черта;

[] квадратные скобки;

{} фигурные скобки;

() круглые скобки;

— длинное тире;

. точка;

, запятая;


8888888888888888888888888

Тут буед находиться специальные символы
&lt; и &amp; записанные в кодировке  
а тут обычные символки с клавиатуры  
< и &

Чтобы вставить изображение нужна прямая ссылка с конструкцией ![Текстнеобязательно] (прямая ссылка)
![Вот такая вот gif](http://i.imgur.com/Vjf2rHg.gif)



**Добавление видео**
<a href="http://www.youtube.com/watch?feature=player_embedded&v=watch?v=SfSYrebXLDE
" target="_blank"><img src="http://img.youtube.com/vi/SfSYrebXLDE/sddefault.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

watch?v=SfSYrebXLDE

Как вариант в чистом MD можно вставить

[![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/SfSYrebXLDE/0.jpg)](http://www.youtube.com/watch?v=SfSYrebXLDE)

