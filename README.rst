====================
kotti_contentpreview
====================

Content preview for Kotti.

`Find out more about Kotti`_

Setup
=====

To activate the ``kotti_contentpreview`` add-on in your Kotti site, you need to
add an entry to the ``kotti.configurators`` setting in your Paste
Deploy config.  If you don't have a ``kotti.configurators`` option,
add one. ``kotti_contentpreview`` depends on kotti_settings_, so you have to
add also an entry for this add-on.
The line in your ``[app:main]`` (or ``[app:kotti]``, depending on how
you setup Fanstatic) section could then look like this:

.. code-block:: ini

    kotti.configurators =
        kotti_settings.kotti_configure
        kotti_contentpreview.kotti_configure

After activation you get a popover with the content of the content type when
you hover over a title in the @@contents view. You can adjust settings for the
view that should be called, the size of the popup window and the delay of showing
and hiding of the window on the settings page. Point your browser to
http://your.domain/@@settings to get to the settingspage or use the submenupoint of 'Site Setup'.

.. _Find out more about Kotti: http://pypi.python.org/pypi/Kotti
.. _kotti_settings: http://pypi.python.org/pypi/kotti_settings
