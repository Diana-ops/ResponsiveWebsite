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
