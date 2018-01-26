# Blog4Git

#### A statically hosted blogging engine for GitHub Pages.

Blog4Git is a statically hosted blogging engine. Statically hosted means that Blog4Git requires no
server side handling and summoning unnecessary dramatic encounters to fetch some mere words from a database and show it to the public.

Blog4Git delivers your content from right where you saved it. It's that simple. Deal with it!

## How Blog4Git works

Blog4Git utilizes a _lightweight markup language_ which the wanderers of the Internet often
refer to as **Markdown** (and your writing skills too) and all the content is managed by a `blogs.json` file that has complete information about the articles that you have written.

## How to use Blog4Git

It's really easy to use. Publishing blogs with Blog4Git is done in four easy steps.

1. Fork/Download this repository.
2. Write your blog.
3. Register it in the `blogs.json` file.
4. Show off.

### Writing your blog

Blog4Git requires you to write your content in [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) format and save it under the `blogs/` folder.

### Registering your blog in the `blog.json` file

Honestly speaking, this file is the heart of of everything and it lives with all your blogs, under the `blogs/` folder. Let's suppose you wrote something about Internet Doggos and saved it as `doggos.md` in the `posts/` folder, then you would register your blog in the `blog.json` file like this.

```json
{
  "all" : [
    {
      "title": "Internet Doggos: A really fancy title that makes no sense",
      "md": "doggos",
      "create": "January 26, 2018 01:05:00",
      "featured": true
    }
  ]
}
```

##### A quick explanation:

* `"title"`: The title that would be shown on the home page under **All Blogs** and **Featured Blogs** section.
* `"md"`: The name of the file in which your blog is (without extension).
* `"create"`: The time when you wrote your blog.
* `"featured"`: Whether blog will appear under the **Featured Blogs** section or not.

So now you know how to write and register a blog and you have written an another one about Garlic Breads, but you don't want it to be featured, then your newly updated `blogs.json` file will look like this:

```json
{
  "all" : [
    {
      "title": "Garlic Breads: Because I hate Banana Breads",
      "md": "gbreads",
      "create": "January 26, 2018 02:10:00",
      "featured": false
    },
    {
      "title": "Internet Doggos: A really fancy title that makes no sense",
      "md": "doggos",
      "create": "January 26, 2018 01:05:00",
      "featured": true
    }
  ]
}
```

And it's done.

**P.S:** The comma is required only when there are multiple blog entries. Put one needlessly and
you'll break your own website.

---

That's pretty much it. If you like, you can head over to the [in-depth instructions](https://jgodara.github.io/blog4git/blogs/#getting-started) on how to leverage everything out of Blog4Git, or customizing it. Or look at [the one that I already use on my website](https://jgodara.github.io/blogs)!
