grainery-db
===========

Prototypal product database for `The Grainery Organic Food Co-op`_.

.. _The Grainery Organic Food Co-op: http://thegrainery.ca

Acquisition
^^^^^^^^^^^

The database system is available for `download from github`_.

.. _download from github:
   http://github.com/intuited/grainery-db/raw/dist/grainery-db.zip

Installation
^^^^^^^^^^^^

The system is an OpenOffice document,
so you should be able to just unzip the zip file,
using 7zip_ or some other archive program,
and open the .odb file contained within.

.. _7zip: http://www.7-zip.org/

Operation
^^^^^^^^^

The system consists of two different forms:

labels
~~~~~~

.. image:: http://github.com/intuited/grainery-db/raw/dist/screenshot.png

The first form, which should pop up when you open the document,
shows a list of products:
their titles, the category (e.g. "Flours") that they come under,
the beginning of the description, etc.

When you click on a row in the list,
that item's label will be generated and displayed in the preview box.
The big green **print** button is supposed to send it out to the printer.
I haven't tested that yet (well, not recently).

I did test PDF generation, which works (at least for me).
To do that, click the "Preview" button before clicking print.
The label should come up in a separate window;
from there you can click the PDF button in that window's toolbar.
I don't expect anyone to want to do this,
but it's useful as a way to show that the labels are getting generated
in some sort of useful form.

product info
~~~~~~~~~~~~

.. image:: http://github.com/intuited/grainery-db/raw/dist/screenshot-admin.png

The other part of the app is the product info page.
You can get there by clicking the button
in the bottom left-hand corner of the product page.
This brings up a form with a bunch of different fields.

The list in the center works like the list in the labels form.
The other areas of the page allow that product's data to be modified.

For example,
you can register a new bulk purchase —in the bottom right-hand corner—
or edit a product description (at the top right).
Changes that you make go right into the DB.

However, the preview doesn't refresh right away,
so to see the effect of the changes,
you have to click on a different row in the main list,
then click back on the item you edited.

I don't think this would be very difficult to fix,
so if people feel that this system is useful,
I'll figure out a way to make that work.

TODO
^^^^

This system was originally developed a couple of years ago.
Since that time, the Grainery has adopted a different pricing model,
and various new products (and prices!).

So the data, and even the label format, used in this system are out of date.

There has also been some effort made to make this data available online.

It is possible to rework the system so that
it can connect to an online database
and use the current pricing formula for the labels it produces.

