# mailchimp-boilerplate

This email blueprint is adapated from [MailChimp](https://github.com/mailchimp/email-blueprints) and licensed under a [Creative Commons Attribution-ShareAlike 3.0 Unported License](http://creativecommons.org/licenses/by-sa/3.0/).

It is used as a starting point for MailChimp templates at [spatie.be](https://spatie.be).

## Usage

- Download as .zip to modify.
- Make a .zip with all assets to upload to Mailchimp

### Outlook 2013

- Caution with importing custom webfonts in Outlook 2013: they tend to break the font stack. Include conditional styles with `!important` to avoid Times New Roman / serif body text.

```html
    <!--[if mso 15]>
    <style type="text/css">
        h1, h2, h3, h4, h5, h6,
        .headerCell, .footerCell,
        .textContent, .textContentLast,
        .buttonContent,
        .emailCalendarDay, .emailCalendarMonth {
            font-family: Arial, sans-serif !important;
            mso-line-height-rule: exactly;
        }
    </style>
    <![endif]-->
```

- Use images with the exact size. Outlook 2013 doesn't handle the `max-width` styles, larger images break the layout.
- Use line-heights in %, eg. `line-height: 150%`


## Changes

- Colors and styling
- Font-family definition bundled
- Google Fonts example
- Default Facebook and Twitter icons
- Header/footer merge tags
- Mc:tags for editable fields/images and repeatable blocks