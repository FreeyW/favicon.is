<div align="center">
  <img src="https://favicon.is/favicon.is" width="64" height="64" alt="Favicon.is logo">
  <h1>Favicon.is</h1>
  <p>A user-friendly API to get favicons quickly and easily from any website.</p>
  <hr>
</div>

## Example

Get the favicon of a domain:

https://favicon.is

- https://favicon.is/google.com

Result: ![https://favicon.is/google.com](https://favicon.is/google.com)

Image resizing is available using the **?s=:size** parameter (max is 256):

- https://favicon.is/google.com?larger=true

Result: ![https://favicon.is/google.com](https://favicon.is/google.com) ![https://favicon.is/google.com?larger=true](https://favicon.is/google.com?larger=true)


## About

Favicone is a super convenient API service that allows you to easily retrieve and serve favicons from any website. With its user-friendly URL structure, Favicone makes the process a piece of cake – just use something like `https://favicon.is/{domain}`.

The magic happens behind the scenes as Favicone cleverly searches for the favicon link within the website's HTML or directly from the favicon.ico file. It's all about efficiency and simplicity!

You can use Favicone in your app or website to enhance the visual appeal of your app and ensure your users enjoy a seamless favicon experience.

## The Problems

Obtaining a favicon from a website can be a challenging task due to the inconsistent locations where the favicon.ico file or favicon references may be found. The following are common sources where a favicon can be located:

1. favicon.ico file: Traditionally, websites have placed the favicon.ico file at the root directory of the website. However, this is not always the case, and the favicon.ico file may be located in different directories or have a different file name.

2. HTML code: Websites often define a favicon link in their HTML code using the `<link>` tag with the `rel="icon"` attribute. The `href` attribute specifies the URL of the favicon. However, the favicon link can have different variations, such as `rel="shortcut icon"`, `rel="apple-touch-icon"`, or other custom variations.

### What is Favicon.is?

Favicon.is is a simple and efficient service that enables you to fetch the favicon (website icon) of any website. Simply provide a domain name, and we'll return the corresponding favicon. It's ideal for developers, designers, or anyone who needs quick access to website icons.

### How does Favicon.is work?

Favicon.is employs a multi-step process to retrieve a website's favicon:
It scans the HTML of the specified website for favicon declarations in the <head> section.
If a favicon is declared in the HTML, Favicon.is retrieves it from the specified location.
If no favicon is found in the HTML, Favicon.is attempts to fetch the favicon from the root directory as 'favicon.ico' (e.g., https://example.com/favicon.ico).
If neither method yields a favicon, a default or placeholder image is returned.
This approach ensures that Favicon.is can retrieve icons from most websites, even those that do not explicitly declare a favicon in their HTML.

### What if a website doesn't have a favicon?

If a website lacks a favicon, Favicon.is will return a default or placeholder image. This guarantees that your application will always receive an image, even if the target site does not have a favicon.

### Can I use Favicon.is in my application?

Absolutely! Favicon.is is designed for easy integration into various applications. You can utilize it to display favicons for links, enhance user interfaces, or in any situation where you need to programmatically fetch website icons.

### Is there a rate limit for using Favicon.is?

While we aim to provide a reliable service, we do implement rate limiting to ensure fair usage. For specific information regarding rate limits or if you require high-volume access, please contact us directly.

These variations in favicon locations and references make it challenging to reliably fetch the favicon for a given website. Favicone aims to address these challenges by searching for the favicon in multiple sources, including the favicon.ico file, HTML code, and web manifest files.
