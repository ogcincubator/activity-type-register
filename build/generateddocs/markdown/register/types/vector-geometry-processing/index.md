
# Vector geometry processing (Model)

`ogc.register.types.vector-geometry-processing` *v0.1*

Operations and tests on vector geometries: buffers, hulls, envelopes, set operations, spatial predicates and extents (including the SQL/MM implementations).

[*Status*](http://www.opengis.net/def/status): Under development

## Description

# Vector geometry processing

Operations and tests on vector geometries: buffers, hulls, envelopes, set operations, spatial predicates and extents (including the SQL/MM implementations).

This family has 25 generic activity types. It is a profile of the Generic Activity Types block and its data resource
(`data.ttl`) is uploaded to the OSPD Prez instance when the register is built.

## Activity types

- [Area](https://w3id.org/ogc/ospd/activity-type/area) (`area`)
- [Boundary](https://w3id.org/ogc/ospd/activity-type/GA002) (`GA002`)
- [Bounding Circle](https://w3id.org/ogc/ospd/activity-type/GA004) (`GA004`)
- [Buffer](https://w3id.org/ogc/ospd/activity-type/GA001) (`GA001`)
- [Buffer](https://w3id.org/ogc/ospd/activity-type/buffer) (`buffer`)
- [Centroid](https://w3id.org/ogc/ospd/activity-type/centroid) (`centroid`)
- [Concave Hull](https://w3id.org/ogc/ospd/activity-type/GA005) (`GA005`)
- [Contains](https://w3id.org/ogc/ospd/activity-type/contains) (`contains`)
- [Convex Hull](https://w3id.org/ogc/ospd/activity-type/GA006) (`GA006`)
- [Convex hull](https://w3id.org/ogc/ospd/activity-type/convex-hull) (`convex-hull`)
- [Crosses](https://w3id.org/ogc/ospd/activity-type/crosses) (`crosses`)
- [Difference](https://w3id.org/ogc/ospd/activity-type/GA019) (`GA019`)
- [Difference](https://w3id.org/ogc/ospd/activity-type/difference) (`difference`)
- [Disjoint](https://w3id.org/ogc/ospd/activity-type/disjoint) (`disjoint`)
- [Envelope](https://w3id.org/ogc/ospd/activity-type/GA003) (`GA003`)
- [Equals](https://w3id.org/ogc/ospd/activity-type/equals) (`equals`)
- [Filter geometries](https://w3id.org/ogc/ospd/activity-type/GA020) (`GA020`)
- [Geometry extent](https://w3id.org/ogc/ospd/activity-type/geometry-extent) (`geometry-extent`)
- [Intersection](https://w3id.org/ogc/ospd/activity-type/intersection) (`intersection`)
- [Intersects](https://w3id.org/ogc/ospd/activity-type/intersects) (`intersects`)
- [Is simple](https://w3id.org/ogc/ospd/activity-type/is-simple) (`is-simple`)
- [Symmetric difference](https://w3id.org/ogc/ospd/activity-type/symdifference) (`symdifference`)
- [Touches](https://w3id.org/ogc/ospd/activity-type/touches) (`touches`)
- [Union](https://w3id.org/ogc/ospd/activity-type/union) (`union`)
- [Within](https://w3id.org/ogc/ospd/activity-type/within) (`within`)

## Examples

### Area
#### turtle
```turtle
@prefix acttype: <https://w3id.org/ogc/rim/activity-type/> .
@prefix dcterms: <http://purl.org/dc/terms/> .
@prefix ospd: <https://w3id.org/ogc/ospd/activity-type/> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix rim: <https://w3id.org/ogc/rim/> .
@prefix skos: <http://www.w3.org/2004/02/skos/core#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

ospd:area a skos:Concept,
        acttype:ActivityType ;
    dcterms:replaces <https://w3id.org/geolabs/ospd/generic-profiles/activity-type/area> ;
    dcterms:source [ ],
        [ ] ;
    rdfs:subClassOf <https://w3id.org/ogc/rim/geoprocessing/GeoprocessingActivityType> ;
    skos:definition "The area of this Surface, as measured in the spatial reference system of this Surface."@en ;
    skos:inScheme <https://w3id.org/ogc/ospd/activity-type/families/vector-geometry-processing> ;
    skos:prefLabel "Area"@en ;
    skos:topConceptOf <https://w3id.org/ogc/ospd/activity-type/families/vector-geometry-processing> ;
    rim:itemClass acttype:activityTypeItemClass ;
    rim:objectIdentifier "https://w3id.org/ogc/ospd/activity-type/area"^^xsd:anyURI ;
    rim:publicationStatus rim:published ;
    rim:validityStatus rim:valid .

<https://w3id.org/ogc/ospd/activity-type/families/vector-geometry-processing> a skos:ConceptScheme .

```


# For developers

The source code for this Building Block can be found in the following repository:

* URL: [https://github.com/ogcincubator/activity-type-register](https://github.com/ogcincubator/activity-type-register)
* Path: `_sources/types/vector-geometry-processing`

