.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the ArrayMesh.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_ArrayMesh:

ArrayMesh
=========

**Inherits:** :ref:`Mesh<class_Mesh>` **<** :ref:`Resource<class_Resource>` **<** :ref:`Reference<class_Reference>` **<** :ref:`Object<class_Object>`

**Category:** Core

Brief Description
-----------------



Properties
----------

+-------------------------------------------------+--------------------------------------------------------------------+
| :ref:`BlendShapeMode<enum_Mesh_BlendShapeMode>` | :ref:`blend_shape_mode<class_ArrayMesh_property_blend_shape_mode>` |
+-------------------------------------------------+--------------------------------------------------------------------+
| :ref:`AABB<class_AABB>`                         | :ref:`custom_aabb<class_ArrayMesh_property_custom_aabb>`           |
+-------------------------------------------------+--------------------------------------------------------------------+

Methods
-------

+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`add_blend_shape<class_ArrayMesh_method_add_blend_shape>` **(** :ref:`String<class_String>` name **)**                                                                                                                                                                   |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`add_surface_from_arrays<class_ArrayMesh_method_add_surface_from_arrays>` **(** :ref:`PrimitiveType<enum_Mesh_PrimitiveType>` primitive, :ref:`Array<class_Array>` arrays, :ref:`Array<class_Array>` blend_shapes=[  ], :ref:`int<class_int>` compress_flags=97280 **)** |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`clear_blend_shapes<class_ArrayMesh_method_clear_blend_shapes>` **(** **)**                                                                                                                                                                                              |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                         | :ref:`get_blend_shape_count<class_ArrayMesh_method_get_blend_shape_count>` **(** **)** const                                                                                                                                                                                  |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`                   | :ref:`get_blend_shape_name<class_ArrayMesh_method_get_blend_shape_name>` **(** :ref:`int<class_int>` index **)** const                                                                                                                                                        |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Error<enum_@GlobalScope_Error>`         | :ref:`lightmap_unwrap<class_ArrayMesh_method_lightmap_unwrap>` **(** :ref:`Transform<class_Transform>` transform, :ref:`float<class_float>` texel_size **)**                                                                                                                  |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`regen_normalmaps<class_ArrayMesh_method_regen_normalmaps>` **(** **)**                                                                                                                                                                                                  |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                         | :ref:`surface_find_by_name<class_ArrayMesh_method_surface_find_by_name>` **(** :ref:`String<class_String>` name **)** const                                                                                                                                                   |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                         | :ref:`surface_get_array_index_len<class_ArrayMesh_method_surface_get_array_index_len>` **(** :ref:`int<class_int>` surf_idx **)** const                                                                                                                                       |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                         | :ref:`surface_get_array_len<class_ArrayMesh_method_surface_get_array_len>` **(** :ref:`int<class_int>` surf_idx **)** const                                                                                                                                                   |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                         | :ref:`surface_get_format<class_ArrayMesh_method_surface_get_format>` **(** :ref:`int<class_int>` surf_idx **)** const                                                                                                                                                         |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`String<class_String>`                   | :ref:`surface_get_name<class_ArrayMesh_method_surface_get_name>` **(** :ref:`int<class_int>` surf_idx **)** const                                                                                                                                                             |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`PrimitiveType<enum_Mesh_PrimitiveType>` | :ref:`surface_get_primitive_type<class_ArrayMesh_method_surface_get_primitive_type>` **(** :ref:`int<class_int>` surf_idx **)** const                                                                                                                                         |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`surface_remove<class_ArrayMesh_method_surface_remove>` **(** :ref:`int<class_int>` surf_idx **)**                                                                                                                                                                       |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`surface_set_name<class_ArrayMesh_method_surface_set_name>` **(** :ref:`int<class_int>` surf_idx, :ref:`String<class_String>` name **)**                                                                                                                                 |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                          | :ref:`surface_update_region<class_ArrayMesh_method_surface_update_region>` **(** :ref:`int<class_int>` surf_idx, :ref:`int<class_int>` offset, :ref:`PoolByteArray<class_PoolByteArray>` data **)**                                                                           |
+-----------------------------------------------+-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Enumerations
------------

