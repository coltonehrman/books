# Chapter 4: Let's Get Lost Real Quick

Ok... so, after a *little* bit of thought on how to start this Chapter and continue on from [Chapter 3](/html//chapters//3/README.md), I have decided to take a detour.

It is time to take a step back and understand the Web outside of just HTML and how to Web works.

## Why?

So, HTML alone is ok, but, it's not very *cool* to be honest. You can't really do much with it. We can continue exploring more tags and ways to structure a page, but none of that is useful without the other pieces that actually bring everything to **LIFE!**

What do I mean by "bring to life"? Well, the `<a>` tag for example, it's meant to link from one Web page to another, BUT, the problem is, up to now, we have been working with HTML locally and through a single file which we copy/pasted into the Browser. That will only get us so far...

In order to unlock the full potential we need to understand some more pieces of the Web and slowly start putting things together.

## HTTP

I introduce you to **HTTP!** Also know as, **HyperText Transfer Protocol**. Which may sound very similar to **HyperText Markup Language** (aka **HTML**). That's because it was made for "transferring" **HTML** from a server to a client.

*Bare with me, I'm sure you may be looking at me funny right now, wondering why I am bringing this up. Everything will start to make sense.*

Now, I think we already sort of talked about server & client previously. We should know that a **Browser** is a **client** by now. Now, what exactly is a server?

A server is just another computer/software that "serves" the client (aka the Browser). How does it serve exactly? Well, the Browser is very complex and does a lot of things for you behind the scene when browsing the wonderful World Wide Web.

Let's look at some other pieces of the puzzle.

### Domain Name & DNS

A domain name is a human friendly name of a Web site, such as `google.com` or `www.google.com`. *Technically, the domain here is just `google.com` and `www.google.com` is a called a sub-domain. But we'll talk about that later.*

Now, when you type in a domain name into your browser a *BUNCH* of things happen behind the scenes, like **MAGIC!**

The first thing that happens is the browser will do a **DNS lookup** on the domain name to find the **IP Address** associated with it *(this is a simplistic representation)*.

#### IP Address

An IP Address is like an address for a computer on the internet. It looks something like this `192.168.0.1` *(this is what is called a local IP address)*.

*Now, back to the DNS...*

When the browser knows the IP Address of the domain you want to navigate to, it can then establish a connection with it. This is what we mean when we say *client-server*. You can actually visualize this connection like this `client<->server`, where the client can talk to the server and the server can talk back to the client. *The client always starts the communication process.*

Once the Browser has established a connection to the server's IP address, it can start communication. For the Web the type of communication "protocol" it uses is called **HTTP**.

### Summary

Here is a summary of the steps we talked about.

1. You type in `google.com` in your browser.
1. Your browser does a **DNS lookup** to find the **IP Address** of `google.com`.
   - The IP Address comes back as `192.168.0.1` *(this is not the correct IP, but just to demonstrate the steps)*
1. Your browser establishes a connection to `192.168.0.1`.
1. Your browser will begin communication with `192.168.0.1` (aka the **server** aka **google.com**) using **HTTP**.

*Now, back to HTTP...*

In a normal scenario, the browser will always start of communication with the server by sending an **HTTP** message that looks something like this.

```
GET /index.html HTTP
Host: google.com
```

This message is saying **GET** me the **index.html** page of **google.com**.

This message is formatted and structured a specific way to follow the **HTTP** protocol, which is a **specification** on "how" you communicate between a client & server.

The **GET** *verb* is the most common HTTP action used by browsers, and just as it sounds, is meant to *get* something from the server. In this case, we want to get the **index.html** page of the server. *__index__ is a commonly known name for the "default" or "root" of something. So, **index.html** is the "root" of **google.com**. You can also visualize this as **google.com/index.html**, which shows the domain and the **path** of the domain.*

