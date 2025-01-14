.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the YSort.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_YSort:

YSort
=====

**Inherits:** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

Sort all child nodes based on their Y positions.

Properties
----------

+-------------------------+--------------------------------------------------------+------+
| :ref:`bool<class_bool>` | :ref:`sort_enabled<class_YSort_property_sort_enabled>` | true |
+-------------------------+--------------------------------------------------------+------+

Description
-----------

Sort all child nodes based on their Y positions. The child node must inherit from :ref:`CanvasItem<class_CanvasItem>` for it to be sorted. Nodes that have a higher Y position will be drawn later, so they will appear on top of nodes that have a lower Y position.

Nesting of YSort nodes is possible. Children YSort nodes will be sorted in the same space as the parent YSort, allowing to better organize a scene or divide it in multiple ones, yet keep the unique sorting.

Property Descriptions
---------------------

.. _class_YSort_property_sort_enabled:

- :ref:`bool<class_bool>` **sort_enabled**

+-----------+-------------------------+
| *Default* | true                    |
+-----------+-------------------------+
| *Setter*  | set_sort_enabled(value) |
+-----------+-------------------------+
| *Getter*  | is_sort_enabled()       |
+-----------+-------------------------+

If ``true``, child nodes are sorted, otherwise sorting is disabled.