.. _enum_ArrayMesh_ArrayType:

.. _class_ArrayMesh_constant_ARRAY_VERTEX:

.. _class_ArrayMesh_constant_ARRAY_NORMAL:

.. _class_ArrayMesh_constant_ARRAY_TANGENT:

.. _class_ArrayMesh_constant_ARRAY_COLOR:

.. _class_ArrayMesh_constant_ARRAY_TEX_UV:

.. _class_ArrayMesh_constant_ARRAY_TEX_UV2:

.. _class_ArrayMesh_constant_ARRAY_BONES:

.. _class_ArrayMesh_constant_ARRAY_WEIGHTS:

.. _class_ArrayMesh_constant_ARRAY_INDEX:

.. _class_ArrayMesh_constant_ARRAY_MAX:

enum **ArrayType**:

- **ARRAY_VERTEX** = **0** --- :ref:`PoolVector3Array<class_PoolVector3Array>`, :ref:`PoolVector2Array<class_PoolVector2Array>`, or :ref:`Array<class_Array>` of vertex positions.

- **ARRAY_NORMAL** = **1** --- :ref:`PoolVector3Array<class_PoolVector3Array>` of vertex normals.

- **ARRAY_TANGENT** = **2** --- :ref:`PoolRealArray<class_PoolRealArray>` of vertex tangents. Each element in groups of 4 floats, first 3 floats determine the tangent, and the last the binormal direction as -1 or 1.

- **ARRAY_COLOR** = **3** --- :ref:`PoolColorArray<class_PoolColorArray>` of vertex colors.

- **ARRAY_TEX_UV** = **4** --- :ref:`PoolVector2Array<class_PoolVector2Array>` for UV coordinates.

- **ARRAY_TEX_UV2** = **5** --- :ref:`PoolVector2Array<class_PoolVector2Array>` for second UV coordinates.

- **ARRAY_BONES** = **6** --- :ref:`PoolRealArray<class_PoolRealArray>` or :ref:`PoolIntArray<class_PoolIntArray>` of bone indices. Each element in groups of 4 floats.

- **ARRAY_WEIGHTS** = **7** --- :ref:`PoolRealArray<class_PoolRealArray>` of bone weights. Each element in groups of 4 floats.

- **ARRAY_INDEX** = **8** --- :ref:`PoolIntArray<class_PoolIntArray>` of integers used as indices referencing vertices, colors, normals, tangents, and textures. All of those arrays must have the same number of elements as the vertex array. No index can be beyond the vertex array size. When this index array is present, it puts the function into "index mode," where the index selects the \*i\*'th vertex, normal, tangent, color, UV, etc. This means if you want to have different normals or colors along an edge, you have to duplicate the vertices.

For triangles, the index array is interpreted as triples, referring to the vertices of each triangle. For lines, the index array is in pairs indicating the start and end of each line.

- **ARRAY_MAX** = **9**

.. _enum_ArrayMesh_ArrayFormat:

.. _class_ArrayMesh_constant_ARRAY_FORMAT_VERTEX:

.. _class_ArrayMesh_constant_ARRAY_FORMAT_NORMAL:

.. _class_ArrayMesh_constant_ARRAY_FORMAT_TANGENT:

.. _class_ArrayMesh_constant_ARRAY_FORMAT_COLOR:

.. _class_ArrayMesh_constant_ARRAY_FORMAT_TEX_UV:

.. _class_ArrayMesh_constant_ARRAY_FORMAT_TEX_UV2:

.. _class_ArrayMesh_constant_ARRAY_FORMAT_BONES:

.. _class_ArrayMesh_constant_ARRAY_FORMAT_WEIGHTS:

.. _class_ArrayMesh_constant_ARRAY_FORMAT_INDEX:

enum **ArrayFormat**:

- **ARRAY_FORMAT_VERTEX** = **1** --- Array format will include vertices (mandatory).

- **ARRAY_FORMAT_NORMAL** = **2** --- Array format will include normals

- **ARRAY_FORMAT_TANGENT** = **4** --- Array format will include tangents

