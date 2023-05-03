# General course's notes:

## Documentation:

https://tailwindcss.com/docs/installation

## General:

- Here we're just importing Tailwind via CDN in our HTML files to keep things simple, but there are better ways to use this framework (specially for big projects) and we'll see them later in the course (probably the examples will be in another repos).

- With Tailwind we don't need to write "pure CSS" files and worry about them getting too big, we don't need to worry about classes names and it's easier/faster to test things out by just changing the values inside the "class" attribute of the HTML elements and see the results.

## Colors:

- The colors **black** and **white** don't have **shades**, but when we're using other colors we **must** specify a shade (from 50 to 950 and excluding the beggining and the end we must step by 100), otherwise it'll show as black (e.g. text-red-500).
  - If we need to **customize our palette**, we can configure our colors under the **colors key** in the **theme section** of your **tailwind.config.js** file, see the documentatio for more info.
- If we need to add color to a **border**, first we need to add the "base" **border** class and then the "modifier class" like **border-red-500**.
- If we need to add color to a **"divider"** (to divide items with a line), first we need to add the "base" **divide-y** (vertically in this case) class and then the "modifier class" like **divide-blue-300**.
- If we need to add color to an **outline**, first we need to add the "base" **outline** class and then the "modifier class" like **outline-purple-300**.
- If we need to add shadow to an element, first we need to add the "base" **shadow** class followed by a size like **shadow-lg** (lg = large).
