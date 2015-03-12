Changelog
=========

2.0 (unreleased)
----------------

- Allow fullview portlets to be derived while making sure, they don't run into
  an infinite recursion loop. This is done via annotating the request with the
  portlet hash.
  [thet]

- Return the content object's title for the management screen portlet title to
  better distinguish several portlets.
  [thet]

- Use the ``RelatedItemsFieldWidget`` from ``plone.app.widgets`` and switch to
  a ``z3c.form`` based implementation.
  [thet]


1.1 (2015-03-06)
----------------

- Only render the fullview portlet, if it's rendered on a context where it is
  directly assigned. Don't render, if it was derived from a parent context.
  This avoids infinite loops when a fullview portlets renders a childitem.
  [thet]


1.0 (2015-03-04)
----------------

- Initial version.
  [thet]