- **ARRAY_FORMAT_COLOR** = **8** --- Array format will include a color array.

- **ARRAY_FORMAT_TEX_UV** = **16** --- Array format will include UVs.

- **ARRAY_FORMAT_TEX_UV2** = **32** --- Array format will include another set of UVs.

- **ARRAY_FORMAT_BONES** = **64** --- Array format will include bone indices.

- **ARRAY_FORMAT_WEIGHTS** = **128** --- Array format will include bone weights.

- **ARRAY_FORMAT_INDEX** = **256** --- Index array will be used.

Constants
---------

.. _class_ArrayMesh_constant_NO_INDEX_ARRAY:

.. _class_ArrayMesh_constant_ARRAY_WEIGHTS_SIZE:

- **NO_INDEX_ARRAY** = **-1** --- Default value used for index_array_len when no indices are present.

- **ARRAY_WEIGHTS_SIZE** = **4** --- Amount of weights/bone indices per vertex (always 4).

Description
-----------

The ``ArrayMesh`` is used to construct a :ref:`Mesh<class_Mesh>` by specifying the attributes as arrays. The most basic example is the creation of a single triangle

::

    var vertices = PoolVector3Array()
    vertices.push_back(Vector3(0, 1, 0))
    vertices.push_back(Vector3(1, 0, 0))
    vertices.push_back(Vector3(0, 0, 1))
    # Initialize the ArrayMesh.
    var arr_mesh = ArrayMesh.new()
    var arrays = []
    arrays.resize(ArrayMesh.ARRAY_MAX)
    arrays[ArrayMesh.ARRAY_VERTEX] = vertices
    # Create the Mesh.
    arr_mesh.add_surface_from_arrays(Mesh.PRIMITIVE_TRIANGLES, arrays)
    var m = MeshInstance.new()
    m.mesh = arr_mesh

The ``MeshInstance`` is ready to be added to the SceneTree to be shown.

Property Descriptions
---------------------

.. _class_ArrayMesh_property_blend_shape_mode:

- :ref:`BlendShapeMode<enum_Mesh_BlendShapeMode>` **blend_shape_mode**

+----------+-----------------------------+
| *Setter* | set_blend_shape_mode(value) |
+----------+-----------------------------+
| *Getter* | get_blend_shape_mode()      |
+----------+-----------------------------+

.. _class_ArrayMesh_property_custom_aabb:

- :ref:`AABB<class_AABB>` **custom_aabb**

+----------+------------------------+
| *Setter* | set_custom_aabb(value) |
+----------+------------------------+
| *Getter* | get_custom_aabb()      |
+----------+------------------------+

An overriding bounding box for this mesh.

Method Descriptions
-------------------

.. _class_ArrayMesh_method_add_blend_shape:

- void **add_blend_shape** **(** :ref:`String<class_String>` name **)**

.. _class_ArrayMesh_method_add_surface_from_arrays:

- void **add_surface_from_arrays** **(** :ref:`PrimitiveType<enum_Mesh_PrimitiveType>` primitive, :ref:`Array<class_Array>` arrays, :ref:`Array<class_Array>` blend_shapes=[  ], :ref:`int<class_int>` compress_flags=97280 **)**

Creates a new surface.

Surfaces are created to be rendered using a "primitive", which may be PRIMITIVE_POINTS, PRIMITIVE_LINES, PRIMITIVE_LINE_STRIP, PRIMITIVE_LINE_LOOP, PRIMITIVE_TRIANGLES, PRIMITIVE_TRIANGLE_STRIP, PRIMITIVE_TRIANGLE_FAN. See :ref:`Mesh<class_Mesh>` for details. (As a note, when using indices, it is recommended to only use points, lines or triangles). :ref:`Mesh.get_surface_count<class_Mesh_method_get_surface_count>` will become the ``surf_idx`` for this new surface.

The ``arrays`` argument is an array of arrays. See :ref:`ArrayType<enum_ArrayMesh_ArrayType>` for the values used in this array. For example, ``arrays[0]`` is the array of vertices. That first vertex sub-array is always required; the others are optional. Adding an index array puts this function into "index mode" where the vertex and other arrays become the sources of data and the index array defines the vertex order. All sub-arrays must have the same length as the vertex array or be empty, except for ``ARRAY_INDEX`` if it is used.

