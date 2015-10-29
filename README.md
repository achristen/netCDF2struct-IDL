# netCDF2struct-IDL

IDL code to read the entire content of any netCDF file directly into an IDL structure or write an IDL structure into a netCDF file. It reads variables, parameter attributes and global attributes from ncdf-files into the structure. Dimension-names are not retreived.

The netCDF format is described here:

http://www.unidata.ucar.edu/software/netcdf/docs/

## ncdf2struct.pro

This program reads the entire content of any netCDF file directly into an IDL structure

calling sequence:

    data = ncdf2struct(ncdf_file)

"ncdf_file" [input]. string. full filepath of ncdf file to be read.

"data" [output]. structure. the returned structure that contains the netCDF's content.

## struct2ncdf.pro

This program writes an IDL structure into a (limited) netCDF file. The output can handle most file formats, but cannot handle string arrays. The string tags are translated into variable names in the netCDF.

calling sequence:

    struct2ncdf, ncdf_file, data

"ncdf_file" [input]. string. full filepath of ncdf file to be written.

"data" [input]. structure. the structure that is to be written into the netCDF.
