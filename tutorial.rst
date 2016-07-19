Describe table 
==============

URL Syntax
----------

  <SERVER_ADDR>:<SERVER_PORT>/<TABLE_NAME>/meta


Table entries
=============

URL Syntax
----------

  <SERVER_ADDR>:<SERVER_PORT>/<TABLE_NAME>/count


Querying table
==============

URL Syntax
----------

  <SERVER_ADDR>:<SERVER_PORT>/<TABLE_NAME>?<PARAM_NAME>=<PARAM_VAL>[&...]

Query params
------------

- <column_name>: Its value is used to select the rows with the matching column.
  This can be either an exact match or a wildcard (e.g. ``%xxx``)

- *filter*: Can be used multiple times. Its value is::
    <column_name>^<comp>^<threshold>
   where ``<comp>`` is one of ``lt`` (less than), ``le`` (less than or equal), 
   ``gt`` (greater than), ``ge`` (greater than or equal)

- *sort*: Its value is the column name to be used for sorting the resources list.

- *limit*: Its value is the number of entries to return in the resources list.

