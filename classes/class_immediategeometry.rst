.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the ImmediateGeometry.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_ImmediateGeometry:

ImmediateGeometry
=================

**Inherits:** :ref:`GeometryInstance<class_GeometryInstance>` **<** :ref:`VisualInstance<class_VisualInstance>` **<** :ref:`Spatial<class_Spatial>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------

Draws simple geometry from code.

Methods
-------

+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`add_sphere<class_ImmediateGeometry_method_add_sphere>` **(** :ref:`int<class_int>` lats, :ref:`int<class_int>` lons, :ref:`float<class_float>` radius, :ref:`bool<class_bool>` add_uv=true **)** |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`add_vertex<class_ImmediateGeometry_method_add_vertex>` **(** :ref:`Vector3<class_Vector3>` position **)**                                                                                        |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`begin<class_ImmediateGeometry_method_begin>` **(** :ref:`PrimitiveType<enum_Mesh_PrimitiveType>` primitive, :ref:`Texture<class_Texture>` texture=null **)**                                     |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`clear<class_ImmediateGeometry_method_clear>` **(** **)**                                                                                                                                         |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`end<class_ImmediateGeometry_method_end>` **(** **)**                                                                                                                                             |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`set_color<class_ImmediateGeometry_method_set_color>` **(** :ref:`Color<class_Color>` color **)**                                                                                                 |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`set_normal<class_ImmediateGeometry_method_set_normal>` **(** :ref:`Vector3<class_Vector3>` normal **)**                                                                                          |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`set_tangent<class_ImmediateGeometry_method_set_tangent>` **(** :ref:`Plane<class_Plane>` tangent **)**                                                                                           |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`set_uv<class_ImmediateGeometry_method_set_uv>` **(** :ref:`Vector2<class_Vector2>` uv **)**                                                                                                      |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void | :ref:`set_uv2<class_ImmediateGeometry_method_set_uv2>` **(** :ref:`Vector2<class_Vector2>` uv **)**                                                                                                    |
+------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Description
-----------

Draws simple geometry from code. Uses a drawing mode similar to OpenGL 1.x.

Method Descriptions
-------------------

.. _class_ImmediateGeometry_method_add_sphere:

- void **add_sphere** **(** :ref:`int<class_int>` lats, :ref:`int<class_int>` lons, :ref:`float<class_float>` radius, :ref:`bool<class_bool>` add_uv=true **)**

Simple helper to draw an UV sphere with given latitude, longitude and radius.

.. _class_ImmediateGeometry_method_add_vertex:

- void **add_vertex** **(** :ref:`Vector3<class_Vector3>` position **)**

Adds a vertex with the currently set color/uv/etc.

.. _class_ImmediateGeometry_method_begin:

- void **begin** **(** :ref:`PrimitiveType<enum_Mesh_PrimitiveType>` primitive, :ref:`Texture<class_Texture>` texture=null **)**

Begin drawing (And optionally pass a texture override). When done call end(). For more information on how this works, search for glBegin() glEnd() references.

For the type of primitive, use the :ref:`Mesh<class_Mesh>`.``PRIMITIVE_*`` enumerations.

.. _class_ImmediateGeometry_method_clear:

- void **clear** **(** **)**

Clears everything that was drawn using begin/end.

.. _class_ImmediateGeometry_method_end:

- void **end** **(** **)**

Ends a drawing context and displays the results.

.. _class_ImmediateGeometry_method_set_color:

- void **set_color** **(** :ref:`Color<class_Color>` color **)**

The current drawing color.

.. _class_ImmediateGeometry_method_set_normal:

- void **set_normal** **(** :ref:`Vector3<class_Vector3>` normal **)**

The next vertex's normal.

.. _class_ImmediateGeometry_method_set_tangent:

- void **set_tangent** **(** :ref:`Plane<class_Plane>` tangent **)**

The next vertex's tangent (and binormal facing).

.. _class_ImmediateGeometry_method_set_uv:

- void **set_uv** **(** :ref:`Vector2<class_Vector2>` uv **)**

The next vertex's UV.

.. _class_ImmediateGeometry_method_set_uv2:

- void **set_uv2** **(** :ref:`Vector2<class_Vector2>` uv **)**

The next vertex's second layer UV.

