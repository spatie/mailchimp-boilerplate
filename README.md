
## Mailchimp boilerplate with repeatable modules

This MailChimp HTML email boilerplate contains useful repeatable modules with `mc:repeatable` and `mc:edit` attributes. 

Imported as a MailChimp Template it gives authors the opportunity to create, duplicate and rearrange different sections in a newsletter. 

Check this [sized screenshot](src/preview.png) with all modules.

Modules included:

- 1 column text
- 2 columns text
- Action button
- Banner + optional caption
- 2 columns thumbnails + text
- Image + text column (right or left aligned)
- All the above with inset & background
- Calendar + text (right or left aligned)

The boilerplate is used as a starting point for MailChimp templates at [spatie.be](https://spatie.be).

## Postcardware

You're free to use this package (it's [Creative Commons Licensed](LICENSE.md)), but if it makes it to your production environment we highly appreciate you sending us a postcard from your hometown, mentioning which of our package(s) you are using.

Our address is: Spatie, Samberstraat 69D, 2060 Antwerp, Belgium.

The best postcards will get published on the open source page on our website.


## Usage

### Customize

- Download or clone this repository
- Adapt and tweak the HTML and embedded CSS in `email.html`

### Upload to MailChimp

- Make a .zip file containing `email.html` and all `*.png` files
- Go to MailChimp's _Templates_ section 
- Select _Create template_ > _Code your own_ > _Import zip_
- Upload the .zip and name your template

When creating new Campaigns in MailChimp, you now can select this layout in the _Template_ step, tab _Saved templates_.

### Caveats

- Use images with the exact size. Outlook 2013 doesn't handle the `max-width` styles, larger images break the layout.
- Use line-heights in %, eg. `line-height: 150%`
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


## Changelog

Please see [CHANGELOG](CHANGELOG.md) for more information what has changed recently.

## Testing

Test with MailChimp's Preview and Inbox Preview functionality. Send test mails to real world mailboxes.

## Contributing

Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Credits

- [Willem Van Bockstal](https://github.com/willemvb)
- [All Contributors](../../contributors)

## About Spatie
Spatie is a webdesign agency based in Antwerp, Belgium. You'll find an overview of all our open source projects [on our website](https://spatie.be/opensource).

## License

Creative Commons License. Please see [License File](LICENSE.md) for more information.