# Maintenance and Error Pages

Static content for displaying error pages on failed servers and maintenance
pages on servers undergoing maintenance.

* ``error.html``: Error page that is displayed when a server throws a 50x error.
* ``scheduled.html``: Maintenance page to be displayed when a server is
    undergoing scheduled maintenance. This page can be edited on the live server
    to include a maintenance window if needed.
* ``unscheduled.html``: Maintenance page to be displayed when there is
    unscheduled maintenance.
* ``provisioning.html``: Maintenance page to be displayed when an server for an
    instance is in the process of being provisione.


All these pages share the same static files placed in the static directory. Due
to the way the server is set up for serving these pages, the assets need to be
referenced as ``/error/static/static_file.ext`` to work on the actual server.

To make it easy to test, you can simply create a directory called ``error`` and
link the static directory inside it.
