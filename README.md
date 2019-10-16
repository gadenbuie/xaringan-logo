## Add a logo to all your xaringan slides

You can use this repository as a template to create your xaringan project, or follow the instructions below.

[Demo](https://gadenbuie.github.io/xaringan-logo)

## Manual Set Up

1. Download your logo. I've used the `xaringan` hex logo: [`xaringan.png`](https://github.com/rstudio/hex-stickers/blob/master/PNG/xaringan.png)

1. Download [`insert-logo.html`](https://github.com/gadenbuie/xaringan-logo/blob/master/insert-logo.html)

1. Add `insert-logo.html` to your `after_body` includes

  ```yaml
  output:
  xaringan::moon_reader:
    includes:
      after_body: insert-logo.html
  ```

1. Edit the `.logo` class in the CSS in `insert-logo.html` to use your logo,
   and adjust the `width`, `height` and position (`top`, `bottom`, `left`, and/or `right`) as needed<sup>*</sup>.

1. Use `class: hide-logo` to hide your logo on individual slides.
