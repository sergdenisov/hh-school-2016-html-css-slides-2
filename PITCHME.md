#HSLIDE

### HTML/CSS, часть 2

![HTML5/CSS3](images/HTML-CSS3.jpg)

Сергей Денисов

Старший фронтенд-разработчик


09.02.2017

#HSLIDE

### CSS: [flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes)

![CSS: flexbox](images/flexbox.png)

[Пример](https://jsfiddle.net/sergdenisov/95y31w8j/), [статья](http://frontender.info/a-guide-to-flexbox/).

#VSLIDE

Свойства flex-контейнера (родительского элемента):

```css
display: flex | inline-flex
flex-direction: row | row-reverse | column | column-reverse
flex-wrap: nowrap | wrap | wrap-reverse
flex-flow: <'flex-direction'> || <'flex-wrap'>
```

#VSLIDE

```css
justify-content: flex-start | flex-end | center |
                 space-between | space-around
```

![CSS: flexbox justify-content](images/justify-content.png)

#VSLIDE

```css
align-items: flex-start | flex-end | center |
             baseline | stretch
```

![CSS: flexbox align-items](images/align-items.png)

#VSLIDE

```css
align-content: flex-start | flex-end | center |
               space-between | space-around | stretch
```

![CSS: flexbox align-items](images/align-content.png)

#VSLIDE

Свойства дочерних элементов:

```css
order: <integer>
flex-grow: <number> (default 0)
flex-shrink: <number> (default 1)
flex-basis: <length> | auto (default auto)
flex: [<'flex-grow'> <'flex-shrink'>? || <'flex-basis'>]
      (default 0 1 auto)
align-self: auto | flex-start | flex-end | center |
            baseline | stretch
```

#HSLIDE

### CSS: [animation](https://developer.mozilla.org/en-US/docs/Web/CSS/animation)

```css
animation-name: none
animation-duration: 0s
animation-timing-function: ease
animation-delay: 0s
animation-iteration-count: 1
animation-direction: normal
animation-fill-mode: none
animation-play-state: running
```

#VSLIDE

```css
@keyframes slide-in {
    0% { margin-left: 0; }
    100% { margin-left: 300px; }
}
div {
    width: 100px;
    height: 100px;
    background-color: tomato;
    animation: 3s ease-in 1s infinite slide-in;    
}
```

[Пример](https://jsfiddle.net/sergdenisov/j5ogte1k/1/).