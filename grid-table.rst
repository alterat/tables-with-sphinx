Grid tables
==============

Tables in RST can be obtained by simply "drawing" their structure with a combination of symbols, as in the following code snippet (it's easier seen than explained!). These are called `grid tables <http://www.sphinx-doc.org/en/master/rest.html#tables>`_ in the documentation.

.. code-block:: rst

   +------+---------------+
   | Item | Character     |
   +======+===============+
   | 1    | Puss in Boots |
   +------+---------------+
   | 2    | Cinderella    |
   +------+---------------+

A row of equal signs separates the first row from the rest, if you want it to be the label of your table. 

Grid tables are well rendered in the PDF output. This is the output from the snippet above.

.. table:: Grid table

   +------+---------------+
   | Item | Character     |
   +======+===============+
   | 1    | Puss in Boots |
   +------+---------------+
   | 2    | Cinderella    |
   +------+---------------+

