## HTML Quotation and Citation Elements
- [Quotations](#blockquote-for-quotations)
- [Short Quotations](#q-for-short-quotations)
- [Abbreviations](#abbr-for-abbreviations)
- [Contact Information / Address](#address-for-contact-information)
- [Citations](#cite-for-work-title)
- [Bi-Directional Override](#bdo-for-bi-directional-override)

### `<blockquote>` for Quotations<hr />
- Defines a section that is quoted from another source.
- Usually indented by browsers.

Example:
```html
<p>Here is a quote from WWF's website:</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 60 years, WWF has worked to help people and nature thrive. As the world's leading conservation organization, WWF works in nearly 100 countries. At every level, we collaborate with people around the world to develop and deliver innovative solutions that protect communities, wildlife, and the places in which they live.
</blockquote>
```
<p>Here is a quote from WWF's website:</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 60 years, WWF has worked to help people and nature thrive. As the world's leading conservation organization, WWF works in nearly 100 countries. At every level, we collaborate with people around the world to develop and deliver innovative solutions that protect communities, wildlife, and the places in which they live.
</blockquote>

### `<q>` for Short Quotations<hr />
- Defines a short inline quotation.
- Browsers normally insert quotation marks `"` around the quotation.

Example:
```html
<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>
```
<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>

### `<abbr>` for Abbreviations<hr />
- Defines an abbreviation or an acronym like "HTML", "CSS", "ASAP", "ATM", etc.
- Provide useful information to browsers, translation systems, and search engines.
- Use the `title` attribute to show the description for the abbreviation when the element is moused over.

Example:
```html
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>
```
<p>The <abbr title="World Health Organization">WHO</abbr> was founded in 1948.</p>

### `<address>` for Contact Information<hr />
- Defines the contact information for the author/owner of a document or an article.
- Contact information can be an email addrress, URL, physical address, phone number, social media handle, etc.
- Usually renders in *italic* and browsers will add a line break before and after the `<address>` element

Example:
```html
<address>
Written by John Doe.<br />
Visit us at:<br />
Example.com<br />
Box 564, Disneyland<br />
USA
</address>
```
<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>

### `<cite>` for Work Title<hr />
- Defines the title of a creative work (e.g. book, poem, song, movie, painting, sculpture, etc.).
- Usually renders in *italic*.

Example:
```html
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>

### `<bdo>` for Bi-Directional Override<hr />
- Used to override the current text direction.

Example:
```html
<bdo dir="rtl">This text will be written from right to left.</bdo>
```
<bdo dir="rtl">This text will be written from right to left.</bdo>

<br />
<hr />

| Previous | Home | Next |
| :---: | :---: | :---: |
| [Formattings](04-formattings.md) | [HTML Introduction](01-introduction.md) | [CSS](06-css.md) |