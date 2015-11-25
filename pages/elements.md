### Элементы

Элементы - это то, из чего состоят блоки. Основное отличие от блоков - это то, что они зависят от блоков и не могут использоваться вне блока. Вот пример элементов:

```html
<!-- Block -->
<div class="news">
	<!-- Elements -->
	<h2 class="news__title">
		News title
	</h2>
	<img src="#" alt="" class="news__img">
	<p class="news__text">
		Lorem ipsum dolor sit amet.
	</p>
	<footer class="news__footer">
		<div class="news__author">
			Andrew Fatuk
		</div>
		<div class="news__date">
			10.11.2015
		</div>
	</footer>
</div>
```

В примере видно, что блок новости состоит из 6 элементов:

* title
* img
* text
* footer
* author
* date

Зная из чего состоят те или иные блоки, не сложно посмотрить понятную и хорошо поддерживаемую структуру.


#### Часто используемые названия для элементов:

* list
* item
* link
* title
* text
* header
* footer
* container
* content
* inner
* wrapper
* btn
* counter
* info
* row
* column
* label

Это, на мой взгляд, наиболее часто используемые общие названия. Бывают, конечно, и более специфичные. Все зависит от потребностей.
