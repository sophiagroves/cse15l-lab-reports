# lab report three

**my chosen command is grep** 

## command line option 1: grep -v
source: https://en.wikibooks.org/wiki/Grep

- *example 1:*
```
14088@DESKTOP-FOGPOI2 MINGW64 ~/Downloads/docsearch-main/technical/plos
$ grep -v "in" journal.pbio.0020100.txt 


        all cellular processes have to be tightly regulated. Some answers to my questions began to 
        epithelium.
        However, most of them have been found biochemically and their function has been elucidated 
        these questions, we need to move to experimentally accessible multicellular organisms, such
        as
        Drosophila , which offers virtually unlimited possibilities as a
        model system for the genetic and molecular analysis of biological processes.
        Drosophila oogenesis. These cells have a simple polarised
        cells.
        These experiments could be expanded to large-scale screens (St Johnston 2002), but this    
        recent reports (Kiger et al. 2003; Rogers et al. 2003) describe a complementary and        
        cytoskeletal function.
        pathways.
        focus must be to understand how all these molecular events and regulation cascades operate 
```
- *example 2:*
```
14088@DESKTOP-FOGPOI2 MINGW64 ~/Downloads/docsearch-main/technical/plos
$ grep -v "a" journal.pbio.0020001.txt 


        serious problems not only for the scientific community in the developing countries, but for


        2002).


        regions.
        In
        However, publishing in

        world.


        built.
```
**grep -v finds and returns all lines that do not have the given string. This is useful for wanting to find information that does not talk about or include a specific phrase.** 
