.. ==================================================
.. FOR YOUR INFORMATION
.. --------------------------------------------------
.. -*- coding: utf-8 -*- with BOM.

.. include:: ../Includes.txt


.. _configuration:

Configuration Reference
=======================

Target group: **Developers**


.. _configuration-typoscript:

TypoScript Reference
--------------------

Most of the setup properties will be inherited from the constants. However you always override them in the setup part of
your TypoScript Template.

Properties
^^^^^^^^^^

.. container:: ts-properties

	=========================== ===================================== ======================= ====================
	Property                    Data type                             :ref:`t3tsref:stdwrap`  Default
	=========================== ===================================== ======================= ====================
	`settings.link`_            :ref:`t3tsref:data-type-string`       no
	`settings.theme`_           :ref:`t3tsref:data-type-string`       no                      :code:`dark-bottom`
	`settings.container`_       :ref:`t3tsref:data-type-string`       no                      :code:`body`
	`settings.path`_            :ref:`t3tsref:data-type-string`       no                      :code:`/`
	`settings.domain`_          :ref:`t3tsref:data-type-string`       no
	`settings.expiryDays`_      :ref:`t3tsref:data-type-integer`      no                      :code:`365`
	=========================== ===================================== ======================= ====================


Property details
^^^^^^^^^^^^^^^^


.. _ts-plugin-tx-cookieconsent2-settings-link:

settings.link
"""""""""""""

:typoscript:`plugin.tx_extensionkey.settings.link =` :ref:`t3tsref:data-type-string`

A link to your cookie policy or disclaimer. Can be a URL to an external page or the uid of a page in your pagetree.


.. _ts-plugin-tx-cookieconsent2-settings-theme:

settings.theme
""""""""""""""

:typoscript:`plugin.tx_extensionkey.settings.theme =` :ref:`t3tsref:data-type-string`

The theme you wish to use. Valid options are ``dark-top``, ``dark-floating``, ``dark-bottom``, ``light-top``,
``light-floating``, ``light-bottom`` or a url to a CSS file. Leave empty to not include any extra CSS files.


.. _ts-plugin-tx-cookieconsent2-settings-container:

settings.container
""""""""""""""""""

:typoscript:`plugin.tx_extensionkey.settings.container =` :ref:`t3tsref:data-type-string`

A CSS selector to define with element of your page to append the cookie consent notice to. Please consider
that the default themes rely on this setting, if you change this you will probably have to use your own theme.


.. _ts-plugin-tx-cookieconsent2-settings-path:

settings.path
"""""""""""""

:typoscript:`plugin.tx_extensionkey.settings.path =` :ref:`t3tsref:data-type-string`

The path for the consent cookie that Cookie Consent uses, to remember that users have consented to cookies.
Use to limit consent to a specific path within your website.


.. _ts-plugin-tx-cookieconsent2-settings-domain:

settings.domain
"""""""""""""""

:typoscript:`plugin.tx_extensionkey.settings.domain =` :ref:`t3tsref:data-type-string`

The domain for the consent cookie that Cookie Consent uses, to remember that users have consented to cookies.
Useful if your website uses multiple subdomains. Defaults to *the current subdomain*.


.. _ts-plugin-tx-cookieconsent2-settings-expiryDays:

settings.expiryDays
"""""""""""""""""""

:typoscript:`plugin.tx_extensionkey.settings.expiryDays =` :ref:`t3tsref:data-type-integer`

The number of days Cookie Consent should store the user’s consent information for.

