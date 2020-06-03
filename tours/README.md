:gem: #### How to do background with image and linear gradient together

```css
/*Hero*/
.hero {
  width: 100%;
  height: 80vh;
  background: linear-gradient(135deg, rgba(49,24,131,0.9) 0%, rgba(72, 56, 149, 0.8) 100%), 
  		url("images/header-bg.jpg") center no-repeat;
}
```

:gem: ####  How to do lateral navbar

```javascript
const selectElement = (s) => document.querySelector(s);

//Open menu on click
selectElement('.open').addEventListener('click', () => {
	selectElement('.nav-list').classList.add('active');
});

//Close menu on click
selectElement('.close').addEventListener('click', () => {
	selectElement('.nav-list').classList.remove('active');
});

```

`nav-list` is the element with menu, `.open` is the element if on click the menu will show and `.close` is the element if on click the menu is hidden
