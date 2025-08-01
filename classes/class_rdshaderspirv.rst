:github_url: hide

.. DO NOT EDIT THIS FILE!!!
.. Generated automatically from Godot engine sources.
.. Generator: https://github.com/godotengine/godot/tree/master/doc/tools/make_rst.py.
.. XML source: https://github.com/godotengine/godot/tree/master/doc/classes/RDShaderSPIRV.xml.

.. _class_RDShaderSPIRV:

RDShaderSPIRV
=============

**Inherits:** :ref:`Resource<class_Resource>` **<** :ref:`RefCounted<class_RefCounted>` **<** :ref:`Object<class_Object>`

SPIR-V intermediate representation as part of an :ref:`RDShaderFile<class_RDShaderFile>` (used by :ref:`RenderingDevice<class_RenderingDevice>`).

.. rst-class:: classref-introduction-group

Description
-----------

**RDShaderSPIRV** represents an :ref:`RDShaderFile<class_RDShaderFile>`'s `SPIR-V <https://www.khronos.org/spir/>`__ code for various shader stages, as well as possible compilation error messages. SPIR-V is a low-level intermediate shader representation. This intermediate representation is not used directly by GPUs for rendering, but it can be compiled into binary shaders that GPUs can understand. Unlike compiled shaders, SPIR-V is portable across GPU models and driver versions.

This object is used by :ref:`RenderingDevice<class_RenderingDevice>`.

.. rst-class:: classref-reftable-group

Properties
----------

.. table::
   :widths: auto

   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+
   | :ref:`PackedByteArray<class_PackedByteArray>` | :ref:`bytecode_compute<class_RDShaderSPIRV_property_bytecode_compute>`                                         | ``PackedByteArray()`` |
   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+
   | :ref:`PackedByteArray<class_PackedByteArray>` | :ref:`bytecode_fragment<class_RDShaderSPIRV_property_bytecode_fragment>`                                       | ``PackedByteArray()`` |
   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+
   | :ref:`PackedByteArray<class_PackedByteArray>` | :ref:`bytecode_tesselation_control<class_RDShaderSPIRV_property_bytecode_tesselation_control>`                 | ``PackedByteArray()`` |
   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+
   | :ref:`PackedByteArray<class_PackedByteArray>` | :ref:`bytecode_tesselation_evaluation<class_RDShaderSPIRV_property_bytecode_tesselation_evaluation>`           | ``PackedByteArray()`` |
   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+
   | :ref:`PackedByteArray<class_PackedByteArray>` | :ref:`bytecode_vertex<class_RDShaderSPIRV_property_bytecode_vertex>`                                           | ``PackedByteArray()`` |
   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+
   | :ref:`String<class_String>`                   | :ref:`compile_error_compute<class_RDShaderSPIRV_property_compile_error_compute>`                               | ``""``                |
   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+
   | :ref:`String<class_String>`                   | :ref:`compile_error_fragment<class_RDShaderSPIRV_property_compile_error_fragment>`                             | ``""``                |
   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+
   | :ref:`String<class_String>`                   | :ref:`compile_error_tesselation_control<class_RDShaderSPIRV_property_compile_error_tesselation_control>`       | ``""``                |
   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+
   | :ref:`String<class_String>`                   | :ref:`compile_error_tesselation_evaluation<class_RDShaderSPIRV_property_compile_error_tesselation_evaluation>` | ``""``                |
   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+
   | :ref:`String<class_String>`                   | :ref:`compile_error_vertex<class_RDShaderSPIRV_property_compile_error_vertex>`                                 | ``""``                |
   +-----------------------------------------------+----------------------------------------------------------------------------------------------------------------+-----------------------+

.. rst-class:: classref-reftable-group

Methods
-------

.. table::
   :widths: auto

   +-----------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`PackedByteArray<class_PackedByteArray>` | :ref:`get_stage_bytecode<class_RDShaderSPIRV_method_get_stage_bytecode>`\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|                                                   |
   +-----------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | :ref:`String<class_String>`                   | :ref:`get_stage_compile_error<class_RDShaderSPIRV_method_get_stage_compile_error>`\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|                                         |
   +-----------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                        | :ref:`set_stage_bytecode<class_RDShaderSPIRV_method_set_stage_bytecode>`\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, bytecode\: :ref:`PackedByteArray<class_PackedByteArray>`\ ) |
   +-----------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
   | |void|                                        | :ref:`set_stage_compile_error<class_RDShaderSPIRV_method_set_stage_compile_error>`\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, compile_error\: :ref:`String<class_String>`\ )    |
   +-----------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Property Descriptions
---------------------

.. _class_RDShaderSPIRV_property_bytecode_compute:

.. rst-class:: classref-property

:ref:`PackedByteArray<class_PackedByteArray>` **bytecode_compute** = ``PackedByteArray()`` :ref:`🔗<class_RDShaderSPIRV_property_bytecode_compute>`

.. rst-class:: classref-property-setget

