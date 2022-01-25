# Frontend Mentor - NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/nft-preview-card-component-SbdUL_w0U). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Links

- Solution URL: https://github.com/itspavit/nftpavit.github.io
- Live Site URL: https://itspavit.github.io/nftpavit.github.io/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid


### What I learned

![hover](https://user-images.githubusercontent.com/92730827/150962329-a6518d5e-9d1b-4e5e-88ab-155819fabfde.png)

The most tricky part was to add an hover overlay effect on the equilibrium image. I used the transition property and opacity property to hide the view icon and then upon hovering over the equilibrium image you can see a cyan background upon hover. The following is the code for it.

.equilibrium-img img {
  /* overflow: hidden; */
  max-width: 100%;
  width: 250px;
  border-radius: 16px;
  opacity: 1;
}

.eyeicon-img img {
  position: absolute;
  transition: 0.5 ease;
  opacity: 0;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: fit-content;
}

.img-holder:hover .equilibrium-img img {
  opacity: 0.7;
}

.img-holder:hover .eyeicon-img img {
  opacity: 1;
}

.img-holder:hover {
  background-color: var(--Cyan);
}


### Continued development

In future i will try to use grid and hopefully i will remake this project when i learn SASS.

### Useful resources

I took alot of help from w3schools.com
Also the slack channel for fronendmentor.io gave me good ideas when i got stuck.

## Author

Pavitpal Singh Bhagat
