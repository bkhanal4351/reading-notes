# NextJs

# Assets, Metadata, and CSS

Assets
- Next.js can serve static assets, like images, under the top-level public directory. Files inside public can be referenced from the root of the application similar to pages.

The public directory is also useful for robots.txt, Google Site Verification, and any other static assets. Check out the documentation for Static File Serving to learn more.

Metadata
  - To modify metadata, such as 'title' HTML tag:

  Open pages/index.js in your editor and find the following lines:

  ```
  <Head>
  <title>Create Next App</title>
  <link rel="icon" href="/favicon.ico" />
  </Head>

  ```

  Notice that Head is used instead of the lowercase head. Head is a React Component that is built into Next.js. It allows you to modify the head of a page.

You can import the Head component from the next/head module.

```
import Head from 'next/head';
```

CSS
  - Next.js has built-in support for CSS and Sass which allows you to import .css and .scss files.

Using popular CSS libraries like Tailwind CSS is also supported.

Notes taken from (https://nextjs.org/learn/basics/create-nextjs-app)
