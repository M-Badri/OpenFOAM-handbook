# ANSYS Meshing to OpenFoam® 

OpenFoam® needs to read a mesh in ASCII format if it comes from another
program so to export a Fluent .msh file in ASCII format the shortest way
(from ANSYS meshing) is:

File → Option → Meshing → Export → Format of input file (.msh)

Choose ASCII and then you can easily extract the file in ASCII format by
exporting the mesh. After you have the file in the working directory,
the addressed command is

```console
fluentMeshToFoam \<fileName\>.msh
```

Remember that it is good practice check the boundary setting in
constant/polyMesh/boundary after a conversion