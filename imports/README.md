# EXTRACTION SCRIPTS

The following commands were used with OBO ROBOT to generate the files and then later merged to produce (>robot [merge](http://robot.obolibrary.org/merge.html)...)

## Human Ancestry Ontology
```
robot extract --method MIREOT --input "hancestro_inferred.owl" --branch-from-term "GEO:000000374" --branch-from-term "HANCESTRO:0003" --branch-from-term "HANCESTRO:0002" --copy-ontology-annotations true --output hancestro-extraction.owl
```

## Population and Community Ontology
```
robot extract --method MIREOT --input "pco.owl" --upper-term "BFO:0000001" --lower-term "ENVO:01000744" --lower-term "PCO:0000030" --lower-term "PATO:0000001" --branch-from-term "PATO:0000001" --lower-term "GO:0035176" --branch-from-term "GO:0035176" --branch-from-term "PCO:0000033" --branch-from-term "PCO:0000005" --lower-term "PCO:1000002" --lower-term "PCO:0000032" --lower-term "PCO:1000003" --intermediates all --copy-ontology-annotations true --output pco-terms.owl
```

## Ontology of Medically Related Social Entities
```
robot extract --method MIREOT --input "omrse.owl" --upper-term "BFO:0000001" --lower-term "OOSTT:00000074" --branch-from-term "OOSTT:00000074" --lower-term "OMRSE:00000204" --branch-from-term "OMRSE:00000204" --lower-term "OMRSE:00000195" --lower-term "OMRSE:00000076" --lower-term "OMRSE:00000062" --branch-from-term "OMRSE:00000062" --lower-term "OMRSE:00000033" --lower-term "OBI:0000245" --branch-from-term "OBI:0000245" --lower-term "IAO:0000310" --branch-from-term "IAO:0000310" --lower-term "OMRSE:00000142" --lower-term "OMRSE:00002060" --lower-term "BFO:0000034" --branch-from-term "BFO:0000034" --lower-term "BFO:0000023" --branch-from-term "BFO:0000023" --lower-term "OMRSE:00002068" --branch-from-term "OMRSE:00002068" --lower-term "BFO:0000182" --lower-term "IAO:0021003" --branch-from-term "IAO:0021003" --lower-term "OAE:0000002" --branch-from-term "OAE:0000002" --lower-term "RO:0002577" --intermediates all --copy-ontology-annotations true --output omrse-terms.owl
```

## Relation Ontology (base)
```
robot extract --method MIREOT --input "ro-base.owl" --upper-term "RO:0002410" --branch-from-term "RO:0003302" --branch-from-term "RO:0002244" --branch-from-term "RO:0004023" --branch-from-term "RO:0002501" --branch-from-term "RO_0002506" --branch-from-term "RO:0002595" --upper-term "RO:0002610" --lower-term "RO:0003308" --lower-term "RO:0002607" --upper-term "RO:0002222" --branch-from-term "BFO:0000063" --branch-from-term "BFO:0000062"  --intermediates all --copy-ontology-annotations true --output ro-terms-test.owl 
```