- |void| **set_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, bytecode\: :ref:`PackedByteArray<class_PackedByteArray>`\ )
- :ref:`PackedByteArray<class_PackedByteArray>` **get_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|

The SPIR-V bytecode for the compute shader stage.

**Note:** The returned array is *copied* and any changes to it will not update the original property value. See :ref:`PackedByteArray<class_PackedByteArray>` for more details.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_property_bytecode_fragment:

.. rst-class:: classref-property

:ref:`PackedByteArray<class_PackedByteArray>` **bytecode_fragment** = ``PackedByteArray()`` :ref:`🔗<class_RDShaderSPIRV_property_bytecode_fragment>`

.. rst-class:: classref-property-setget

- |void| **set_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, bytecode\: :ref:`PackedByteArray<class_PackedByteArray>`\ )
- :ref:`PackedByteArray<class_PackedByteArray>` **get_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|

The SPIR-V bytecode for the fragment shader stage.

**Note:** The returned array is *copied* and any changes to it will not update the original property value. See :ref:`PackedByteArray<class_PackedByteArray>` for more details.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_property_bytecode_tesselation_control:

.. rst-class:: classref-property

:ref:`PackedByteArray<class_PackedByteArray>` **bytecode_tesselation_control** = ``PackedByteArray()`` :ref:`🔗<class_RDShaderSPIRV_property_bytecode_tesselation_control>`

.. rst-class:: classref-property-setget

- |void| **set_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, bytecode\: :ref:`PackedByteArray<class_PackedByteArray>`\ )
- :ref:`PackedByteArray<class_PackedByteArray>` **get_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|

The SPIR-V bytecode for the tessellation control shader stage.

**Note:** The returned array is *copied* and any changes to it will not update the original property value. See :ref:`PackedByteArray<class_PackedByteArray>` for more details.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_property_bytecode_tesselation_evaluation:

.. rst-class:: classref-property

:ref:`PackedByteArray<class_PackedByteArray>` **bytecode_tesselation_evaluation** = ``PackedByteArray()`` :ref:`🔗<class_RDShaderSPIRV_property_bytecode_tesselation_evaluation>`

.. rst-class:: classref-property-setget

- |void| **set_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, bytecode\: :ref:`PackedByteArray<class_PackedByteArray>`\ )
- :ref:`PackedByteArray<class_PackedByteArray>` **get_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|

The SPIR-V bytecode for the tessellation evaluation shader stage.

**Note:** The returned array is *copied* and any changes to it will not update the original property value. See :ref:`PackedByteArray<class_PackedByteArray>` for more details.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_property_bytecode_vertex:

.. rst-class:: classref-property

:ref:`PackedByteArray<class_PackedByteArray>` **bytecode_vertex** = ``PackedByteArray()`` :ref:`🔗<class_RDShaderSPIRV_property_bytecode_vertex>`

.. rst-class:: classref-property-setget

- |void| **set_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, bytecode\: :ref:`PackedByteArray<class_PackedByteArray>`\ )
- :ref:`PackedByteArray<class_PackedByteArray>` **get_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|

The SPIR-V bytecode for the vertex shader stage.

**Note:** The returned array is *copied* and any changes to it will not update the original property value. See :ref:`PackedByteArray<class_PackedByteArray>` for more details.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_property_compile_error_compute:

.. rst-class:: classref-property

:ref:`String<class_String>` **compile_error_compute** = ``""`` :ref:`🔗<class_RDShaderSPIRV_property_compile_error_compute>`

.. rst-class:: classref-property-setget

- |void| **set_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, compile_error\: :ref:`String<class_String>`\ )
- :ref:`String<class_String>` **get_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|

The compilation error message for the compute shader stage (set by the SPIR-V compiler and Godot). If empty, shader compilation was successful.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_property_compile_error_fragment:

.. rst-class:: classref-property

:ref:`String<class_String>` **compile_error_fragment** = ``""`` :ref:`🔗<class_RDShaderSPIRV_property_compile_error_fragment>`

.. rst-class:: classref-property-setget

- |void| **set_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, compile_error\: :ref:`String<class_String>`\ )
- :ref:`String<class_String>` **get_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|

The compilation error message for the fragment shader stage (set by the SPIR-V compiler and Godot). If empty, shader compilation was successful.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_property_compile_error_tesselation_control:

.. rst-class:: classref-property

:ref:`String<class_String>` **compile_error_tesselation_control** = ``""`` :ref:`🔗<class_RDShaderSPIRV_property_compile_error_tesselation_control>`

.. rst-class:: classref-property-setget

- |void| **set_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, compile_error\: :ref:`String<class_String>`\ )
- :ref:`String<class_String>` **get_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|

The compilation error message for the tessellation control shader stage (set by the SPIR-V compiler and Godot). If empty, shader compilation was successful.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_property_compile_error_tesselation_evaluation:

.. rst-class:: classref-property

:ref:`String<class_String>` **compile_error_tesselation_evaluation** = ``""`` :ref:`🔗<class_RDShaderSPIRV_property_compile_error_tesselation_evaluation>`

