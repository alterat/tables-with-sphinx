Long tables
===========

You might be dealing with a large table, one that would be difficult to write as a `regular table <regular-table.html>`_ described before. 

One possibility is to use CSV files. You can store your data in a CSV table, without the need to worry about misplacing an equal sign in your table. 

If your table is really long, however, it might sometimes break in the PDF output. Take for example the table below. 

In order to make it look good in the PDF, you should use some LaTeX magic, disguised in RST directives. Using the :code:`:class: longtable` parameter in the table definition allows to nicely break long tables into several pages. You can also control the width of the individual columns with the :code:`tabularcolumns` directive: this will be familiar to you if you used LaTeX before. 

Finally, the :code:`:widths: 1 1` parameter controls how the columns look in the HTML page. As you can see, this is independent on the way columns behave in the PDF. 

.. code-block:: rst

   .. tabularcolumns:: |p{1cm}|p{7cm}|
   
   .. csv-table:: Lorem Ipsum
      :file: _files/lorem-tab.csv 
      :header-rows: 1 
      :class: longtable
      :widths: 1 1

.. tabularcolumns:: |p{1cm}|p{7cm}|

.. csv-table:: Lorem Ipsum
   :file: _files/lorem-tab.csv 
   :header-rows: 1 
   :class: longtable
   :widths: 1 1
