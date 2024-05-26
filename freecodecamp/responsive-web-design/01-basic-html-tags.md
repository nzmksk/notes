# Basic HTML Tags
| Tag | Attribute | Function |
| -- | -- | -- |
| html |  | All elements must be nested inside `<html>` tag. |
|  | lang | Specify the language of the page. <br />`en` set the language to English. |
| head |  | Webpage metadata and other important information must be nested inside the `<head>` tag. |
| title |  | Set the ***title*** of the browser tab. |
| meta |  | Set the browser behaviour. |
|  | charset | `UTF-8` tells the browser to parse the markup into multiple languages. |
|  | name | Specify a name for the metadata. |
|  | content | Specify the value associated with the `http-equiv` or name attribute. |
| style |  | Used to define ***style*** information for a document |
| link | rel | Define the ***relationship*** between the current document and an external resource. |
|  | href | Specify the location of the linked document. |
| body |  | All **page content** elements that should be rendered to the webpage must be nested inside `<body>` tag. |
| h1-h6 |  | ***Heading*** elements used to signify the importance of content below them. The lower the number, the higher the importance. <br />Use **only one `<h1>` per page**. |
| p |  | Used to create a ***paragraph*** of text on websites. |
| em |  | Used to ***emphasize*** text. |
| strong |  | Used to indicate that some text is of ***strong*** importance or urgent. |
| main |  | Semantic tag that **helps with Search Engine Optimization (SEO) and accessibility**. <br />Used for ***main*** section/content of the webpage. |
| section |  | Used to represent a group of related content as a ***section***. |
| footer |  | Used to define a ***footer*** section. |
| figure |  | Used to represent self-contained content that allows images to be associated with a caption. |
| figcaption |  | Used to add a caption to describe the `<img>` contained within the `<figure>` element. |
| img |  | Used to embed ***images*** in HTML document. |
|  | src | ***Source*** of the image. |
|  | alt | ***Alternate*** text of the image used for screen readers to **improve accessibility** and is displayed if the image fails to load. |
| form |  | A web ***form*** to collect information from users. |
|  | action | Indicate where `<form>` data should be sent. |
| fieldset |  | Used to group related `<input>` and `<label>` together in a `<form>`. |
| legend |  | Act as a caption for the content in the `<fieldset>` element. <br />Give users context about what they should enter into that part of the form. |
| label |  | Used to help associate the text ***label*** for an `<input>` element, **especially for assistive technologies like screen readers**.  |
|  | for | Associate the wrapped text with the `<input>` field of the same *`name`*. |
| input |  | Allow web `<form>` to collect data from user ***input***. |
| button |  | Create a clickable ***button***. <br />The default behaviour of clicking a form button without any attributes **submits the form to the location specified in the `<form action>`** |
| a | href | An ***anchor*** used to link text or content to another page or section. |
|  | target | Target `_blank` will open the link in a new tab. |
| ul |  | ***Unordered list*** (bullet list). Require `<li>` as children. |
| ol |  | ***Ordered list*** (numbered list). Require `<li>` as children. |
| li |  | Used in unordered and ordered lists as ***list items***. |

## Example HTML Skeleton
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Hello World</title>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="css-filename.css" />
    <style>
      /** For internal CSS styling
      h1 {
        text-align: center;
      }
      */
    </style>
  </head>
  <body>
    <nav>
      <a target="_blank" href="www.google.com">
        This link opens in new tab.
      </a>
      <a href="#main-content">
        This link redirects to the main content in the same document.
      </a>
      </nav>
    <main id="main-content">
      <h1>Use only <strong>one</strong> h1 tag in a single document.</h1>
      <section>
        <h2>Lists</h2>
        <h3>Unordered lists:</h3>
        <ul>
          <li>Item 1</li>
          <li>Item 2</li>
          <li>Item 3</li>
        </ul>
        <h3>Ordered lists:</h3>
        <ol>
          <li>Item 1</li>
          <li>Item 2</li>
          <li>Item 3</li>
        </ol>
        <figure>
          <img src="www.google.com" alt="Alternate text for accessibility." />
          <figcaption>This is a caption for the above image.</figcaption>
        </figure>
      </section>
      <section>
        <form action="www.google.com/submit-data">
          <fieldset>
            <legend>This acts as a caption for the content in <i>fieldset</i> element.</legend>
            <label>
              <input
                id="input-checkbox"
                type="checkbox"
                name="input1"
                value="yes"
                checked
              />This is the label for the input.
            </label>
            <label for="input-text">You can also label the input using <i>label for</i>.</label>
            <input
              id="input-text"
              type="text"
              name="input2"
            />
          </fieldset>
          <fieldset>
          </fieldset>        
          <button></button>
        </form>
      </section>
      <div>
        <p><i>div</i> container is less preferred as it's not semantic.</p>
      </div>
    </main>
    <footer></footer>
    <script></script>
  </body>
</html>
```

## General Attributes
- `id` attribute is used to identify specific HTML elements.
- Each `id` attribute's value **must be unique** from all other `id` values for the entire page

### Input Tag
| Attribute | Function |
| -- | -- |
| type="text" | Single-line text input field. |
| type="search" | A search field that behaves like a regular text field. |
| type="numeric" | Numeric input field. |
| type="tel" | Input that validates a telephone number. |
| type="password" | Defines a password field. | 
| type="email" | Input field that validate inputs as email addresses. |
| type="url" | Input field that validate inputs as web addresses. |
| type="range" | Slider input. |
| type="hidden" | Lets developers include data that cannot be seen or modified by users when a form is submitted. |
| type="radio" | Let a user to select **ONLY ONE** of a limited number of choices. |
| type="checkbox" | Let a user select **ZERO** or **MORE** options of a limited number of choices. |
| type="file" | Allow file uploads. |
| type="date" | Date picker input. |
| type="time" | Allows user to select a time (without time zone). |
| type="datetime-local" | Date and time input field with no time zone. |
| type="month" | Allow user to pick month and year. |
| type="week" | Allow user to pick week and year. |
| type="color" | Color picker input. |
| type="image" | Defines an image as a submit button. Sends the X and Y coordinates of the click that activated the image button. |
| type="submit" | Defines a button for submitting form data to a form-handler specified in the `<form action>`.
| type="button" | Defines a button. |
| type="reset" | Defines a reset button that will reset all form values to their default values. |
| name | The ***name*** of the input field which can be accessed later in the location specified in `<form action>`. |
| value | Specify the value for the input field with *`name`* which can be accessed later in the location specified in `<form action>`. |
| placeholder | Used to give user a hint about what kind of information to enter into an input. |
| required | Make an input field ***required*** to be filled by the user. |
| checked | Make a `radio` or `checkbox` button selected by default. |

### Button Tag
| Attribute | Function |
| -- | -- |
| type | Specify a button ***type***. <br />`submit` - submits form data. <br />`button` - clickable button. <br />`reset` - resets the form data to its inital values. |
