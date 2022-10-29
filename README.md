# Frontend Mentor - Product preview card component solution


### What I learned

You can start with a:
mobile version: use flex-direction column for it
Switch to the desktop version: use grid and two columns.

To place image and text in one container, you can use two articles. To have two images to alternate for desktop and mobile version, you can use "picture" property. 

Picture tag allows multiple images can be designed to more nicely fill the browser viewport.There should be a default image. In this case, it is a mobile image


  ```html
  <picture> <source media="(min-width:640px)" srcset="images/image-product-desktop.jpg"/>
  <img src="images/image-product-mobile.jpg" alt="mobile-image">
  </picture>
  ```


1. Set max-width to 100%, so an image does not overflow the container.
```css
img {
    max-width: 100%;
}
```

2. Always set min-height and to turn it to a mobile version set it pixels.

```css
    min-height: calc(100vh-0.1px);
```


3. To remove bullets

```css
ul{
    list-style-type: none;
}
```

4. TO STOP CONTAINER FROM OVERFLOWING: set its  max-width to a number

```css
.container {
    max-width: 600px;
}
```

5. Repeat twice with 1 fraction of a column each to create a double row 

```css
     .container {
        display: grid; 
        grid-template-columns: repeat(2, 1fr);
    }

```


## Author

- Youtube - [Tsbsankara](https://www.youtube.com/watch?v=BMOH4zSLTnQ&t=1471s)

