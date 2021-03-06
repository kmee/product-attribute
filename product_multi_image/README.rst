.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
   :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
   :alt: License: AGPL-3

===========================
Multiple Images in Products
===========================

This module implements the possibility to have multiple images for a product
template, a.k.a. an image gallery.

Installation
============

To install this module, you need to:

* Install ``base_multi_image`` from
  `OCA/server-tools <https://github.com/OCA/server-tools>`_.

Usage
=====

To use this module, you need to:

#. Go to *Sales > Products > Products* and choose a product template.
#. Go to the new *Images* tab.
#. Add a new image.
#. Refresh the page.
#. The first image in the collection is the main image for the product.
#. Go to *Sales > Products > Product Variants* and choose a product variant.
#. It shares the main image and collection with its template.
#. If you change the main image from the variant, it becomes the variant's main
   image but does not appear in the template.
#. If you change images from the *Images* tab, it changes in the template too.

.. image:: https://odoo-community.org/website/image/ir.attachment/5784_f2813bd/datas
   :alt: Try me on Runbot
   :target: https://runbot.odoo-community.org/runbot/135/8.0

Known issues / Roadmap
======================

* Provide proper migration scripts from module product_images from 7.0.
* Migrate to v8 api when https://github.com/odoo/odoo/issues/10799 gets fixed.
* If you try to sort images before saving the product variant or template, you
  will get an error similar to ``DataError: invalid input syntax for integer:
  "one2many_v_id_62"``. This bug has not been fixed yet, but a workaround is to
  save and edit again to sort images.

Bug Tracker
===========

Bugs are tracked on `GitHub Issues
<https://github.com/OCA/product-attribute/issues>`_. In case of trouble, please
check there if your issue has already been reported. If you spotted it first,
help us smashing it by providing a detailed and welcomed `feedback
<https://github.com/OCA/
product-attribute/issues/new?body=module:%20
product_multi_image%0Aversion:%20
8.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Credits
=======

Original implementation
-----------------------
This module is inspired in previous module *product_images* from OpenLabs
and Akretion.


Contributors
------------

* Pedro M. Baeza <pedro.baeza@serviciosbaeza.com>
* Rafael Blasco <rafabn@antiun.com>
* Jairo Llopis <yajo.sk8@gmail.com>

Maintainer
----------

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

This module is maintained by the OCA.

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

To contribute to this module, please visit https://odoo-community.org.
