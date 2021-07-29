# Forms

### Intro to Forms

Forms enable users to perform actions like searching, signing up for membership on sites, adding items to the cart on shopping platforms, and a myriad of other things. The most recognizable example of a form is probably google's search box.

#### Form Structure

Forms are typically structured like this:

```html
<form action="https://www.example.com/login.php">
  <p>Username:
    <input type="text" name="username" maxlength="30" />
  </p>
</form>
```

Form controsl live inside the `<form>` element. This element should always have the `action` attribute and will typically have a `method` and `id` attribute too. The `action` attribute signals where the info in the form should be sent to when submitted. The `method` attribute can either be `get` or `post`. The `get` method is ideal for short forms (like search boxes) and times where retrieving info from a web server is all that's needed. The `post` method is useful for forms that allow users to upload a file, contain senstive data, and add to or delete info from a database. The `input` element is used for creating the form controls. The type of form that's used is determined by the `type` attribute. In the codeblock above, `type="text"` creates a single-line text input. The `name` attribute allows the server to know which form control each piece of data was entered into. Lastly, the `maxlength` attribute can be used to limit the amount of characters a user may enter into the text field.

