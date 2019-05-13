OpenStreetMap for transport planning: a review of its uptake based on an analysis of academic publications and government reports
================
Robin Lovelace
2019-05-13

``` r
# get citations
refs = RefManageR::ReadZotero(group = "418217", .params = list(collection = "JFR868KJ", limit = 100))
RefManageR::WriteBib(refs, "software.bib")
```

    ## Writing 64 Bibtex entries ... OK
    ## Results written to file 'software.bib'

Abstract
--------

``` r
test = fulltext::ft_search(query = "transport planning", from = "crossref")
test = fulltext::ft_search(query = "transport planning", from = "arxiv")
test$arxiv$data
```

    ##                    id           submitted             updated
    ## 1  astro-ph/9204005v1 1992-04-30 19:18:05 1992-04-30 19:18:05
    ## 2    hep-ph/9206214v1 1992-06-10 21:35:55 1992-06-10 21:35:55
    ## 3    hep-ph/9207212v1 1992-07-03 21:05:00 1992-07-03 21:05:00
    ## 4    hep-ph/9207234v1 1992-07-10 23:15:00 1992-07-10 23:15:00
    ## 5  cond-mat/9207014v1 1992-07-15 12:01:03 1992-07-15 12:01:03
    ## 6  cond-mat/9207017v1 1992-07-15 21:25:36 1992-07-15 21:25:36
    ## 7  cond-mat/9207018v1 1992-07-15 21:41:54 1992-07-15 21:41:54
    ## 8  cond-mat/9207024v1 1992-07-20 17:04:03 1992-07-20 17:04:03
    ## 9    hep-ph/9207269v1 1992-07-29 23:03:09 1992-07-29 23:03:09
    ## 10 cond-mat/9208002v1 1992-08-05 17:47:00 1992-08-05 17:47:00
    ##                                                                                                                title
    ## 1                                                                             Radiation Transfer in Gamma-Ray Bursts
    ## 2                                           Debye Screening and Baryogenesis during the Electroweak Phase Transition
    ## 3                                                          Collider discovery limits for supersymmetric Higgs bosons
    ## 4                                                           The Neutralino Relic Density in Minimal N=1 Supergravity
    ## 5                                    Morphology of Amorphous Layers Ballistically Deposited on a Planar\n  Substrate
    ## 6                                  Transport Properties and Fluctuations in Type II Superconductors Near\n  $H_{c2}$
    ## 7  Vortex motion and the Hall effect in type II superconductors: a time\n  dependent Ginzburg-Landau theory approach
    ## 8                                    Zero Frequency Current Noise for the Double Tunnel Junction Coulomb\n  Blockade
    ## 9                                      New Higgs Signatures in Supersymmetry with Spontraneously Broken R\n  Parity"
    ## 10                                                    Transport Properties of the Infinite Dimensional Hubbard Model
    ##                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      abstract
    ## 1                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               We have calculated gamma-ray radiative transport in regions of high energy\ndensity, such as gamma-ray burst source regions, using a discrete ordinate,\ndiscrete energy group method. The calculations include two-photon pair\nproduction and annihilation, as well as three-photon pair annihilation. The\nradiation field itself acts as an absorbing medium, and the optical depth\ndepends on its intensity, so the problem is intrinsically nonlinear. Spherical\ndivergence produces effective collimation of the flux. At high optical depth\nthe high energy ($E > 1$ MeV) portion of the emergent spectrum assumes a nearly\nuniversal form. An approximate limit is derived for the high energy flux from a\ngamma-ray burst source region of given size, and the implications of this limit\nfor the distance to the March 5, 1979 event are briefly discussed. We discuss\nmore generally the problem of very luminous bursts, and implications of\nGalactic halo distances for flare models.\n
    ## 2                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 We examine a recent claim that Debye screening will affect the charge\ntransport mechanism of anomalous electroweak baryogenesis. We show that the\neffects of gauge charge screening do not affect the baryon number produced\nduring a first order electroweak phase transition. (Requires harvmac.tex)\n
    ## 3                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   The prospects for discovery of the five Higgs bosons of the minimal\nsupersymmetric standard model are assessed for existing and planned future\ncolliders, including LEP\\,I, LEP\\,II, LHC and SSC. As a benchmark for\ncomparisons, we take a top-quark mass $m_t= 150\\,$GeV and squark mass parameter\n$\\tilde m= 1\\,$TeV in evaluating one-loop radiative corrections; some results\nfor other $m_t$ values are also given. Searches based on the most promising\nproduction and decay channels are taken into account. For large regions in\nparameter space, detectable signals are predicted for one or more of the Higgs\nbosons, but there remains a region for which no signals would be visible at the\nabove colliders.\n
    ## 4    We compute the cosmic relic (dark matter) density of the lightest\nsupersymmetric particle (LSP) in the framework of minimal $N=1$ Supergravity\nmodels with radiative breaking of the electroweak gauge symmetry. To this end,\nwe re--calculate the cross sections for all possible annihilation processes for\na general, mixed neutralino state with arbitrary mass. Our analysis includes\neffects of all Yukawa couplings of third generation fermions, and allows for a\nfairly general set of soft SUSY breaking parameters at the Planck scale. We\nfind that a cosmologically interesting relic density emerges naturally over\nwide regions of parameter space. However, the requirement that relic\nneutralinos do not overclose the universe does not lead to upper bounds on SUSY\nbreaking parameters that are strictly valid for all combinations of parameters\nand of interest for existing or planned collider experiments; in particular,\ngluino and squark masses in excess of 5 TeV cannot strictly be excluded. On the\nother hand, in the ``generic'' case of a gaugino--like neutralino whose\nannihilation cross sections are not ``accidentally'' enhanced by a nearby Higgs\nor $Z$ pole, all sparticles should lie within the reach of the proposed $pp$\nand $e^+e^-$ supercolliders. We also find that requiring the LSP to provide all\ndark matter predicted by inflationary models imposes a strict lower bound of 40\nGeV on the common scalar mass $m$ at the Planck scale, while the lightest\nsleptons would have to be heavier\n
    ## 5                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              We report numerical simulation of the deposition of spherical particles on a\nplanar surface, by ballistic, straight-line trajectory transport, and assuming\nirreversible adhesion on contact with the surface or previously deposited\nparticles. Our data indicate that the deposit formed has a loosely layered\nstructure within few diameters from the surface. This structure can be\nexplained by a model of growth via chain formation. Away from the surface we\nfound evidence of a monotonic, power-law approach to the bulk density. Both\ndensity and contact-statistics results suggest that the deposit formed is\nsparse: the space-filling fraction is about 15%, and the average number of\ncontacts is 2. The morphology of the deposit both near the surface and in the\nbulk seems to be a result of competition of screening and branching; nearly\nhalf of all the spheres are either single-contact dangling ends, or branching\nnodes with more than two contacts.\n
    ## 6                                                                                                                                                                                                                                                                                                         We study the flux-flow Hall effect and thermomagnetic transport near the\nupper critical field \\hctwo\\ in extreme type-II superconductors starting from a\nsuitable generalization of the time dependent Ginzburg-Landau equations. We\nexplicitly incorporate the effects of backflow into the calculations of the\nlocal electric field and current, leading to a current which is properly\ndivergenceless. The Hall conductivity calculated from this current agrees with\nother mean-field calculations which assume a uniform applied electric field\n(the Schmid-Caroli-Maki solution), thereby vindicating these simplified\ntreatments. We then use these results to calculate the transverse\nthermomagnetic effects (the Ettingshausen and Nernst effects). The effects of\nthermal fluctuations and nonlocal elasticity of the flux lattice are\nincorporated using a method recently developed by Vecris and Pelcovits [G.\nVecris and R. A. Pelcovits, Phys. Rev. B {\\bf 44}, 2767 (1991)]. Our results,\ntaken together with those of Vecris and Pelcovits, provide a rather complete\ndescription of the transport properties of the flux lattice state near \\hctwo,\nat least within the framework of time dependent Ginzburg-Landau theory.\n
    ## 7                                                                                  Vortex motion in type II superconductors is studied starting from a variant\nof the time dependent Ginzburg-Landau equations, in which the order parameter\nrelaxation time is taken to be complex. Using a method due to Gor'kov and\nKopnin, we derive an equation of motion for a single vortex ($B\\ll H_{c2}$) in\nthe presence of an applied transport current. The imaginary part of the\nrelaxation time and the normal state Hall effect both break ``particle-hole\nsymmetry,'' and produce a component of the vortex velocity parallel to the\ntransport current, and consequently a Hall field due to the vortex motion.\nVarious models for the relaxation time are considered, allowing for a\ncomparison to some phenomenological models of vortex motion in superconductors,\nsuch as the Bardeen-Stephen and Nozi\\`eres-Vinen models, as well as to models\nof vortex motion in neutral superfluids. In addition, the transport energy,\nNernst effect, and thermopower are calculated for a single vortex. Vortex\nbending and fluctuations can also be included within this description,\nresulting in a Langevin equation description of the vortex motion. The Langevin\nequation is used to discuss the propagation of helicon waves and the\ndiffusional motion of a vortex line. The results are discussed in light of the\nrather puzzling sign change of the Hall effect which has been observed in the\nmixed state of the high temperature superconductors.\n
    ## 8                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    We compute the zero frequency current noise numerically and in several limits\nanalytically for the coulomb blockade problem consisting of two tunnel\njunctions connected in series. At low temperatures over a wide range of\nvoltages, capacitances, and resistances it is shown that the noise measures the\nvariance in the number of electrons in the region between the two tunnel\njunctions. The average current, on the other hand, only measures the mean\nnumber of electrons. Thus, the noise provides additional information about\ntransport in these devices which is not available from measuring the current\nalone.\n
    ## 9                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              Higgs production from $Z$ decay in supersymmetry with spontaneous broken R\nparity proceeds mostly by the Bjorken process as in the standard model.\nHowever, the corresponding production rates can be weaker than in the standard\nmodel (SM), especially in the low mass region. This will substantially weaken\nthe Higgs boson mass limits derived from LEP1. More strikingly, the main Higgs\ndecay channel is "invisible", over most of the mass range accessible to LEP1,\nleading to events with large missing energy carried by majorons. This\npossibility should be taken into account in the planning of Higgs boson search\nstrategies not only at LEP but also at high energy supercolliders.\n
    ## 10                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         Results for the optical conductivity and resistivity of the Hubbard model in\ninfinite spatial dimensions are presented. At half filling we observe a gradual\ncrossover from a normal Fermi-liquid with a Drude peak at $\\omega=0$ in the\noptical conductivity to an insulator as a function of $U$ for temperatures\nabove the antiferromagnetic phase transition. When doped, the ``insulator''\nbecomes a Fermi-liquid with a corresponding temperature dependence of the\noptical conductivity and resistivity. We find a $T^2$-coefficient in the low\ntemperature resistivity which suggests that the carriers in the system acquire\na considerable mass-enhancement due to the strong local correlations. At high\ntemperatures, a crossover into a semi-metallic regime takes place.\n
    ##                                                                                  authors
    ## 1                                                              B. J. Carrigan|J. I. Katz
    ## 2                                                  A. G. Cohen|D. B. Kaplan|A. E. Nelson
    ## 3                                V. Barger|Kingman Cheung|R. J. N. Phillips|A. L. Stange
    ## 4                                                                  M. Drees|M. M. Nojiri
    ## 5                                                 B. D. Lubachevsky|V. Privman|S. C. Roy
    ## 6                                                          Robert J. Troy|Alan T. Dorsey
    ## 7                                                                         Alan T. Dorsey
    ## 8  Selman Hershfield|John H. Davies|Per Hyldgaard|Christopher J. Stanton|John W. Wilkins
    ## 9                                                        J Romao|F de Campos|J W F Valle
    ## 10                                                     Th. Pruschke|D. L. Cox|M. Jarrell
    ##    affiliations                           link_abstract
    ## 1               http://arxiv.org/abs/astro-ph/9204005v1
    ## 2                 http://arxiv.org/abs/hep-ph/9206214v1
    ## 3                 http://arxiv.org/abs/hep-ph/9207212v1
    ## 4                 http://arxiv.org/abs/hep-ph/9207234v1
    ## 5               http://arxiv.org/abs/cond-mat/9207014v1
    ## 6               http://arxiv.org/abs/cond-mat/9207017v1
    ## 7               http://arxiv.org/abs/cond-mat/9207018v1
    ## 8               http://arxiv.org/abs/cond-mat/9207024v1
    ## 9                 http://arxiv.org/abs/hep-ph/9207269v1
    ## 10              http://arxiv.org/abs/cond-mat/9208002v1
    ##                                   link_pdf
    ## 1  http://arxiv.org/pdf/astro-ph/9204005v1
    ## 2    http://arxiv.org/pdf/hep-ph/9206214v1
    ## 3    http://arxiv.org/pdf/hep-ph/9207212v1
    ## 4    http://arxiv.org/pdf/hep-ph/9207234v1
    ## 5  http://arxiv.org/pdf/cond-mat/9207014v1
    ## 6  http://arxiv.org/pdf/cond-mat/9207017v1
    ## 7  http://arxiv.org/pdf/cond-mat/9207018v1
    ## 8  http://arxiv.org/pdf/cond-mat/9207024v1
    ## 9    http://arxiv.org/pdf/hep-ph/9207269v1
    ## 10 http://arxiv.org/pdf/cond-mat/9208002v1
    ##                                          link_doi
    ## 1                http://dx.doi.org/10.1086/171906
    ## 2  http://dx.doi.org/10.1016/0370-2693(92)91640-U
    ## 3      http://dx.doi.org/10.1103/PhysRevD.46.4914
    ## 4       http://dx.doi.org/10.1103/PhysRevD.47.376
    ## 5        http://dx.doi.org/10.1103/PhysRevE.47.48
    ## 6      http://dx.doi.org/10.1103/PhysRevB.47.2715
    ## 7      http://dx.doi.org/10.1103/PhysRevB.46.8376
    ## 8      http://dx.doi.org/10.1103/PhysRevB.47.1967
    ## 9  http://dx.doi.org/10.1016/0370-2693(92)91183-A
    ## 10   http://dx.doi.org/10.1209/0295-5075/21/5/015
    ##                                                                                                                                              comment
    ## 1                                                                                                                                           24 pages
    ## 2                                                                                                             12 pages, UCSD-PTH-92-19, BU-HEP-92-20
    ## 3                                                                                   24 pages, 23 postscript figures available on request. MAD/PH/696
    ## 4                                                                        53 pages(8figs are not included), Latex file; DESY 92-101,\n  SLAC-PUB-5860
    ## 5                                                                                                                              20 pages, TeX (plain)
    ## 6                                                                                                                   27 pages (no figures); in REVTEX
    ## 7  to be published in Phys. Rev. B; 47 pages, 1 figure (available upon\n  request); uses jnl.tex along with the macros reforder.tex and eqnorder.tex
    ## 8                                                                                                                               33 pages, 10 figures
    ## 9                                                                                      14 pages, 2 Figures, latex, uses macro matex, CERN TH.6586/92
    ## 10                                                                                                                                          14 pages
    ##                        journal_ref                          doi
    ## 1  Astrophys.J. 399 (1992) 100-107               10.1086/171906
    ## 2     Phys.Lett. B294 (1992) 57-62 10.1016/0370-2693(92)91640-U
    ## 3      Phys.Rev.D46:4914-4929,1992     10.1103/PhysRevD.46.4914
    ## 4        Phys.Rev.D47:376-408,1993      10.1103/PhysRevD.47.376
    ## 5          Phys.Rev.E47:48-53,1993       10.1103/PhysRevE.47.48
    ## 6                                      10.1103/PhysRevB.47.2715
    ## 7      Phys.Rev.B46:8376-8392,1992     10.1103/PhysRevB.46.8376
    ## 8                                      10.1103/PhysRevB.47.1967
    ## 9      Phys.Lett.B292:329-336,1992 10.1016/0370-2693(92)91183-A
    ## 10                                   10.1209/0295-5075/21/5/015
    ##    primary_category categories
    ## 1          astro-ph   astro-ph
    ## 2            hep-ph     hep-ph
    ## 3            hep-ph     hep-ph
    ## 4            hep-ph     hep-ph
    ## 5          cond-mat   cond-mat
    ## 6          cond-mat   cond-mat
    ## 7          cond-mat   cond-mat
    ## 8          cond-mat   cond-mat
    ## 9            hep-ph     hep-ph
    ## 10         cond-mat   cond-mat
