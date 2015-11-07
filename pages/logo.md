### Логотип

Этот блок есть почти на каждом сайте и было бы странно верстать его каждый раз по-разному.
Давайте рассмотрим как вообще его можно реализовать.

Такую конструкцию нам предлагает Google. Это верстка логотипа в поисковой выдаче:

```html
<!-- Google -->
<h1>
	<a id="logo" href="https://www.google.ru/webhp?hl=ru" title="Главная страница Google">
		<img width="167" height="410" src="/images/nav_logo242.png" alt="Google">
	</a>
</h1>
```

А так выглядит логотип на главной Yahoo! Изображение они поместили на background.

```html
<!-- Yahoo -->
<h1>
    <a href="http://hsrd.yahoo.com/_ylt=AvPAejvyhR0Y0xj.2yfhI4KbvZx4/RV=1/RE=1448109009/RH=aHNyZC55YWhvby5jb20-/RO=2/RU=aHR0cHM6Ly93d3cueWFob28uY29tLw--/RS=^ADAFYdbmOZ2We_J9Cvteu2s0acrivk-" id="yucs-logo-ani" class="y-logo-new ml-xs ti">
    	Yahoo
    </a>
</h1>
```

Похожая картина наблюдается и у Яндекса:

```html
<!-- Yandex -->
<div class="logo logo_lang_ru i-bem logo_js_inited">
	<a class="logo__link" href="//www.yandex.ru/" tabindex="-1">
		Яндекс
	</a>
</div>
```

Плюсы использования фонового изображения:
* поддержка ретины (растровая графика)
* спрайты

Минусы:
* неудобно менять изображение, только в CSS
* неявное объявление изображения

При использовании формата svg плюсы невелируются. Поэтому я предпочитаю такой блок логотипа:

```html
<!-- My way -->
<h1 class="logo">
	<a href="#" class="logo__link">
		<img src="#" width="100" height="50" alt="Logo" class="logo__img">
	</a>
</h1>
```
Говорят для SEO оптимизации тег `<h1>` должен быть один на страницу. В любом случае методология БЭМ позволяет менять теги, т.к. мы не привязываемся к их именам. Также мы можем легко отказаться от ссылки в случае, если мы уже находимся на данной странице.

```html
<!-- My way -->
<div class="logo">
	<img src="#" width="100" height="50" alt="Logo" class="logo__img">
</div>
```

[<- Оглавление](../README.md)
