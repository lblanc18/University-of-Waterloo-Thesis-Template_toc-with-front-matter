# University-of-Waterloo-Thesis-Template_toc-with-front-matter
UW thesis template with my updates to reference front matter in the toc and include a List of Abbreviations

TOC ENTRIES
-----------

Front matter content is added to toc using the following general format:

\addcontentsline{toc}{frontmatter}{\bigskip \newline TITLE \hfill}   

These lines can be commented out to remove the entry from the toc, 
Note that the command \phantomsection is added as appropriate so \hyperref links to the approriate page.


LIST OF ABBREVIATIONS
---------------------

The following package is used to generate a list of abbreviations

\usepackage[printonlyused, withpage]{acronym}   
  % printonlyused can be removed to print all abbreviations
  % withpage can be removed to remove page numbers from the List of Abbreviations (LoA)
  
Add acronyms into the LoA with the following command:
  \acro{short name}{long name}
  
Call acronyms throught document with:
  \ac{short name}