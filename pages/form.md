### Форма

Чаще всего формы представляют собой набор строчек с двумя колонками внутри. В первой лейблы, во второй собственно поля. Такую структуру можно представить так:

```html
<!-- Form -->
<div class="form">
	<form action="#">
		<!-- Title -->
		<h2 class="form__title">
			Form title
		</h2>
		<div class="form__row">
			<div class="form__column">
				<label for="input-1" class="label">
					Field 1
				</label>
			</div>
			<div class="form__column">
				<!-- Field -->
				<div class="field">
					<input type="text" class="input" id="input-1">
				</div>
			</div>
		</div>
	</form>
</div>
```

Напрашивается вопрос: зачем мы используем обертку `<div class="field">` для текстового поля? Благодаря ей мы сможем легко добавить сообшение ошибки валидации и сообщение будет автоматически привязано к нужному полю.

```html
<!-- Form -->
<div class="form">
	<form action="#">
		<!-- Title -->
		<h2 class="form__title">
			Form title
		</h2>
		<div class="form__row">
			<div class="form__column">
				<label for="input-1" class="label">
					Field 1
				</label>
			</div>
			<div class="form__column">
				<!-- Field -->
				<div class="field">
					<input type="text" class="input" id="input-1">
					<!-- Error -->
					<div class="error">
						Enter correct data
					</div>
				</div>
			</div>
		</div>
	</form>
</div>
```
