# tree-diff
Experiments showing (taxonomic) tree diffs.

The GBIF Checklist Bank and backbone tools can dump datasets in simple hierarchical text files or create an xml representation. 

## Tree text files
Tree text files simply list all names in a taxonomic order, sorting all children and synonyms by their rank and then name string.
In addition to the name itself the tree provides a few other properties per name:
 - the rank is given in brackets after the name
 - synonym names are prefixed with a ***
 - basionyms are prefixed with a *$*

```
Mantodea [order]
  Hymenopodidae [family]
    Amphecostephanus [genus]
      Amphecostephanus rex [species]
    Galinthias [genus]
      Galinthias amoena [species]
        *Galinthias hyalina [species]
      $Galinthias meruensis [species]
        *Galinthias usambarica [species]
        *Oxypilus meruensis [species]
        *Oxypilus nigericus [species]
      Galinthias occidentalis [species]
```

The text files can either use simple canonical names (default) or names with the full authorship indicated by filenames containing **-full**.

## Tree xml files
tbd
