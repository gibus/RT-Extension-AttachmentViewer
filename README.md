# NAME

RT::Extension::AttachmentViewer - View full size attachments from the dropzone

# DESCRIPTION

By default, when attachments are to be uploaded in RT, the dropzone where there are added shows a thunbmbnail. This extention allows to click on the thumbnail to view the full size attachment in a popup, whether it's an image, a PDF, an audio, an HTML or a text file, otherwise it can be downloaded in your browser.

# RT VERSION

Works with RT 5 and RT 6.

# INSTALLATION

- export `$RTHOME=/home/of/your/RT/installation/lib`

    This is needed if your `RT` installation directory is not `/opt/rt6/` for RT 6 nor C/opt/rt5/> for RT 5.

- `perl Makefile.PL`
- `make`
- `make install`

    May need root permissions

- Edit your `/opt/rt6/etc/RT_SiteConfig.pm`

    Add this line:

        Plugin('RT::Extension::AttachmentViewer');

    or add `RT::Extension::AttachmentViewer` to your existing `@Plugins` line.

- Clear your mason cache

        rm -rf /opt/rt6/var/mason_data/obj

- Restart your webserver

# AUTHOR

Gérald Sédrati <gibus@easter-eggs.com>

# REPOSITORY

[https://github.com/gibus/RT-Extension-AttachmentViewer](https://github.com/gibus/RT-Extension-AttachmentViewer)

# BUGS

All bugs should be reported via email to

[bug-RT-Extension-AttachmentViewer@rt.cpan.org](mailto:bug-RT-Extension-AttachmentViewer@rt.cpan.org)

or via the web at

[rt.cpan.org](http://rt.cpan.org/Public/Dist/Display.html?Name=RT-Extension-AttachmentViewer).

# LICENSE AND COPYRIGHT

This software is Copyright (c) 2026 by Gérald Sédrati, Easter-Eggs

This is free software, licensed under:

The GNU General Public License, Version 3, June 2007
