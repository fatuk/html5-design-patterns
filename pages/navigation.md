### Навигация

Список из однородных элементов принято делать ненумерованным списком `<ul>`. Нельзя сказать, что это неприложное правило, но список добавляет дополнительную семантику.
К блокам навигации можно отнести:
* menu
* breadcrumbs
* pagination

По сути навигация - это просто набор ссылок.

```html
<nav class="menu">
	<ul class="menu__list">
		<li class="menu__item">
			<a class="menu__link menu__link_active">
				Home
			</a>
		</li>
		<li class="menu__item">
			<a class="menu__link">
				News
			</a>
		</li>
		<li class="menu__item">
			<a class="menu__link">
				Contacts
			</a>
		</li>
	</ul>
</nav>
```
