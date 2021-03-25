# CSS Questions

1. Main difference between CSS Flexbox and Grid

   - Flexbox works on a row or a column and Grid works for rows and columns at the same time.

2. Within a HTML body, I have a div where width and height are set to 100%, why I can see the width on the full screen but I can't see the full height applied?

   - The [User Agent Style](https://meiert.com/en/blog/user-agent-style-sheets/) (Latest Chrome) for the body tag is the following: `body { display: block; margin: 8px; }`. We need to focus on the display: block; because the block value by default, takes as much horizontal space as it can. So if we apply a 100% width value on the child element (the div) we can see that will be extended for the all length of the parent. The 100% height is not applied because body tag does not have such a standard height, if we change the parent's height the child will be going as much as it can with its own height value.
     An example can be found on the file `2.html`

3. What techniques will you use for making a a website responsive?

   - I will personally use [Media Query](https://www.w3schools.com/css/css_rwd_mediaqueries.asp) at most, because it makes life really easy and because queries are customizable.
