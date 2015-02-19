# EuroWordNetLemon
EuroWordNet lemon lexicons generated from the LMF versions of the Multilingual Central Repository (MCR) EuroWordNet lexicons created by the Euskal Herriko Unibertsitatea. IXA Taldea. It includes lexicons for Spanish, Catalan, Basque &amp; Galician.
 
The Catalan lexicon is linked to the Catalan Parole/Simple lemon lexicon.
Gloss and rgloss relations between synsets are not included.
For LexicalEntries and LexicalSenses, original ID's are encoded in dcterms:source and the URIs follow the pattern '../lemma-PoS'.
For Synsets and Translations original IDs are used in the URIs (.../ID). 
Synset rdfs:labels were generated as follows:

INSERT {?synset rdfs:label ?labels } 
WHERE
{SELECT ?synset (GROUP_CONCAT(?label; separator = '  ; ') as ?labels)
   {  ?sense  lemon:reference ?synset; rdfs:label ?label . }
   GROUP BY ?synset
}



 http://lodserver.iula.upf.edu/id/WordNetLemon/CAT/
 http://lodserver.iula.upf.edu/id/WordNetLemon/ES/
 http://lodserver.iula.upf.edu/id/WordNetLemon/EU/
 http://lodserver.iula.upf.edu/id/WordNetLemon/GL/
 
 
