
# Mailchimp boilerplate with repeatable blocks

This MailChimp HTML email boilerplate contains useful repeatable blocks with `mc:repeatable` and `mc:edit` attributes. 

Imported as a MailChimp Template it gives authors the opportunity to create, duplicate and rearrange different sections in a newsletter. 

Check this [sized screenshot](src/preview.png) with all available blocks.

Included:

- 1 column text
- 2 columns text
- Action button
- Banner + optional caption
- 2 columns thumbnails + text
- Image + text column (right or left aligned)
- All the above with inset & background
- Calendar + text (right or left aligned)

The boilerplate is used as a starting point for MailChimp templates at [spatie.be](https://spatie.be).

## Support us

[![Image](https://github-ads.s3.eu-central-1.amazonaws.com/mailchimp-boilerplate.jpg)](https://spatie.be/github-ad-click/mailchimp-boilerplate)

We invest a lot of resources into creating [best in class open source packages](https://spatie.be/open-source). You can support us by [buying one of our paid products](https://spatie.be/open-source/support-us).

We highly appreciate you sending us a postcard from your hometown, mentioning which of our package(s) you are using. You'll find our address on [our contact page](https://spatie.be/about-us). We publish all received postcards on [our virtual postcard wall](https://spatie.be/open-source/postcards).

## Postcardware

You're free to use this package (it's [Creative Commons Licensed](LICENSE.md)), but if it makes it to your production environment we highly appreciate you sending us a postcard from your hometown, mentioning which of our package(s) you are using.

Our address is: Spatie, Kruikstraat 22, 2018 Antwerp, Belgium.

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

### Compose campaigns

When creating new Campaigns in MailChimp select this layout in the _Template_ step, tab _Saved templates_.

Compose your email in the _Edit_ step:
- Hover a content section and duplicate blocks with the *+* at the bottom left
- Change a block type in the dropdown
- Drag blocks to reorder

More info in this [MailChimp KB article](http://kb.mailchimp.com/templates/basic-and-themes/repeatable-or-variable-content-blocks)

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