Adding an index array puts this function into "index mode" where the vertex and other arrays become the sources of data, and the index array defines the order of the vertices.

Godot uses clockwise winding order for front faces of triangle primitive modes.

.. _class_ArrayMesh_method_clear_blend_shapes:

- void **clear_blend_shapes** **(** **)**

Remove all blend shapes from this ``ArrayMesh``.

.. _class_ArrayMesh_method_get_blend_shape_count:

- :ref:`int<class_int>` **get_blend_shape_count** **(** **)** const

Returns the number of blend shapes that the ``ArrayMesh`` holds.

.. _class_ArrayMesh_method_get_blend_shape_name:

- :ref:`String<class_String>` **get_blend_shape_name** **(** :ref:`int<class_int>` index **)** const

Returns the name of the blend shape at this index.

.. _class_ArrayMesh_method_lightmap_unwrap:

- :ref:`Error<enum_@GlobalScope_Error>` **lightmap_unwrap** **(** :ref:`Transform<class_Transform>` transform, :ref:`float<class_float>` texel_size **)**

Will perform a UV unwrap on the ``ArrayMesh`` to prepare the mesh for lightmapping.

.. _class_ArrayMesh_method_regen_normalmaps:

- void **regen_normalmaps** **(** **)**

Will regenerate normal maps for the ``ArrayMesh``.

.. _class_ArrayMesh_method_surface_find_by_name:

- :ref:`int<class_int>` **surface_find_by_name** **(** :ref:`String<class_String>` name **)** const

Returns the index of the first surface with this name held within this ``ArrayMesh``. If none are found -1 is returned.

.. _class_ArrayMesh_method_surface_get_array_index_len:

- :ref:`int<class_int>` **surface_get_array_index_len** **(** :ref:`int<class_int>` surf_idx **)** const

Returns the length in indices of the index array in the requested surface (see :ref:`add_surface_from_arrays<class_ArrayMesh_method_add_surface_from_arrays>`).

.. _class_ArrayMesh_method_surface_get_array_len:

- :ref:`int<class_int>` **surface_get_array_len** **(** :ref:`int<class_int>` surf_idx **)** const

Returns the length in vertices of the vertex array in the requested surface (see :ref:`add_surface_from_arrays<class_ArrayMesh_method_add_surface_from_arrays>`).

.. _class_ArrayMesh_method_surface_get_format:

- :ref:`int<class_int>` **surface_get_format** **(** :ref:`int<class_int>` surf_idx **)** const

Returns the format mask of the requested surface (see :ref:`add_surface_from_arrays<class_ArrayMesh_method_add_surface_from_arrays>`).

.. _class_ArrayMesh_method_surface_get_name:

- :ref:`String<class_String>` **surface_get_name** **(** :ref:`int<class_int>` surf_idx **)** const

Get the name assigned to this surface.

.. _class_ArrayMesh_method_surface_get_primitive_type:

- :ref:`PrimitiveType<enum_Mesh_PrimitiveType>` **surface_get_primitive_type** **(** :ref:`int<class_int>` surf_idx **)** const

Returns the primitive type of the requested surface (see :ref:`add_surface_from_arrays<class_ArrayMesh_method_add_surface_from_arrays>`).

.. _class_ArrayMesh_method_surface_remove:

- void **surface_remove** **(** :ref:`int<class_int>` surf_idx **)**

Remove a surface at position surf_idx, shifting greater surfaces one surf_idx slot down.

.. _class_ArrayMesh_method_surface_set_name:

- void **surface_set_name** **(** :ref:`int<class_int>` surf_idx, :ref:`String<class_String>` name **)**

Set a name for a given surface.

.. _class_ArrayMesh_method_surface_update_region:

- void **surface_update_region** **(** :ref:`int<class_int>` surf_idx, :ref:`int<class_int>` offset, :ref:`PoolByteArray<class_PoolByteArray>` data **)**

