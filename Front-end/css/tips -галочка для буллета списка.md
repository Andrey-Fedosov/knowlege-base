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

------------
вариант через before

такой же html,

css

````
.list-item {
	position: relative;
	padding: 0px 0px 0px 50px;
}

.list-item:before {
	content: '';
	background: url('/free-fe/img/iconmonstr-check-mark-1.svg') 0 0 no-repeat;
	position: absolute;
	top: -2px;
	left: 0;
	width: 25px;
	height: 25px;
}
````
 заметка связана с:
[[css псевдоэлемент]]
[[создание круглого буллета для элемента списка]]

#tips-for-work
#css
#псевдоэлемент