### Распространенные ошибки

1. Не используйте элементы вне блока, к которому они привязаны. Даже если элементы одинаковые. В случае, если они действительно одинаковые, нужно вынести такие элементы в отдельный блок или представить, что их одинаковость это совпадение и стили написать для каждого эелемента отдельно. (ПЕРЕПИСАТЬ БОЛЕЕ ПОНЯТНО)

```html
<div class="news">
	<h2 class="news__title">
		This is news title
	</h2>
</div>
<!-- /////////////////////////////////// -->
<article class="article">
	<h2 class="news__title">
		This is article title but the same as news title
	</h2>
</article>
```

2. Не разбивайте сложные имена классов подчеркиванием `_`. Используйте дефис `-`

```html
<div class="block">
	<h2 class="block__my_special_title">
		Wrong title
	</h2>
</div>
<!-- ///////////////////////////////// -->
<div class="block">
	<h2 class="block__my-special-title">
		Right title
	</h2>
</div>
```

[<- Оглавление](../README.md)
