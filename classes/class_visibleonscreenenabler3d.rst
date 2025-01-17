:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/VisibleOnScreenEnabler3D.xml.

.. _class_VisibleOnScreenEnabler3D:

VisibleOnScreenEnabler3D
========================

**Inherits:** :ref:`VisibleOnScreenNotifier3D<class_VisibleOnScreenNotifier3D>` **<** :ref:`VisualInstance3D<class_VisualInstance3D>` **<** :ref:`Node3D<class_Node3D>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

Enables certain nodes only when approximately visible.

.. rst-class:: classref-introduction-group

Description
-----------

The VisibleOnScreenEnabler3D will disable :ref:`RigidBody3D<class_RigidBody3D>` and :ref:`AnimationPlayer<class_AnimationPlayer>` nodes when they are not visible. It will only affect other nodes within the same scene as the VisibleOnScreenEnabler3D itself.

If you just want to receive notifications, use :ref:`VisibleOnScreenNotifier3D<class_VisibleOnScreenNotifier3D>` instead.

\ **Note:** VisibleOnScreenEnabler3D uses an approximate heuristic for performance reasons. It doesn't take walls and other occlusion into account. The heuristic is an implementation detail and may change in future versions. If you need precise visibility checking, use another method such as adding an :ref:`Area3D<class_Area3D>` node as a child of a :ref:`Camera3D<class_Camera3D>` node and/or :ref:`Vector3.dot<class_Vector3_method_dot>`.

\ **Note:** VisibleOnScreenEnabler3D will not affect nodes added after scene initialization.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-------------------------------------------------------------+-----------------------------------------------------------------------------------+--------------------+
   | :ref:`EnableMode<enum_VisibleOnScreenEnabler3D_EnableMode>` | :ref:`enable_mode<class_VisibleOnScreenEnabler3D_property_enable_mode>`           | ``0``              |
   +-------------------------------------------------------------+-----------------------------------------------------------------------------------+--------------------+
   | :ref:`NodePath<class_NodePath>`                             | :ref:`enable_node_path<class_VisibleOnScreenEnabler3D_property_enable_node_path>` | ``NodePath("..")`` |
   +-------------------------------------------------------------+-----------------------------------------------------------------------------------+--------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Enumerations
------------

.. _enum_VisibleOnScreenEnabler3D_EnableMode:

.. rst-class:: classref-enumeration

enum **EnableMode**:

.. _class_VisibleOnScreenEnabler3D_constant_ENABLE_MODE_INHERIT:

.. rst-class:: classref-enumeration-constant

:ref:`EnableMode<enum_VisibleOnScreenEnabler3D_EnableMode>` **ENABLE_MODE_INHERIT** = ``0``



.. _class_VisibleOnScreenEnabler3D_constant_ENABLE_MODE_ALWAYS:

.. rst-class:: classref-enumeration-constant

:ref:`EnableMode<enum_VisibleOnScreenEnabler3D_EnableMode>` **ENABLE_MODE_ALWAYS** = ``1``



.. _class_VisibleOnScreenEnabler3D_constant_ENABLE_MODE_WHEN_PAUSED:

.. rst-class:: classref-enumeration-constant

:ref:`EnableMode<enum_VisibleOnScreenEnabler3D_EnableMode>` **ENABLE_MODE_WHEN_PAUSED** = ``2``



.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_VisibleOnScreenEnabler3D_property_enable_mode:

.. rst-class:: classref-property

:ref:`EnableMode<enum_VisibleOnScreenEnabler3D_EnableMode>` **enable_mode** = ``0``

.. rst-class:: classref-property-setget

- void **set_enable_mode** **(** :ref:`EnableMode<enum_VisibleOnScreenEnabler3D_EnableMode>` value **)**
- :ref:`EnableMode<enum_VisibleOnScreenEnabler3D_EnableMode>` **get_enable_mode** **(** **)**

.. container:: contribute

	There is currently no description for this property. Please help us by :ref:`contributing one <doc_updating_the_class_reference>`!

.. rst-class:: classref-item-separator

----

.. _class_VisibleOnScreenEnabler3D_property_enable_node_path:

.. rst-class:: classref-property

:ref:`NodePath<class_NodePath>` **enable_node_path** = ``NodePath("..")``

.. rst-class:: classref-property-setget

- void **set_enable_node_path** **(** :ref:`NodePath<class_NodePath>` value **)**
- :ref:`NodePath<class_NodePath>` **get_enable_node_path** **(** **)**

.. container:: contribute

	There is currently no description for this property. Please help us by :ref:`contributing one <doc_updating_the_class_reference>`!

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
