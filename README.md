# pgcdemtools
Tools for indexing, shelving, copying, and modifying SETSM and ASP dems

## Download
Version `1.0` released 11 Oct 2017.

#### [Download Latest](https://github.com/PolarGeospatialCenter/pgcdemtools/releases)

## Tools
### Rename
rename_setsm_add_version

### Index
index_setsm - Build a gdb or shapefile index of a single SETSM DEM or a directory of DEMs.

index_setsm_tiles - Build a gdb or shapefile index of a SETSM DEM mosaic tile or a directory of tiles.

### Package
package_setsm - Build an index of a SETSM DEM or directory of DEMs and package all auxilary files into tar.gz archives.

package_setsm_tiles - Build an index of a SETSM DEM mosaic tiles or directory of tiles and package all auxilary files into tar.gz archives.

### Shelve
shelve_setsm_by_date - Move or copy a SETSM DEM or a directory of DEMs into folders based on acquisition date.

shelve_setsm_by_geocell - Move or copy a SETSM DEM or a directory of DEMs into folders based on the geocell that intersects with the DEM cetroid, as identified by the lower left geocell corner.

shelve_setsm_by_shp - Move or copy a SETSM DEM or a directory of DEMs into folders based on a custon shapefile index.

### Retrieve
copy_dems - Copy DEMs using a subset of the DEM index bult using index_setsm.py.

### Misc
apply_setsm_registration - If GCP registration information is included with a SETSM DEM, apply the offset and output a new raster.

resample_setsm - resample SETSM DEMs to a lower resolution.

divide_setsm_tiles - Divide SETSM DEM mosaic tiles into subtiles.

## Usage notes
Some of the tools are designed to be run either in a serial, parallel, or with a PBS scheduler.  If a PBS scheduler is present, the --pbs option can often be used to submit the jobs to PBS.  The qsub* scripts can be modified or used as a template for job submission scripts. The --parallel-processes option, if available, allows the given tool to operate on several tasks at once.

## Contact
Claire Porter

[Polar Geospatial Center](//www.pgc.umn.edu)

Email: <porte254@umn.edu>
