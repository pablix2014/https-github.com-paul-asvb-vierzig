# Vierzig Theme Demo

A Demo Page for [Vierzig Theme](https://github.com/ASVBPREAUBV/vierzig) (a [Hugo](https://gohugo.io/) Theme)

[Demo](https://vierzig-theme-demo.netlify.com/) for the page

[Demo](https://vierzig-theme-demo.netlify.com/admin) for the Admin Interface


## Installation

Create a new Hugo Site and inside the site folder run the following commands:

    $ cd themes
    $ git clone https://github.com/ASVBPREAUBV/vierzig

To learn how to create a Hugo Site read the [official guide](//gohugo.io/overview/installing/) of Hugo.

### Netlify

If you are using Netlify to host your hugo site, you will want to add it as a submodule instead of cloning:

    $ cd themes
    $ git submodule add https://github.com/ASVBPREAUBV/vierzig

This is because Netlify uses the hugo build command when autopublish is enabled and will produce an error if the theme is not a submodule. See the [Hugo Guide](https://gohugo.io/hosting-and-deployment/hosting-on-netlify/#use-hugo-themes-with-netlify) for more information.

If your javascript or css isn't rendering, check your BaseURL frontmatter in the `config.toml` file. This needs to be set to match the URL you are publishing to. i.e. if you are publishing to https://www.yourdomain.com your frontmatter should be `BaseURL = https://www.yourdomain.com`

## Using the theme

After cloning Forty or adding it as a submodule, there are a few other things you should do:

### Config File

There is an [`exampleSite`](//github.com/MarcusVirg/forty/tree/master/exampleSite) folder for this theme. Copy the file called [`config.toml`](//github.com/MarcusVirg/forty/blob/master/exampleSite/config.toml) to your websites root directory.
Here you can customize some of the text and content on the website.

### Contact form

This page is static so [formspree.io](https://formspree.io/) is used to forward the message to your email. Visitors can send you up to 1,000 emails per month for free.
You can set your email in the [`config.toml`](//github.com/MarcusVirg/forty/blob/master/exampleSite/config.toml) file. You then have to confirm your email with formspree and will begin recieving messages after you do so. I recommend only having the contact form on one page, most likely the index.html, because you have to confirm for every URL the contact form is on.

### Preview

You can see a preview of your site while developing it by running Hugo's built-in webserver.

    $ hugo server -D

Now enter [`localhost:1313`](http://localhost:1313/) in the address bar of your browser to see your site.

`NOTE: In the command above -D loads content that is marked as a draft. You can switch content from draft to final by changing the frontmatter value of draft to false in the .md file for the content.`

## Contributing

Find a bug or want a new feature? Use the issue tracker or submit a pull request.

## License

This theme is released under the Creative Commons Attribution 3.0.
For more information read the [License](//github.com/MarcusVirg/forty/blob/master/LICENSE.md).

## Acknowledgements

Thanks to:

- AJ from [HTML5 UP](https://html5up.net/) for creating the theme
- [Bjørn Erik Pedersen](https://github.com/bep), [Steve Francia](//github.com/spf13), [digitalcraftsman](//github.com/digitalcraftsman), and others for creating and maintaining Hugo.
