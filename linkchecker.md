Linkchecker surrounds broken link with images.

This looks like this:

```html
<li>
  <img src="/libs/cq/linkchecker/resources/linkcheck_o.gif" alt="invalid link: /content/site/home/es.html/cat=cat1" title="invalid link:/content/site/home/es.html/cat=cat1" border="0">
  cat1
  <img src="/libs/cq/linkchecker/resources/linkcheck_c.gif" border="0">
</li>
```

This can cause huge images if some CSS targets `<img>` and tells them to be `max-width:100%;`

The following CSS targets these image

```css
img[src^="/libs/cq/linkchecker/resources/linkcheck_"] {
    width: auto;
}
```
