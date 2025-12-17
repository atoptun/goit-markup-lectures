# Flex cheatsheet

Flexible Box Layout (Flexbox)

![Flex container](images/image_01.png)

## Container

Main axis, Cross axis

![Cross axis](images/image_03.png)

main-start, main-end, cross-start, cross-end

![Start, end points](images/image_04.png)

### display

```css
display: flex | inline-flex
```

### gap

проміжок між flex-елементами

``` css
gap: 8px;
row-gap: 8px;
column-gap: 8px;
```

### flex-direction

Властивість `flex-direction` задає напрямок головної осі, а отже визначає напрямок елементів у контейнері.

```css
flex-direction: row | row-reverse | column | column-reverse
```

![flex-direction](images/image_05.png)

### justify-content

Властивість `justify-content` керує позиціонуванням елементів на головній осі, від `main-start` до `main-end`.

```css
justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly
```

![justify-content](images/image_06.png)

### align-items

Властивість `align-items` керує розташуванням елементів вздовж поперечної осі `cross axis`. Це аналог `justify-content` тільки для іншої осі.

```css
align-items: stretch | flex-start | flex-end | center | baseline
```

![align-items](images/image_07.png)

### flex-wrap

Властивість `flex-wrap` дозволяє перетворити однорядковий контейнер на багаторядковий.

```css
flex-wrap: nowrap | wrap | wrap-reverse
```

![flex-wrap](images/image_08.png)

```css
.item {
  width: calc((100% - 2*10px) / 3);
}

/* 100% - кількість_проміжків_у_рядку * значення_одного_проміжку) / кількість_елементів_у_рядку */
```

### align-content

Керує вирівнюванням усіх рядків багаторядкового контейнера уздовж `cross axis`, якщо є вільне місце. Аналогічно тому, як `align-items` вирівнює елементи в кожному рядку. Ця властивість не діє, коли є лише один рядок елементів або в контейнері немає вільного місця за вертикаллю (явно не задана висота більше, ніж контент).

```css
align-content: flex-start | flex-end | center | space-between | space-around | space-evenly | stretch
```

![align-content](images/image_09.png)

