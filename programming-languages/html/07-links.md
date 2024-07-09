## HTML Links
- HTML links are hyperlinks - an area on a web page that, when clicked on with a mouse, will transport the user to another web page.

### Default Behaviour
| State | Default Behaviour |
| --- | --- |
| Hovering mouse on a link | Mouse arrow turns into a little hand. |
| Unvisited link | Underlined and blue in colour. |
| Visited link | Underlined and purple in colour. |
| Active link | Underlined and red in colour. |

### Syntax
```html
<a href="www.google.com">Search on Google</a>
```
<a href="www.google.com">Search on Google</a>

### Attributes
<table>
  <tr>
    <th>Attribute</th>
    <th>Value</th>
    <th>Description</th>
  </tr>
  <tr>
    <td rowspan=4>href</td>
    <td>Absolute URL</td>
    <td>Full web address. Example: <code>https://www.google.com</code></td>
  </tr>
  <tr>
    <td>Relative URL</td>
    <td>A link to a page within the same website. Example: <code>/maps</code> in Google website will point to <code>https://www.google.com/maps</code></td>
  </tr>
  <tr>
    <td>Email</td>
    <td>Open the user's email program to let them send a new email. Example: <code>mailto:john_doe@email.com</code></td>
  </tr>
  <tr>
    <td>Web section</td>
    <td>A link to an ID within the same page or another page using the tag's ID as reference. Example: <code>#html_id</code> or <code>https://www.example.com#html_id</code></td>
  </tr>
  <tr>
    <td rowspan=4>target</td>
    <td><code>_self</code></td>
    <td>Default - Opens the document in the same window/tab as it was clicked</td>
  </tr>
  <tr>
    <td><code>_blank</code></td>
    <td>Opens the document in a new window or tab</td>
  </tr>
  <tr>
    <td><code>_parent</code></td>
    <td>Opens the document in the parent frame</td>
  </tr>
  <tr>
    <td><code>_top</code></td>
    <td>Opens the document in the full body of the window</td>
  </tr>
  <tr>
    <td>title</td>
    <td></td>
    <td>Displayed as a tooltip text when the mouse moves over the element.</td>
  </tr>
</table>


### Notes
- A link does not have to be text. It can also be an image or any other HTML element.

<br />
<hr />

| Previous | Home | Next |
| :---: | :---: | :---: |
| [CSS](./06-css.md) | [HTML Introduction](./01-introduction.md) |  |