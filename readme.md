### Go to the [HTML Preview Source Repo](https://github.com/htmlpreview/htmlpreview.github.com)

# Original Source - GitHub & BitBucket HTML Preview
Many GitHub repositories don't use GitHub Pages to host their HTML files. **GitHub & BitBucket HTML Preview** allows you to render those files without cloning or downloading whole repositories. It is a client-side solution using a CORS proxy to fetch assets.

If you try to open raw version of any HTML, CSS or JS file in a web browser directly from GitHub, all you will see is a source code. GitHub forces them to use the "text/plain" content-type, so they cannot be interpreted. This script overrides it by using a CORS proxy.

## Usage

In order to use it, just prepend the below fragment to the URL of any HTML file. Copy and paste below: 
```markdown
https://nobedee.github.io/htmlpreview.github.com/?
```
## For Example
 - https://nobedee.github.io/htmlpreview.github.com/?https://github.com/twbs/bootstrap/gh-pages/2.3.2/index.html
 - https://nobedee.github.io/htmlpreview.github.com/?https://github.com/documentcloud/backbone/blob/master/examples/todos/index.html

What it does is: load HTML using CORS proxy, then process all links, frames, scripts and styles, and load each of them using CORS proxy, so they can be evaluated by the browser.

**GitHub & BitBucket HTML Preview** was tested under the latest Google Chrome and Mozilla Firefox.

## License

&copy; 2019 Jerzy Głowacki under Apache License 2.0.
