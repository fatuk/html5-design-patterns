### Наборы блоков

Если у нас уже есть блок и его нужно вывести много раз в одном месте, то лучше создать дополнительный блок, который будет представлять набор. Например, у нас есть блок `product` и нам нужно вывести его много раз в каталоге:

```html
<!-- Product set -->
<div class="products-set">
	<!-- Title -->
	<h2 class="products-set__title">
		Found products
	</h2>
	<ul class="products-set__list">
		<li class="products-set__item">
			<!-- Product -->
			<div class="product">
				<!-- Title -->
				<h2 class="product__title">
					Product name 1
				</h2>
				<!-- Price -->
				<div class="product__price">
					100$
				</div>
			</div>
		</li>
		<li class="products-set__item">
			<!-- Product -->
			<div class="product">
				<!-- Title -->
				<h2 class="product__title">
					Product name 2
				</h2>
				<!-- Price -->
				<div class="product__price">
					120$
				</div>
			</div>
		</li>
	</ul>
</div>
```

Набор позволяет нам не награмождать основной блок `product`, особенно, если набор усложниться в будущем.
