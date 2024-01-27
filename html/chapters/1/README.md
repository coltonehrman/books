# Chapter 1: Core Concepts & Terminology

Welcome to the first step of your web development journey! This chapter is all about laying a solid foundation. We'll demystify the jargon and introduce the essential concepts of HTML and web development. Whether you're an absolute beginner or brushing up on basics, this chapter will align our understanding and prepare you for the exciting journey ahead.

## What is Web Development?

Web development is the art and science of building websites and web applications. It encompasses everything from creating simple static web pages to complex, interactive web applications. There are three main layers to web development:

- **Frontend (Client-Side):** This is what you see and interact with on a website. It's all about the user experience, involving HTML for structure, CSS for styling, and JavaScript for functionality.
- **Backend (Server-Side):** This involves the server, database, and applications that work behind the scenes. It's where the data processing happens, and it supports the frontend.
- **Full Stack:** A combination of both frontend and backend development. Full-stack developers can handle all aspects of web development.

In this book, we will only be discussing HTML, which perhaps to your surprise, can fall into the category of Full Stack. But, for the purpose of the book, we will mainly focus on HTML on the client only.

For the time being let's just focus on this one concept. **HTML is used by the Web Browser**.

### Now, what exactly does that mean?

To put it simply, you will write HTML "code" as text, aka, not binary or some weird format, just think of it as plain text, that follows specific grammar and rules.

Once you have written your HTML code, you can save it to a file using a special extension `.html`. This tell the web browser that the text is HTML based and it will begin "parsing" (aka reading) the text and do it's magic.

Now, to fully demonstrate this in a simplistic way, we will do an exercise.

### Exercise

Create a new file, with the `.html` extension (ie: `my-page.html`) and open it in a text editor, such as **Notepad**, or whatever you use to right plain text. The editor should **not** write text in a rich format, like **Word**.

Now, let's copy/paste this HTML into the new file.

```html
<!DOCTYPE html>
<html>
  <body>
    <h1>Hello World!</h1>
  </body>
</html>
```

Now, save the file and copy the file location of the newly saved `.html` file. If you are on a Windows computer, it may look something like this `file:///C:/Users/bob/Desktop/my-page.html`.

Now, here is where the **magic** happens. Open up a Web Browser, such as **Google Chrome**, **Firefox**, or **Safari**, and paste the full file location into your URL bar at the top.

If done correctly, you will see something like this.

![My First HTML Page](./first-html-page.png)

Notice how the only thing you see is the text **Hello World!** and none of the other code was shown to you. This is how HTML works, the browser took your code and created representation of it for you to view.

Now, you may be asking, what everything means or does inside the code we just wrote. We will get into that in the upcoming chapters, for now, let's celebrate our 1st step into the magical journey of the web.

#### Exercise Problems?

If you experience any issues with the excerise, please ensure the following conditions are met:

1. You copy/pasted the correct code into the file.
1. You saved the file with the correct extension `.html`.
   - Make sure the file was not saved with any hidden extensions added to it.
1. You copied the correct _full_ location of the file.

Another issue that _may_ come up is your browser or computer are not correctly determining the file is on your computer and instead trying to browser the internet or search on a search engine for that file. If that is the case, your setup may have some issues. You can attempt to google solutions, or just continue following along for now.

## Understanding HTML

At its core, HTML is the language that web browsers understand to display web pages. Here's how it works:

- **Tags and Elements:** HTML uses tags to markup text, images, and other content to display it on the web page. For example, `<p>` is a tag for paragraph text.
- **Attributes:** Tags can have attributes that provide additional information about an element, such as `<img src="image.jpg" alt="description">`, where src and alt are attributes of the img tag.
- **Structure:** An HTML document has a defined structure, including a doctype declaration, and `<html>`, `<head>`, and `<body>` sections.

## The Evolution of HTML

HTML has evolved significantly since its inception. The latest version, HTML5, introduced new elements, attributes, and behaviors with a greater emphasis on multimedia, graphical content, and improved accessibility for users and compatibility across devices.
