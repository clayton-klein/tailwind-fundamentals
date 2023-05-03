# General course's notes:

## Documentation:

https://tailwindcss.com/docs/installation

## General:

- Here we're just importing Tailwind via CDN in our HTML files to keep things simple, but there are better ways to use this framework (specially for big projects) and we'll see them later in the course (probably the examples will be in other repos).

- With Tailwind we don't need to write "pure CSS" files and worry about them getting too big, we don't need to worry about classes names and it's easier/faster to test things out by just changing the utility classes inside the `class=""` attribute of the HTML elements to see the results.

- There are some specific comments in each **index.html** file as well.

- There are some utility classes that need a "base" class to be added first before being able to be used, otherwise they don't work. For example, we must add `border` before defining a color for the border with `border-red-300`.

## Colors:

- The colors **black** and **white** don't have **shades**, but when we're using other colors we **must** specify a shade (from 50 to 950 and excluding the beggining and the end we must "step" by 100), otherwise it'll show as black (e.g. `text-red-500`).
  - If we need to **customize our palette**, we can configure our colors under the **colors key** in the **theme section** of your **tailwind.config.js** file, see the documentatio for more info.
- If we need to add color to a **border**, first we need to add the "base" `border` class and then the "modifier class" like `border-red-500`.
- If we need to add color to a **"divider"** (to divide items with a line), first we need to add the "base" `divide-y` (vertically in this case) class and then the "modifier class" like `divide-blue-300` (the default is black).
- If we need to add color to an **outline**, first we need to add the "base" `outline` class and then the "modifier class" like `outline-purple-300`.
- If we need to add **shadow** to an element, first we need to add the "base" `shadow` class followed by a size like `shadow-lg` (lg = large).

## Spacing:

- When we add the `container` class to an element, we're automatically making it responsive with 5 breakpoints by default (max-width: 640, 768, 1024, 1280, 1536px).

- By default the **numbers** we use for spacing are **rem** based and number **1 = 0.25rem = 4px**, so the utility class `mt-4` (margin top 4) for example, is equal to **1rem**. If we want just **1px** we declare it like `mb-px` (margin bottom = 1px),the numbers **start at 0 and go untill 96** = 24rem = 384px (0.5 step based). It's possible to change the values though if we create a config file.

- We can also use arbitrary
