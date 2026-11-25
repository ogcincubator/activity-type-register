# Activity Type Register

A register of generic activity types, implemented as a profile of the Registered Item Model: the activity type,
geoprocessing and machine learning profiles, and the generic activity types grouped into families.


The profiles in this register are implemented as classes of the Registered Item Model, which lives in a separate [register](https://ogcincubator.github.io/registered-item-model/). 
The intent for this register is to be the generic 'top level' register that federated registers can inherit from for specific activity profiles in the respective domains.
The generic activity types live under `https://w3id.org/ogc/ospd/activity-type/`; federated registers, such as the
[OSPD activity types register](https://ogcincubator.github.io/ospd-activity-types/), specialise them with `skos:broader`.


## Building Blocks

### `ogc.register.activity-types` — Activity Types Register Profile

**Type:** model

A profile of the Registered Item Model for governed activity type records in the acttype:ActivityType hierarchy, with related PROV object types and an optional plan.

### `ogc.register.generic.core` — Generic Activity Types

**Type:** model

The catalog of the generic activity types: one concept scheme per family of related types, under https://w3id.org/ogc/ospd/activity-type/.

### `ogc.register.geoprocessing-activity-types` — Geoprocessing Activity Types Profile

**Type:** model

A profile of the Activity Type Register Profile for geoprocessing activity types: registered sub-classes of geoproc:GeoprocessingActivityType, each required to use or generate at least one GeoSPARQL spatial data type.

### `ogc.register.generic.earth-observation` — Earth observation

**Type:** model

Earth-observation data access and applications: Sentinel-2 band retrieval and product selection, cloud and best-available-pixel handling, and the water-bodies, algae-bloom and mangrove-biomass workflows.

### `ogc.register.generic.information-extraction-and-retrieval` — Information extraction and retrieval

**Type:** model

Source acquisition, text metadata enrichment (entity extraction, geotagging, classification, normalization) and retrieval-augmented generation.

### `ogc.register.generic.ml-and-statistical-modeling` — Machine learning and statistical modeling

**Type:** model

Machine-learning and statistical activities: regression, climate-variable downscaling, super-resolution and trend analysis, and inference executions.

### `ogc.register.generic.point-cloud-processing` — Point-cloud processing

**Type:** model

Point-cloud thinning, gridding and conversion to shapes.

### `ogc.register.generic.raster-coverage-processing` — Raster and coverage processing

**Type:** model

Operations on rasters and coverages: reprojection, resampling, cropping, mosaicking, format conversion, rendering, band math, spectral indices and zonal analysis.

### `ogc.register.generic.spatial-indexing` — Spatial indexing

**Type:** model

Discrete global grid system (DGGS) indexing and conversion of geometries to grid cells.

### `ogc.register.generic.terrain-and-hydrology` — Terrain and hydrology

**Type:** model

Terrain derivatives (slope, hillshading, ruggedness and position indices) and hydrological analysis (flow direction and accumulation, watersheds, stream networks, wetness index).

### `ogc.register.generic.vector-geometry-processing` — Vector geometry processing

**Type:** model

Operations and tests on vector geometries: buffers, hulls, envelopes, set operations, spatial predicates and extents (including the SQL/MM implementations).

### `ogc.register.generic.workflow-and-scoring` — Workflow and scoring

**Type:** model

Workflow runs and scoring or classification activities used in the model-of-models and workflow examples.

### `ogc.register.st-ml-activity-types` — SpatioTemporal ML Activity Types Profile

**Type:** model

A profile of the SpatioTemporal Machine learning Activity Types Profile describing spatiotemporal machine learning training and inference runs, and registrable ML activity types, using the STAC MLM extension's task, framework/accelerator and input/output vocabulary.

### `ogc.register.schemas.activity-types-schema` — Activity Types Register Profile Schema

**Type:** schema

This is a schema representation of the ogc.register.activity-types model

### `ogc.register.schemas.geoprocessing-activity-types-schema` — Geoprocessing Activity Types Profile Schema

**Type:** schema

This is a schema representation of the ogc.register.geoprocessing-activity-types model

### `ogc.register.schemas.st-ml-activity-types-schema` — SpatioTemporal ML Activity Types Profile Schema

**Type:** schema

This is a schema representation of the ogc.register.st-ml-activity-types model

