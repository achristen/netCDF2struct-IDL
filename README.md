# netCDF2struct-IDL

IDL code to read the entire content of any netCDF file directly into an IDL structure. It reads variables, parameter attributes and global attributes from
ncdf-files into a single idl-structure. Dimension-names are not retreived. The netCDF format is described here:

## netCDF2struct.pro

This program reads the entire content of any netCDF file directly into an IDL structure

calling sequence:

    ubc_fil_ncdf2struct, ncdf_file

input:

* ncdf_file : string. full filepath of ncdf file.

## struct2netCFF.pro

This program writes a IDL structure into a (limited) netCDF file.
