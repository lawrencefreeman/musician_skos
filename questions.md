**`owl:sameAs` for linking OWL individuals to SKOS concepts**

I link my OWL role individuals (e.g. `mus:Instrumentalist`) to SKOS concepts (e.g. `muv:instrumentalist`) via `owl:sameAs`. 
What would be the best way to do this?

**Individuals with `subRoleOf` vs. subclasses**

I model my role hierarchy as individuals connected by a transitive `mus:subRoleOf` property, which should mirror `skos:broader`. 
The alternative would be OWL classes with `rdfs:subClassOf`, which would enable type-based inference (Guitarist automatically implies Instrumentalist).
Which approach is preferred here?

**SKOS triples inside the ontology file**

I included the `muv:` SKOS definitions (prefLabel, narrower, exactMatch etc.) directly in the same Turtle file as my OWL ontology.
Should I keep the SKOS vocabulary in a separate file for cleaner separation of concerns? 
If so, how to reference it?
