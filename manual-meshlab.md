<!--

@created at 2020-06-19

#
#
#
#
#
#
#
#
#
#

-->

# Contents

- [Contents](#contents)
- [Search](#search)
- [Datastructure](#datastructure)
- [IO](#io)
  - [Supported Export Formats](#supported-export-formats)
  - [Supported Import Formats](#supported-import-formats)

# Search

- Pre-Open Options

  ```bash
  /home/ftx/Documents/yangxl-2014-fe/[fork]-Graphics/meshlab/src/meshlab/mainwindow_RunTime.cpp
  ```

- ASC Mesh Loading

  ```bash
  /home/ftx/Documents/yangxl-2014-fe/[fork]-Graphics/meshlab/vcglib/wrap/io_trimesh/import_asc.h
  ```

# Datastructure

```C++
class CVertexO : public vcg::Vertex< MyUsedTypes, vcg::vertex::Coord3f, vcg::vertex::Normal3f, vcg::vertex::BitFlags>{};

class CMeshO   : public vcg::tri::TriMesh< std::vector<CVertexO>, std::vector<CFaceO>,std::vector<CEdgeO> >
class CMeshO    : public vcg::tri::TriMesh< vcg::vertex::vector_ocf<CVertexO>, vcg::face::vector_ocf<CFaceO> >

template < class Container0 = DummyContainer, class Container1 = DummyContainer,
           class Container2 = DummyContainer, class Container3 = DummyContainer, class Container4 = DummyContainer >
class TriMesh
        : public  MArity5<   BaseMeshTypeHolder<typename Container0::value_type::TypesPool>, Container0, Der ,Container1, Der, Container2, Der, Container3, Der, Container4, Der >

/home/ftx/Documents/yangxl-2014-fe/[fork]-Graphics/meshlab/vcglib/vcg/complex/base.h
    VertContainer vert;
    typedef CONTV   VertContainer;
    typedef std::vector< typename TYPESPOOL::VertexType > CONTV;
```

# IO

## Supported Export Formats

```bash
meshlab$ tree | grep -i export_
│   │   │   ├── export_xyz.h
│   │   │   ├── export_x3d.h
│   │   ├── filter_web_export_vmust
│   │   │   └── filter_web_export_vmust.pro
│   │   │   │   ├── export_rib.h
│   │   │   │   ├── export_svg.h
│   │   │   │   ├── export_rib.h
│   │   │   ├── export_m.h
        │   ├── export_dxf.h
        │   └── export_svg.h
        │   ├── export_ply.h
        │   ├── export_tet.h
        │   ├── export_ts.h
        │   ├── export_vtk.h
        │   ├── export_3ds.h
        │   ├── export_ctm.h
        │   ├── export_dae.h
        │   ├── export_dxf.h
        │   ├── export_fbx.h
        │   ├── export_field.h
        │   ├── export_gts.h
        │   ├── export_idtf.h
        │   ├── export_iv.h
        │   ├── export_obj.h
        │   ├── export_off.h
        │   ├── export_ply.h
        │   ├── export_smf.h
        │   ├── export_stl.h
        │   ├── export_u3d.h
        │   ├── export_vmi.h
        │   ├── export_vrml.h
```

## Supported Import Formats

```bash
tree | grep -i import_
│   │   │   ├── import_mesh.png
│   │   │   ├── import_3ds.h
│   │   │   ├── import_expe.h
│   │   │   ├── import_xyz.h
│   │   │   ├── import_x3d.h
│   │   │       │   ├── import_ocm_ply.h
│   │   │       │   ├── import_ply_to_ocme.h
    │   │   ├── trimesh_import_fbx
    │   │   │   ├── trimesh_import_fbx.cpp
    │   │   │   └── trimesh_import_fbx.pro
        │   ├── import_msh.h
        │   ├── import_ply.h
        │   ├── import_ts.h
        │   ├── import_asc.h
        │   ├── import_ctm.h
        │   ├── import_dae.h
        │   ├── import_fbx.h
        │   ├── import_field.h
        │   ├── import_gts.h
        │   ├── import_nvm.h
        │   ├── import_obj.h
        │   ├── import_off.h
        │   ├── import_out.h
        │   ├── import_ply.h
        │   ├── import_ptx.h
        │   ├── import_raw.h
        │   ├── import_smf.h
        │   ├── import_stl.h
        │   ├── import_vmi.h
```

<!--

- <div align="left"><img src="xxx" height="" width="640" /></div>

#
#
#
#
#
#
#
#
#
#

<details>
<summary>
</summary>
<br/>
</details>

-->
