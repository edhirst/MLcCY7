# MLcCY7
Repository for generation of Calabi-Yau links from wp4 spaces, computation of their topological properties (Sasakian Hodge numbers, CN invariant), and their ML.

The `Data` folder lists the 7555 weights which create wp4 spaces which admit CY3 hypersurfaces in file `WP4s.txt` (the respective CY Hodge numbers $(h^{1,1},h^{2,1})$ are listed in `WP4_Hodges.txt`). CY polynomials (with the required singularity structure to create a CY link) are given in `CYPolynomials.txt`, as well as the respective topological invariant data in the file `Topological_Data.txt` listing each weight system, CY polynomial, Sasakian Hodge numbers, CN invariant, then Groebner basis length respectively. A selection of Groebner bases are given explicitly in the zipped file also.    

The `CY3PolynomialGeneration.sage` script details how the CY3s where generated, ensuring the correct singularity structure. The `CYLinkInvariantComputation.sage` script details how the respective topological invariants were computed (code is parallelised for efficiency). The `wREquivalenceChecks.sage` script contains general functionality for statistically verifying the weak R-Equivalence conjecture across the database.        

The remaining scripts perform the respective ML investigations as detailed in the paper.       

# BibTeX Citation
``` 
@article{Aggarwal:2023swe,
    author = "Aggarwal, Daattavya and He, Yang-Hui and Heyes, Elli and Hirst, Edward and Earp, Henrique N. S\'a and Silva, Tom\'as S. R.",
    title = "{Machine learning Sasakian and G2 topology on contact Calabi-Yau 7-manifolds}",
    eprint = "2310.03064",
    archivePrefix = "arXiv",
    primaryClass = "math.DG",
    reportNumber = "QMUL-PH-23-14",
    doi = "10.1016/j.physletb.2024.138517",
    journal = "Phys. Lett. B",
    volume = "850",
    pages = "138517",
    year = "2024"
}
```