.. rst-class:: classref-property-setget

- |void| **set_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, compile_error\: :ref:`String<class_String>`\ )
- :ref:`String<class_String>` **get_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|

The compilation error message for the tessellation evaluation shader stage (set by the SPIR-V compiler and Godot). If empty, shader compilation was successful.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_property_compile_error_vertex:

.. rst-class:: classref-property

:ref:`String<class_String>` **compile_error_vertex** = ``""`` :ref:`🔗<class_RDShaderSPIRV_property_compile_error_vertex>`

.. rst-class:: classref-property-setget

- |void| **set_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, compile_error\: :ref:`String<class_String>`\ )
- :ref:`String<class_String>` **get_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const|

The compilation error message for the vertex shader stage (set by the SPIR-V compiler and Godot). If empty, shader compilation was successful.

.. rst-class:: classref-section-separator

----

.. rst-class:: classref-descriptions-group

Method Descriptions
-------------------

.. _class_RDShaderSPIRV_method_get_stage_bytecode:

.. rst-class:: classref-method

:ref:`PackedByteArray<class_PackedByteArray>` **get_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const| :ref:`🔗<class_RDShaderSPIRV_method_get_stage_bytecode>`

Equivalent to getting one of :ref:`bytecode_compute<class_RDShaderSPIRV_property_bytecode_compute>`, :ref:`bytecode_fragment<class_RDShaderSPIRV_property_bytecode_fragment>`, :ref:`bytecode_tesselation_control<class_RDShaderSPIRV_property_bytecode_tesselation_control>`, :ref:`bytecode_tesselation_evaluation<class_RDShaderSPIRV_property_bytecode_tesselation_evaluation>`, :ref:`bytecode_vertex<class_RDShaderSPIRV_property_bytecode_vertex>`.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_method_get_stage_compile_error:

.. rst-class:: classref-method

:ref:`String<class_String>` **get_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`\ ) |const| :ref:`🔗<class_RDShaderSPIRV_method_get_stage_compile_error>`

Returns the compilation error message for the given shader ``stage``. Equivalent to getting one of :ref:`compile_error_compute<class_RDShaderSPIRV_property_compile_error_compute>`, :ref:`compile_error_fragment<class_RDShaderSPIRV_property_compile_error_fragment>`, :ref:`compile_error_tesselation_control<class_RDShaderSPIRV_property_compile_error_tesselation_control>`, :ref:`compile_error_tesselation_evaluation<class_RDShaderSPIRV_property_compile_error_tesselation_evaluation>`, :ref:`compile_error_vertex<class_RDShaderSPIRV_property_compile_error_vertex>`.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_method_set_stage_bytecode:

.. rst-class:: classref-method

|void| **set_stage_bytecode**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, bytecode\: :ref:`PackedByteArray<class_PackedByteArray>`\ ) :ref:`🔗<class_RDShaderSPIRV_method_set_stage_bytecode>`

Sets the SPIR-V ``bytecode`` for the given shader ``stage``. Equivalent to setting one of :ref:`bytecode_compute<class_RDShaderSPIRV_property_bytecode_compute>`, :ref:`bytecode_fragment<class_RDShaderSPIRV_property_bytecode_fragment>`, :ref:`bytecode_tesselation_control<class_RDShaderSPIRV_property_bytecode_tesselation_control>`, :ref:`bytecode_tesselation_evaluation<class_RDShaderSPIRV_property_bytecode_tesselation_evaluation>`, :ref:`bytecode_vertex<class_RDShaderSPIRV_property_bytecode_vertex>`.

.. rst-class:: classref-item-separator

----

.. _class_RDShaderSPIRV_method_set_stage_compile_error:

.. rst-class:: classref-method

|void| **set_stage_compile_error**\ (\ stage\: :ref:`ShaderStage<enum_RenderingDevice_ShaderStage>`, compile_error\: :ref:`String<class_String>`\ ) :ref:`🔗<class_RDShaderSPIRV_method_set_stage_compile_error>`

Sets the compilation error message for the given shader ``stage`` to ``compile_error``. Equivalent to setting one of :ref:`compile_error_compute<class_RDShaderSPIRV_property_compile_error_compute>`, :ref:`compile_error_fragment<class_RDShaderSPIRV_property_compile_error_fragment>`, :ref:`compile_error_tesselation_control<class_RDShaderSPIRV_property_compile_error_tesselation_control>`, :ref:`compile_error_tesselation_evaluation<class_RDShaderSPIRV_property_compile_error_tesselation_evaluation>`, :ref:`compile_error_vertex<class_RDShaderSPIRV_property_compile_error_vertex>`.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |required| replace:: :abbr:`required (This method is required to be overridden when extending its base class.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
.. |bitfield| replace:: :abbr:`BitField (This value is an integer composed as a bitmask of the following flags.)`
.. |void| replace:: :abbr:`void (No return value.)`
