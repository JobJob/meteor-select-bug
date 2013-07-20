meteor-select-bug
=================

A workaround added to the minimal reproduction of the FF select bug in Meteor. https://github.com/meteor/meteor/issues/1234

After running in FF try in the firebug console:
    Session.set("syntax", "b")

If you comment out the Deps.autorun on line 26, you'll see it doesn't work.
