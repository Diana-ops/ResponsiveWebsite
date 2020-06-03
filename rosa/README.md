![therosawallpaper](https://user-images.githubusercontent.com/46378210/83565443-cf975b80-a4f4-11ea-9ab0-0a49f4cb3b0d.PNG)

### Deploy 

> https://therosarestaurant.netlify.app/

### Resources 

:gem: Scroll with [UNPKG](https://unpkg.com/)

```html
<!-- Import Scroll in HTML -->
<script src="https://unpkg.com/scrollreveal"></script>
```
```javascript
/*Scroll of navbar in JS*/
window.sr = scrollReveal();

sr.reveal('.animate-left', {
	origin: 'left',
	duration: 1000,
	distances: '25rem',
	delay: 300
});

sr.reveal('.animate-right', {
	origin: 'right',
	duration: 1000,
	distances: '25rem',
	delay: 600
});
```

:gem: Icons and Font Style with [Font Awesome](https://fontawesome.com/6?next=%2F)

```html
<!--Font awesome CDN-->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.11.2/css/all.min.css">
```

:memo: <strong>Variables in CSS</strong>

```css
:root{
    --main-font: 'Source Sans Pro', sans-serif;
    --secondary-font: 'Herr Von Muellerhoff', cursive;
    --body-font: 'Cabin', sans-serif;
    --main-font-color-dark: #252525;
    --secondary-font-color: #c59d5f;
    --body-font-color: #515151;
}

html {
	/*Using variables*/
	font-family: var(--body-font);
}
```
:memo: <strong>Before and After</strong>

```css
.social-icons i:hover, 
.social-icons i:focus {
	color: var(--secondary-font-color);
}
```
:memo: <strong>Animations</strong>
```css

.sub-headline {
	font-size: 8.5rem;
	font-family: var(--secondary-font);
	color: var(--secondary-font-color);
	font-weight: 100;
	line-height: .4;
	letter-spacing:  2px;
	opacity: 0;
	animation: fadeUp .5s forwards;
	animation-delay: .5s;
}

/*Animations*/

@keyframes fadeUp {
	0% {
		transform: translateY(4rem);
	}

	100% {
		opacity: 1;
		transform: translateY(0);
	}
}
```

How to result, the element with class _sub-headline_ will appear from the outside to the inside of the page. First with `opacity: 0`, after with `opacity: 1`. 0% will be the characteristics in initial, before `delay`, the characteristics will be in 100%

#### Efect to icon animate always
```css
.back-to-top i {
	display: block;
	color: #fff;
	font-size: 2rem;
	padding: 2rem;
	animation: up 2s infinite;
}

@keyframes up {
	0% {
		opacity: 0;
	}

	50% {
		opacity: 1;
	}

	100% {
		opacity: 0;
		transform: translateY(-1rem);
	}
}
```
