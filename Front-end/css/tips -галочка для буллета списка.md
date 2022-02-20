# tips -галочка для буллета списка

## кога нужно создать для  маркированного списка маркер отличный от стандартного можно сделать следующее

*******
способ 1

использовать специальные символы  и псевдоэлемент before

html
````
<ul class="list">
		  <li class="list-item">text</li>
		  <li class="list-item">text</li>
		  <li class="list-item">text</li>
		  <li class="list-item">text</li>
		  <li class="list-item">text</li>
		  <li class="list-item">text</li>
	  </ul>

````
css
````
.list-item:before {
	content: '\2713';
}
````

\2713 -  сокращение для спецсивола птички

[[css псевдоэлемент]]
[[создание круглого буллета для элемента списка]]

#tips-for-work
#css