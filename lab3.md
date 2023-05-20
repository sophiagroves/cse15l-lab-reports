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
**grep -v finds and returns all lines that do not contain the given string. This is useful for wanting to find information that does not talk about or include a specific phrase.** 

## command line option 2: ls | grep 
source: https://en.wikibooks.org/wiki/Grep

- *example 1:*

```
14088@DESKTOP-FOGPOI2 MINGW64 ~/Downloads/docsearch-main/technical/biomed
$ ls | grep 99
1471-2199-2-1.txt
1471-2199-2-10.txt
1471-2199-2-12.txt
1471-2199-2-2.txt 
1471-2199-2-3.txt 
1471-2199-2-4.txt 
1471-2199-2-5.txt 
1471-2199-2-6.txt 
1471-2199-3-10.txt
1471-2199-3-11.txt
1471-2199-3-12.txt
1471-2199-3-17.txt
1471-2199-3-3.txt 
1471-2199-3-7.txt 
1471-2199-4-4.txt 
1471-2199-4-5.txt 
ar799.txt
cc991.txt
```

- *examples 2:* 

```
14088@DESKTOP-FOGPOI2 MINGW64 ~/Downloads/docsearch-main/technical/government/About_LSC
$ ls | grep "Legal"
LegalServCorp_v_VelazquezDissent.txt 
LegalServCorp_v_VelazquezOpinion.txt 
LegalServCorp_v_VelazquezSyllabus.txt
```
**ls | grep finds all files within the current directory that have the given string in their name. This is useful for quickly filtering and finding specificic files in directories that are too large to manually look through efficiently.
