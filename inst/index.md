::: {.cell layout-align="center"}

:::



Local preview

# Welcome {-}

This is the landing page of the `BiocBook` entitled *...*.  

This book introduces the reader to *...*.  

# Docker image {-}

A `Docker` image built from this repository is available here: 

👉 [ghcr.io/bschilder/bbreprex](https://ghcr.io/bschilder/bbreprex) 🐳

::: {.callout-tip icon='true'}
## Get started now 🎉

You can get access to all the packages used in this book in < 1 minute, 
using this command in a terminal: 



::: {.cell layout-align="center" filename='bash'}

```{.sh .cell-code}
docker run -it ghcr.io/bschilder/bbreprex:devel R
```
:::



:::

# RStudio Server {-}

An RStudio Server instance can be initiated from the `Docker` image as follows: 



::: {.cell layout-align="center" filename='bash'}

```{.sh .cell-code}
docker run \
    --volume <local_folder>:<destination_folder> \
    -e PASSWORD=OHCA \
    -p 8787:8787 \
    ghcr.io/bschilder/bbreprex:devel
```
:::



The initiated RStudio Server instance will be available at 
[https://localhost:8787](https://localhost:8787).

<!-- 
# System dependencies and conda 

A pre-configured `micromamba` environment called `BiocBook` is available 
once the Docker image is loaded. It provides all the softwares listed in 
`requirements.yml`. 



::: {.cell layout-align="center" filename='bash'}

```{.sh .cell-code}
docker run -it ghcr.io/bschilder/bbreprex:devel bash
micromamba activate BiocBook
```
:::


-->

# Session info {-}

::: {.callout-note collapse="true"}

## Click to expand 👇



::: {.cell layout-align="center"}

```{.r .cell-code}
sessioninfo::session_info(
    installed.packages()[,"Package"], 
    include_base = TRUE
)
##  ─ Session info ────────────────────────────────────────────────────────────
##   setting  value
##   version  R version 4.3.1 (2023-06-16)
##   os       macOS Sonoma 14.3.1
##   system   aarch64, darwin20
##   ui       X11
##   language (EN)
##   collate  en_US.UTF-8
##   ctype    en_US.UTF-8
##   tz       Europe/London
##   date     2024-03-18
##   pandoc   3.1.3 @ /Users/bms20/anaconda3/envs/pytorch/bin/ (via rmarkdown)
##  
##  ─ Packages ────────────────────────────────────────────────────────────────
##   ! package                            * version        date (UTC) lib source
##     abind                                1.4-5          2016-07-21 [1] CRAN (R 4.3.0)
##     ade4                                 1.7-22         2023-02-06 [1] CRAN (R 4.3.0)
##     adegenet                             2.1.10         2023-01-26 [1] CRAN (R 4.3.0)
##     adephylo                             1.1-16         2023-10-06 [1] CRAN (R 4.3.1)
##     ADImpute                             1.12.0         2023-10-26 [1] Bioconductor
##     ADMM                                 0.3.3          2021-08-08 [1] CRAN (R 4.3.0)
##     afex                                 1.3-1          2024-02-25 [1] CRAN (R 4.3.1)
##     alphavantager                        0.1.3          2023-03-31 [1] CRAN (R 4.3.0)
##     anndata                              0.7.5.6        2023-03-17 [1] CRAN (R 4.3.0)
##     anndataR                             0.99.0         2023-12-05 [1] Bioconductor
##     annotate                             1.80.0         2023-10-26 [1] Bioconductor
##     AnnotationDbi                        1.64.1         2023-11-02 [1] Bioconductor
##     AnnotationFilter                     1.26.0         2023-10-26 [1] Bioconductor
##     AnnotationHub                        3.10.0         2023-10-26 [1] Bioconductor
##     anytime                              0.3.9          2020-08-27 [1] CRAN (R 4.3.0)
##     aod                                  1.3.3          2023-12-13 [1] CRAN (R 4.3.1)
##     ape                                  5.7-1          2023-03-13 [1] CRAN (R 4.3.0)
##     aplot                                0.2.2          2023-10-06 [1] CRAN (R 4.3.1)
##     ArchR                                1.0.2          2023-11-17 [1] Github (GreenleafLab/ArchR@c61b064)
##     arrow                                14.0.0.2       2023-12-02 [1] CRAN (R 4.3.1)
##     arules                               1.7-7          2023-11-29 [1] CRAN (R 4.3.1)
##     AsioHeaders                          1.22.1-2       2022-12-08 [1] CRAN (R 4.3.0)
##     askpass                              1.2.0          2023-09-03 [1] CRAN (R 4.3.0)
##     assertthat                           0.2.1          2019-03-21 [1] CRAN (R 4.3.0)
##     attempt                              0.3.1          2020-05-03 [1] CRAN (R 4.3.0)
##     autoCV                               0.99.1         2023-11-14 [1] local
##     av                                   0.9.0          2023-12-05 [1] CRAN (R 4.3.1)
##     available                            1.1.0          2022-07-10 [1] CRAN (R 4.3.0)
##     aws.s3                               0.3.21         2020-04-07 [1] CRAN (R 4.3.0)
##     aws.signature                        0.6.0          2020-06-01 [1] CRAN (R 4.3.0)
##     babelgene                            22.9           2022-09-29 [1] CRAN (R 4.3.0)
##     backports                            1.4.1          2021-12-13 [1] CRAN (R 4.3.0)
##     badger                               0.2.3          2023-01-28 [1] CRAN (R 4.3.0)
##     bamsignals                           1.34.0         2023-10-26 [1] Bioconductor
##     base                               * 4.3.1          2023-06-16 [?] local
##     base64enc                            0.1-3          2015-07-28 [1] CRAN (R 4.3.0)
##     base64url                            1.4            2018-05-14 [1] CRAN (R 4.3.0)
##     basilisk                             1.14.3         2024-01-30 [1] Bioconductor 3.18 (R 4.3.2)
##     basilisk.utils                       1.14.1         2023-11-20 [1] Bioconductor 3.18 (R 4.3.1)
##     batchelor                            1.18.1         2023-12-30 [1] Bioconductor 3.18 (R 4.3.2)
##     BayesFactor                          0.9.12-4.7     2024-01-24 [1] CRAN (R 4.3.1)
##     bayestestR                           0.13.2         2024-02-12 [1] CRAN (R 4.3.1)
##     beachmat                             2.18.1         2024-02-17 [1] Bioconductor 3.18 (R 4.3.2)
##     beeswarm                             0.4.0          2021-06-01 [1] CRAN (R 4.3.0)
##     BH                                   1.84.0-0       2024-01-10 [1] CRAN (R 4.3.1)
##     bibliometrix                         4.1.4          2023-11-28 [1] CRAN (R 4.3.1)
##     bibliometrixData                     0.3.0          2022-04-20 [1] CRAN (R 4.3.0)
##     bigassertr                           0.1.6          2023-01-10 [1] CRAN (R 4.3.0)
##     biglm                                0.9-2.1        2020-11-27 [1] CRAN (R 4.3.0)
##     bigparallelr                         0.3.2          2021-10-02 [1] CRAN (R 4.3.0)
##     bigreadr                             0.2.5          2022-12-06 [1] CRAN (R 4.3.0)
##     bigstatsr                            1.5.12         2022-10-14 [1] CRAN (R 4.3.0)
##     Biobase                              2.62.0         2023-10-26 [1] Bioconductor
##     BiocBaseUtils                        1.4.0          2023-10-26 [1] Bioconductor
##     biocBiocypher                        0.0.2          2023-12-10 [1] Github (vjcitn/biocBiocypher@246c655)
##     BiocBook                             1.0.0          2023-10-30 [1] Bioconductor
##     BiocCheck                            1.38.2         2024-01-27 [1] Bioconductor 3.18 (R 4.3.2)
##     BiocFileCache                        2.10.1         2023-10-26 [1] Bioconductor
##     BiocGenerics                         0.48.1         2023-11-01 [1] Bioconductor
##     BiocIO                               1.12.0         2023-10-26 [1] Bioconductor
##     BiocManager                          1.30.22        2023-08-08 [1] CRAN (R 4.3.0)
##     BiocNeighbors                        1.20.2         2024-01-13 [1] Bioconductor 3.18 (R 4.3.2)
##     BiocParallel                         1.36.0         2023-10-26 [1] Bioconductor
##     BiocPkgTools                         1.20.0         2023-10-30 [1] Bioconductor
##     BiocSingular                         1.18.0         2023-10-24 [1] Bioconductor
##     BiocStyle                            2.30.0         2023-10-26 [1] Bioconductor
##     biocthis                             1.12.0         2023-10-26 [1] Bioconductor
##     BiocVersion                          3.18.1         2023-11-18 [1] Bioconductor 3.18 (R 4.3.2)
##     biocViews                            1.70.0         2023-10-26 [1] Bioconductor
##     biolink                              0.1.8          2023-08-21 [1] CRAN (R 4.3.0)
##     biomaRt                              2.58.2         2024-02-03 [1] Bioconductor 3.18 (R 4.3.2)
##     Biostrings                           2.70.2         2024-01-30 [1] Bioconductor 3.18 (R 4.3.2)
##     biovizBase                           1.50.0         2023-10-26 [1] Bioconductor
##     bit                                  4.0.5          2022-11-15 [1] CRAN (R 4.3.0)
##     bit64                                4.0.5          2020-08-30 [1] CRAN (R 4.3.0)
##     bitops                               1.0-7          2021-04-24 [1] CRAN (R 4.3.0)
##     blob                                 1.2.4          2023-03-17 [1] CRAN (R 4.3.0)
##     bold                                 1.3.0          2023-05-02 [1] CRAN (R 4.3.0)
##     bookdown                             0.38           2024-03-04 [1] CRAN (R 4.3.1)
##     boot                                 1.3-30         2024-02-26 [1] CRAN (R 4.3.1)
##     brew                                 1.0-10         2023-12-16 [1] CRAN (R 4.3.1)
##     BRGenomics                           1.14.1         2024-03-02 [1] Bioconductor 3.18 (R 4.3.2)
##     brio                                 1.1.4          2023-12-10 [1] CRAN (R 4.3.1)
##     broom                                1.0.5          2023-06-09 [1] CRAN (R 4.3.0)
##     broom.helpers                        1.14.0         2023-08-07 [1] CRAN (R 4.3.0)
##     BSgenome                             1.70.2         2024-02-10 [1] Bioconductor 3.18 (R 4.3.2)
##     BSgenome.Hsapiens.UCSC.hg19          1.4.3          2023-10-13 [1] Bioconductor
##     BSgenome.Hsapiens.UCSC.hg38          1.4.5          2023-10-13 [1] Bioconductor
##     BSgenome.Mmusculus.UCSC.mm10         1.4.3          2023-10-13 [1] Bioconductor
##     BSgenome.Mmusculus.UCSC.mm9          1.4.0          2023-10-13 [1] Bioconductor
##     bslib                                0.6.1          2023-11-28 [1] CRAN (R 4.3.1)
##     bsplus                               0.1.4          2022-11-16 [1] CRAN (R 4.3.0)
##     BWStest                              0.2.3          2023-10-10 [1] CRAN (R 4.3.1)
##     ca                                   0.71.1         2020-01-24 [1] CRAN (R 4.3.0)
##     cachem                               1.0.8          2023-05-01 [1] CRAN (R 4.3.0)
##     Cairo                                1.6-2          2023-11-28 [1] CRAN (R 4.3.1)
##     callr                                3.7.5          2024-02-19 [1] CRAN (R 4.3.1)
##     car                                  3.1-2          2023-03-30 [1] CRAN (R 4.3.0)
##     carData                              3.0-5          2022-01-06 [1] CRAN (R 4.3.0)
##     caret                                6.0-94         2023-03-21 [1] CRAN (R 4.3.0)
##     catalogueR                           1.0.1          2023-09-20 [1] Github (RajLabMSSM/catalogueR@9868792)
##     caTools                              1.18.2         2021-03-28 [1] CRAN (R 4.3.0)
##     cellranger                           1.1.0          2016-07-27 [1] CRAN (R 4.3.0)
##     cellxgene.census                     1.8.0          2023-11-20 [1] https://chanzuckerberg.r-universe.dev (R 4.3.2)
##     chattr                               0.0.0.9005     2023-10-24 [1] Github (mlverse/chattr@210cfb2)
##     checkmate                            2.3.1          2023-12-04 [1] CRAN (R 4.3.1)
##     ChIPseeker                           1.38.0         2023-10-26 [1] Bioconductor
##     chromote                             0.2.0          2024-02-12 [1] CRAN (R 4.3.1)
##     chromVAR                             1.24.0         2023-10-24 [1] Bioconductor
##     circlize                             0.4.16         2024-02-20 [1] CRAN (R 4.3.1)
##     class                                7.3-22         2023-05-03 [1] CRAN (R 4.3.1)
##     classInt                             0.4-10         2023-09-05 [1] CRAN (R 4.3.0)
##     cli                                  3.6.2          2023-12-11 [1] CRAN (R 4.3.1)
##     clipr                                0.8.0          2022-02-22 [1] CRAN (R 4.3.0)
##     clisymbols                           1.2.0          2017-05-21 [1] CRAN (R 4.3.0)
##     clock                                0.7.0          2023-05-15 [1] CRAN (R 4.3.0)
##     clue                                 0.3-65         2023-09-23 [1] CRAN (R 4.3.1)
##     cluster                              2.1.6          2023-12-01 [1] CRAN (R 4.3.1)
##     clusterGeneration                    1.3.8          2023-08-16 [1] CRAN (R 4.3.0)
##     clusterProfiler                      4.10.1         2024-03-09 [1] Bioconductor 3.18 (R 4.3.3)
##     clustree                             0.5.1          2023-11-05 [1] CRAN (R 4.3.1)
##     CNEr                                 1.38.0         2023-10-24 [1] Bioconductor
##     coda                                 0.19-4.1       2024-01-31 [1] CRAN (R 4.3.1)
##     codetools                            0.2-19         2023-02-01 [1] CRAN (R 4.3.1)
##     coin                                 1.4-3          2023-09-27 [1] CRAN (R 4.3.1)
##     collections                          0.3.7          2023-01-05 [1] CRAN (R 4.3.0)
##     coloc                                5.2.3          2023-10-03 [1] CRAN (R 4.3.1)
##     colorDF                              0.1.7          2022-09-26 [1] CRAN (R 4.3.0)
##     colorjam                             0.0.27.900     2023-10-12 [1] Github (jmw86069/colorjam@b92c6df)
##     colorRamp2                           0.1.0          2022-12-21 [1] CRAN (R 4.3.0)
##     colorspace                           2.1-0          2023-01-23 [1] CRAN (R 4.3.0)
##     combinat                             0.0-8          2012-10-29 [1] CRAN (R 4.3.0)
##     CommonDataModel                      0.2.0          2023-11-16 [1] Github (OHDSI/CommonDataModel@55c4d7a)
##     commonmark                           1.9.1          2024-01-30 [1] CRAN (R 4.3.1)
##   P compiler                             4.3.1          2023-06-16 [1] local
##     ComplexHeatmap                       2.18.0         2023-10-26 [1] Bioconductor
##     ComplexUpset                         1.3.3          2021-12-11 [1] CRAN (R 4.3.0)
##     concatenate                          1.0.0          2016-05-08 [1] CRAN (R 4.3.0)
##     conditionz                           0.1.0          2019-04-24 [1] CRAN (R 4.3.0)
##     config                               0.3.2          2023-08-30 [1] CRAN (R 4.3.0)
##     conflicted                           1.2.0          2023-02-01 [1] CRAN (R 4.3.0)
##     consensusSeekeR                      1.30.0         2023-10-26 [1] Bioconductor
##     contfrac                             1.1-12         2018-05-17 [1] CRAN (R 4.3.0)
##     coro                                 1.0.4          2024-03-11 [1] CRAN (R 4.3.1)
##     corpcor                              1.6.10         2021-09-16 [1] CRAN (R 4.3.0)
##     correlation                          0.8.4          2023-04-06 [1] CRAN (R 4.3.0)
##     corrplot                             0.92           2021-11-18 [1] CRAN (R 4.3.0)
##     covr                                 3.6.4          2023-11-09 [1] CRAN (R 4.3.1)
##     cowplot                              1.1.3          2024-01-22 [1] CRAN (R 4.3.1)
##     cpp11                                0.4.7          2023-12-02 [1] CRAN (R 4.3.1)
##     cranlogs                             2.1.2          2023-10-24 [1] Github (neurogenomics/cranlogs@7a063a6)
##     crayon                               1.5.2          2022-09-29 [1] CRAN (R 4.3.0)
##     credentials                          2.0.1          2023-09-06 [1] CRAN (R 4.3.0)
##     crosstalk                            1.2.1          2023-11-23 [1] CRAN (R 4.3.1)
##     crul                                 1.4.0          2023-05-17 [1] CRAN (R 4.3.0)
##     curl                                 5.2.1          2024-03-01 [1] CRAN (R 4.3.1)
##     CVXR                                 1.0-12         2024-02-02 [1] CRAN (R 4.3.1)
##     cyclocomp                            1.1.1          2023-08-30 [1] CRAN (R 4.3.0)
##     data.table                           1.15.2         2024-02-29 [1] CRAN (R 4.3.1)
##     data.tree                            1.1.0          2023-11-12 [1] CRAN (R 4.3.1)
##     DatabaseConnector                    6.3.2          2023-12-11 [1] CRAN (R 4.3.1)
##     DatabaseConnectorJars                1.1.0          2019-04-07 [1] CRAN (R 4.3.0)
##   P datasets                           * 4.3.1          2023-06-16 [1] local
##     datawizard                           0.9.1          2023-12-21 [1] CRAN (R 4.3.1)
##     DBI                                  1.2.2          2024-02-16 [1] CRAN (R 4.3.1)
##     dbparser                             2.0.2          2024-02-16 [1] CRAN (R 4.3.1)
##     dbplyr                               2.4.0          2023-10-26 [1] CRAN (R 4.3.1)
##     dbscan                               1.1-12         2023-11-28 [1] CRAN (R 4.3.1)
##     DDRTree                              0.1.5          2017-04-30 [1] CRAN (R 4.3.0)
##     debugme                              1.1.0          2017-10-22 [1] CRAN (R 4.3.0)
##     DelayedArray                         0.28.0         2023-10-24 [1] Bioconductor
##     DelayedMatrixStats                   1.24.0         2023-10-24 [1] Bioconductor
##     deldir                               2.0-4          2024-02-28 [1] CRAN (R 4.3.1)
##     dendextend                           1.17.1         2023-03-25 [1] CRAN (R 4.3.0)
##     desc                                 1.4.3          2023-12-10 [1] CRAN (R 4.3.1)
##     DescTools                            0.99.54        2024-02-03 [1] CRAN (R 4.3.1)
##     DESeq2                               1.42.1         2024-03-09 [1] Bioconductor 3.18 (R 4.3.3)
##     deSolve                              1.40           2023-11-27 [1] CRAN (R 4.3.1)
##     devoptera                            0.99.1         2023-12-10 [1] Bioconductor
##     devtools                             2.4.5          2022-10-11 [1] CRAN (R 4.3.0)
##     dfidx                                0.0-5          2022-06-28 [1] CRAN (R 4.3.0)
##     diagram                              1.6.5          2020-09-30 [1] CRAN (R 4.3.0)
##     DiagrammeR                           1.0.11         2024-02-02 [1] CRAN (R 4.3.1)
##     dials                                1.2.1          2024-02-22 [1] CRAN (R 4.3.1)
##     DiceDesign                           1.10           2023-12-07 [1] CRAN (R 4.3.1)
##     dichromat                            2.0-0.1        2022-05-02 [1] CRAN (R 4.3.0)
##     diffobj                              0.3.5          2021-10-05 [1] CRAN (R 4.3.0)
##     digest                               0.6.35         2024-03-11 [1] CRAN (R 4.3.1)
##     dimensionsR                          0.0.3          2022-02-07 [1] CRAN (R 4.3.0)
##     dir.expiry                           1.10.0         2023-10-26 [1] Bioconductor
##     DirichletMultinomial                 1.44.0         2023-10-26 [1] Bioconductor
##     distributional                       0.4.0          2024-02-07 [1] CRAN (R 4.3.1)
##     dlstats                              0.1.7          2023-05-24 [1] CRAN (R 4.3.0)
##     dnet                                 1.1.7          2020-02-20 [1] CRAN (R 4.3.0)
##     docopt                               0.7.1          2020-06-24 [1] CRAN (R 4.3.0)
##     doParallel                           1.0.17         2022-02-07 [1] CRAN (R 4.3.0)
##     DOSE                                 3.28.2         2023-12-12 [1] Bioconductor 3.18 (R 4.3.2)
##     dotCall64                            1.1-1          2023-11-28 [1] CRAN (R 4.3.1)
##     dotenv                               1.0.3          2021-04-22 [1] CRAN (R 4.3.0)
##     downlit                              0.4.3          2023-06-29 [1] CRAN (R 4.3.0)
##     downloader                           0.4            2015-07-09 [1] CRAN (R 4.3.0)
##     downloadR                            0.99.6         2023-09-20 [1] Github (RajLabMSSM/downloadR@182e3f3)
##     downloadthis                         0.3.3          2023-11-09 [1] CRAN (R 4.3.1)
##     dplyr                                1.1.4          2023-11-17 [1] CRAN (R 4.3.1)
##     dqrng                                0.3.2          2023-11-29 [1] CRAN (R 4.3.1)
##     DrImpute                             1.0            2017-07-15 [1] CRAN (R 4.3.0)
##     DT                                   0.32           2024-02-19 [1] CRAN (R 4.3.1)
##     dtplyr                               1.3.1          2023-03-22 [1] CRAN (R 4.3.0)
##     dynamicTreeCut                       1.63-1         2016-03-11 [1] CRAN (R 4.3.0)
##     e1071                                1.7-14         2023-12-06 [1] CRAN (R 4.3.1)
##     echoannot                            0.99.11        2023-10-24 [1] Github (RajLabMSSM/echoannot@d18debe)
##     echoconda                            0.99.10        2024-02-11 [1] local
##     echodata                             0.99.17        2024-02-11 [1] Github (RajLabMSSM/echodata@0d19cc1)
##     echodeps                             0.99.3         2023-10-27 [1] Bioconductor
##     echofinemap                          0.99.5         2023-09-20 [1] Github (RajLabMSSM/echofinemap@7a0013e)
##     echogithub                           0.99.2         2024-01-26 [1] Github (RajLabMSSM/echogithub@1e3594d)
##     echoLD                               0.99.9         2023-09-20 [1] Github (RajLabMSSM/echoLD@7cf3953)
##     echolocatoR                          2.0.3          2023-09-20 [1] Github (RajLabMSSM/echolocatoR@c9cc313)
##     echoplot                             0.99.7         2023-10-24 [1] Github (RajLabMSSM/echoplot@fd2605d)
##     echotabix                            0.99.10        2023-11-17 [1] local
##     echoverseTemplate                    0.99.0         2023-10-24 [1] Github (RajLabMSSM/echoverseTemplate@f5a0db0)
##     ECOSolveR                            0.5.5          2023-05-15 [1] CRAN (R 4.3.0)
##     edgeR                                4.0.16         2024-02-20 [1] Bioconductor 3.18 (R 4.3.2)
##     effectsize                           0.8.6          2023-09-14 [1] CRAN (R 4.3.0)
##     egg                                  0.4.5          2019-07-13 [1] CRAN (R 4.3.0)
##     ellipse                              0.5.0          2023-07-20 [1] CRAN (R 4.3.0)
##     ellipsis                             0.3.2          2021-04-29 [1] CRAN (R 4.3.0)
##     elliptic                             1.4-0          2019-03-14 [1] CRAN (R 4.3.0)
##     emmeans                              1.10.0         2024-01-23 [1] CRAN (R 4.3.1)
##     english                              1.2-6          2021-08-21 [1] CRAN (R 4.3.0)
##     enrichplot                           1.22.0         2023-10-24 [1] Bioconductor
##     EnsDb.Hsapiens.v75                   2.99.0         2023-09-20 [1] Bioconductor
##     EnsDb.Hsapiens.v86                   2.99.0         2023-11-17 [1] Bioconductor
##     ensembldb                            2.26.0         2023-10-26 [1] Bioconductor
##     ensemblr                             0.1.0          2024-02-06 [1] Github (ramiromagno/ensemblr@8507fc9)
##     ensemblVEP                           1.44.0         2023-11-02 [1] Bioconductor
##     EnvStats                             2.8.1          2023-08-22 [1] CRAN (R 4.3.0)
##     EpiCompare                           1.6.5          2024-02-13 [1] Bioconductor 3.18 (R 4.3.2)
##     estimability                         1.5            2024-02-20 [1] CRAN (R 4.3.1)
##     etm                                  1.1.1          2020-09-08 [1] CRAN (R 4.3.0)
##     europepmc                            0.4.3          2023-09-20 [1] CRAN (R 4.3.1)
##     evaluate                             0.23           2023-11-01 [1] CRAN (R 4.3.1)
##     EWCE                                 1.11.3         2024-01-26 [1] Github (NathanSkene/EWCE@3838e2c)
##     ewceData                             1.10.0         2023-10-26 [1] Bioconductor
##     Exact                                3.2            2022-09-25 [1] CRAN (R 4.3.0)
##     ExperimentHub                        2.10.0         2023-10-26 [1] Bioconductor
##     expm                                 0.999-9        2024-01-11 [1] CRAN (R 4.3.1)
##     FactoMineR                           2.10           2024-02-29 [1] CRAN (R 4.3.1)
##     fANCOVA                              0.6-1          2020-11-13 [1] CRAN (R 4.3.0)
##     fansi                                1.0.6          2023-12-08 [1] CRAN (R 4.3.1)
##     farver                               2.1.1          2022-07-06 [1] CRAN (R 4.3.0)
##     fastcluster                          1.2.6          2024-01-12 [1] CRAN (R 4.3.1)
##     fastDummies                          1.7.3          2023-07-06 [1] CRAN (R 4.3.0)
##     fastICA                              1.2-4          2023-11-27 [1] CRAN (R 4.3.1)
##     fastmap                              1.1.1          2023-02-24 [1] CRAN (R 4.3.0)
##     fastmatch                            1.1-4          2023-08-18 [1] CRAN (R 4.3.0)
##     fauxpas                              0.5.2          2023-05-03 [1] CRAN (R 4.3.0)
##     ff                                   4.0.12         2024-01-12 [1] CRAN (R 4.3.1)
##     fgsea                                1.28.0         2023-10-26 [1] Bioconductor
##     filelock                             1.0.3          2023-12-11 [1] CRAN (R 4.3.1)
##     fitdistrplus                         1.1-11         2023-04-25 [1] CRAN (R 4.3.0)
##     flashClust                           1.01-2         2012-08-21 [1] CRAN (R 4.3.0)
##     flock                                0.7            2016-11-12 [1] CRAN (R 4.3.0)
##     FNN                                  1.1.4          2024-01-12 [1] CRAN (R 4.3.1)
##     fontawesome                          0.5.2          2023-08-19 [1] CRAN (R 4.3.0)
##     forcats                              1.0.0          2023-01-29 [1] CRAN (R 4.3.0)
##     foreach                              1.5.2          2022-02-02 [1] CRAN (R 4.3.0)
##     forecast                             8.22.0         2024-03-04 [1] CRAN (R 4.3.1)
##     foreign                              0.8-86         2023-11-28 [1] CRAN (R 4.3.1)
##     formatR                              1.14           2023-01-17 [1] CRAN (R 4.3.0)
##     Formula                              1.2-5          2023-02-24 [1] CRAN (R 4.3.0)
##     formula.tools                        1.7.1          2018-03-01 [1] CRAN (R 4.3.0)
##     fracdiff                             1.5-3          2024-02-01 [1] CRAN (R 4.3.1)
##     fresh                                0.2.0          2020-05-29 [1] CRAN (R 4.3.0)
##     fs                                   1.6.3          2023-07-20 [1] CRAN (R 4.3.0)
##     furrr                                0.3.1          2022-08-15 [1] CRAN (R 4.3.0)
##     futile.logger                        1.4.3          2016-07-10 [1] CRAN (R 4.3.0)
##     futile.options                       1.0.1          2018-04-20 [1] CRAN (R 4.3.0)
##     future                               1.33.1         2023-12-22 [1] CRAN (R 4.3.1)
##     future.apply                         1.11.1         2023-12-21 [1] CRAN (R 4.3.1)
##     gargle                               1.5.2          2023-07-20 [1] CRAN (R 4.3.0)
##     gclus                                1.3.2          2019-01-07 [1] CRAN (R 4.3.0)
##     gdata                                3.0.0          2023-10-16 [1] CRAN (R 4.3.1)
##     GeneOverlap                          1.38.0         2023-10-26 [1] Bioconductor
##     generics                             0.1.3          2022-07-05 [1] CRAN (R 4.3.0)
##     genetics.binaRies                    0.1.1          2023-10-20 [1] Github (MRCIEU/genetics.binaRies@b0324f1)
##     genomation                           1.34.0         2023-10-26 [1] Bioconductor
##     GenomeInfoDb                         1.38.7         2024-03-09 [1] Bioconductor 3.18 (R 4.3.3)
##     GenomeInfoDbData                     1.2.11         2023-10-19 [1] Bioconductor
##     GenomicAlignments                    1.38.2         2024-01-20 [1] Bioconductor 3.18 (R 4.3.2)
##     GenomicFeatures                      1.54.4         2024-03-12 [1] Bioconductor 3.18 (R 4.3.3)
##     GenomicFiles                         1.38.0         2023-10-26 [1] Bioconductor
##     GenomicInteractions                  1.36.0         2023-10-26 [1] Bioconductor
##     GenomicRanges                        1.54.1         2023-10-30 [1] Bioconductor
##     GenomicSEM                           0.0.5          2023-12-13 [1] Github (GenomicSEM/GenomicSEM@a723459)
##     geodata                              0.5-9          2023-10-13 [1] CRAN (R 4.3.1)
##     GEOmetadb                            1.64.0         2023-10-26 [1] Bioconductor
##     GEOquery                             2.70.0         2023-10-26 [1] Bioconductor
##     gert                                 2.0.1          2023-12-04 [1] CRAN (R 4.3.1)
##     getopt                               1.20.4         2023-10-01 [1] CRAN (R 4.3.1)
##     GetoptLong                           1.0.5          2020-12-15 [1] CRAN (R 4.3.0)
##     GGally                               2.2.1          2024-02-14 [1] CRAN (R 4.3.1)
##     ggbeeswarm                           0.7.2          2023-04-29 [1] CRAN (R 4.3.0)
##     ggbio                                1.50.0         2023-11-01 [1] Bioconductor
##     ggbreak                              0.1.2          2023-06-26 [1] CRAN (R 4.3.0)
##     ggcorrplot                           0.1.4.1        2023-09-05 [1] CRAN (R 4.3.0)
##     ggdendro                             0.2.0          2024-02-23 [1] CRAN (R 4.3.1)
##     ggdist                               3.3.2          2024-03-05 [1] CRAN (R 4.3.1)
##     ggforce                              0.4.2          2024-02-19 [1] CRAN (R 4.3.1)
##     ggfun                                0.1.4          2024-01-19 [1] CRAN (R 4.3.1)
##     ggimage                              0.3.3          2023-06-19 [1] CRAN (R 4.3.0)
##     gginnards                            0.1.2          2023-05-24 [1] CRAN (R 4.3.0)
##     ggiraph                              0.8.9          2024-02-24 [1] CRAN (R 4.3.1)
##     ggnetwork                            0.5.13         2024-02-14 [1] CRAN (R 4.3.1)
##     ggnewscale                           0.4.10         2024-02-08 [1] CRAN (R 4.3.1)
##     ggpattern                            1.0.1          2022-11-09 [1] CRAN (R 4.3.0)
##     ggplot2                              3.5.0          2024-02-23 [1] CRAN (R 4.3.1)
##     ggplotify                            0.1.2          2023-08-09 [1] CRAN (R 4.3.0)
##     ggpubr                               0.6.0          2023-02-10 [1] CRAN (R 4.3.0)
##     ggraph                               2.2.1          2024-03-07 [1] CRAN (R 4.3.1)
##     ggrastr                              1.0.2          2023-06-01 [1] CRAN (R 4.3.0)
##     ggrepel                              0.9.5          2024-01-10 [1] CRAN (R 4.3.1)
##     ggridges                             0.5.6          2024-01-23 [1] CRAN (R 4.3.1)
##     ggsci                                3.0.1          2024-03-02 [1] CRAN (R 4.3.1)
##     ggside                               0.3.1          2024-03-01 [1] CRAN (R 4.3.1)
##     ggsignif                             0.6.4          2022-10-13 [1] CRAN (R 4.3.0)
##     ggstats                              0.5.1          2023-11-21 [1] CRAN (R 4.3.1)
##     ggstatsplot                          0.12.2         2024-01-14 [1] CRAN (R 4.3.1)
##     ggtext                               0.1.2          2022-09-16 [1] CRAN (R 4.3.0)
##     ggtree                               3.10.1         2024-02-27 [1] Bioconductor 3.18 (R 4.3.2)
##     gh                                   1.4.0          2023-02-22 [1] CRAN (R 4.3.0)
##     gitcreds                             0.1.2          2022-09-08 [1] CRAN (R 4.3.0)
##     githubinstall                        0.2.2          2018-02-18 [1] CRAN (R 4.3.0)
##     gld                                  2.6.6          2022-10-23 [1] CRAN (R 4.3.0)
##     glmGamPoi                            1.14.3         2024-02-10 [1] Bioconductor 3.18 (R 4.3.2)
##     glmnet                               4.1-8          2023-08-22 [1] CRAN (R 4.3.0)
##     GlobalOptions                        0.1.2          2020-06-10 [1] CRAN (R 4.3.0)
##     globals                              0.16.3         2024-03-08 [1] CRAN (R 4.3.1)
##     glue                                 1.7.0          2024-01-09 [1] CRAN (R 4.3.1)
##     gmp                                  0.7-4          2024-01-15 [1] CRAN (R 4.3.1)
##     GO.db                                3.18.0         2023-10-13 [1] Bioconductor
##     goftest                              1.2-3          2021-10-07 [1] CRAN (R 4.3.0)
##     googleAuthR                          2.0.1          2023-04-11 [1] CRAN (R 4.3.0)
##     googledrive                          2.1.1          2023-06-11 [1] CRAN (R 4.3.0)
##     googlesheets4                        1.1.1          2023-06-11 [1] CRAN (R 4.3.0)
##     GOSemSim                             2.28.1         2024-01-20 [1] Bioconductor 3.18 (R 4.3.2)
##     gower                                1.0.1          2022-12-22 [1] CRAN (R 4.3.0)
##     GPfit                                1.0-8          2019-02-08 [1] CRAN (R 4.3.0)
##     gplots                               3.1.3.1        2024-02-02 [1] CRAN (R 4.3.1)
##     gprofiler2                           0.2.3          2024-02-23 [1] CRAN (R 4.3.1)
##     graph                                1.80.0         2023-10-26 [1] Bioconductor
##   P graphics                           * 4.3.1          2023-06-16 [1] local
##     graphlayouts                         1.1.1          2024-03-09 [1] CRAN (R 4.3.1)
##   P grDevices                          * 4.3.1          2023-06-16 [1] local
##     grid                                 4.3.1          2023-06-16 [?] local
##     gridBase                             0.4-7          2014-02-24 [1] CRAN (R 4.3.0)
##     gridExtra                            2.3            2017-09-09 [1] CRAN (R 4.3.0)
##     gridGraphics                         0.5-1          2020-12-13 [1] CRAN (R 4.3.0)
##     gridpattern                          1.1.1          2023-10-25 [1] CRAN (R 4.3.1)
##     gridtext                             0.1.5          2022-09-16 [1] CRAN (R 4.3.0)
##     grImport2                            0.3-1          2023-10-27 [1] CRAN (R 4.3.1)
##     grr                                  0.9.5          2016-08-26 [1] CRAN (R 4.3.0)
##     gson                                 0.1.0          2023-03-07 [1] CRAN (R 4.3.0)
##     gtable                               0.3.4          2023-08-21 [1] CRAN (R 4.3.0)
##     gtools                               3.9.5          2023-11-20 [1] CRAN (R 4.3.1)
##     Gviz                                 1.46.1         2023-11-18 [1] Bioconductor 3.18 (R 4.3.2)
##     h2o                                  3.44.0.3       2024-01-11 [1] CRAN (R 4.3.1)
##     haploR                               4.0.7          2023-10-09 [1] CRAN (R 4.3.1)
##     hardhat                              1.3.1          2024-02-02 [1] CRAN (R 4.3.1)
##     harmony                              1.2.0          2023-11-29 [1] CRAN (R 4.3.1)
##     haven                                2.5.4          2023-11-30 [1] CRAN (R 4.3.1)
##     HDF5Array                            1.30.1         2024-02-17 [1] Bioconductor 3.18 (R 4.3.2)
##     hdf5r                                1.3.10         2024-03-02 [1] CRAN (R 4.3.1)
##     HDO.db                               0.99.1         2023-10-13 [1] Bioconductor
##     heatmaply                            1.5.0          2023-10-06 [1] CRAN (R 4.3.1)
##     here                                 1.0.1          2020-12-13 [1] CRAN (R 4.3.0)
##     hexbin                               1.28.3         2023-03-21 [1] CRAN (R 4.3.0)
##     hexSticker                           0.4.9          2020-12-05 [1] CRAN (R 4.3.0)
##     HGNChelper                           0.8.1          2019-10-24 [1] CRAN (R 4.3.0)
##     highr                                0.10           2022-12-22 [1] CRAN (R 4.3.0)
##     Hmisc                                5.1-2          2024-03-11 [1] CRAN (R 4.3.1)
##     hms                                  1.1.3          2023-03-21 [1] CRAN (R 4.3.0)
##     homologene                           1.4.68.19.3.27 2019-03-28 [1] CRAN (R 4.3.0)
##     HPO.db                               0.99.2         2023-06-28 [1] Bioconductor
##     HPOExplorer                          1.0.0          2024-03-15 [1] Bioconductor
##     HSMMSingleCell                       1.22.0         2023-10-26 [1] Bioconductor
##     htmlTable                            2.4.2          2023-10-29 [1] CRAN (R 4.3.1)
##     htmltools                            0.5.7          2023-11-03 [1] CRAN (R 4.3.1)
##     htmlwidgets                          1.6.4          2023-12-06 [1] CRAN (R 4.3.1)
##     httpcode                             0.3.0          2020-04-10 [1] CRAN (R 4.3.0)
##     httpuv                               1.6.14         2024-01-26 [1] CRAN (R 4.3.1)
##     httr                                 1.4.7          2023-08-15 [1] CRAN (R 4.3.0)
##     httr2                                1.0.0          2023-11-14 [1] CRAN (R 4.3.1)
##     hunspell                             3.0.3          2023-10-06 [1] CRAN (R 4.3.1)
##     hypergeo                             1.2-13         2016-04-07 [1] CRAN (R 4.3.0)
##     ica                                  1.0-3          2022-07-08 [1] CRAN (R 4.3.0)
##     ids                                  1.0.1          2017-05-31 [1] CRAN (R 4.3.0)
##     igraph                               2.0.3          2024-03-13 [1] CRAN (R 4.3.1)
##     impute                               1.76.0         2023-10-26 [1] Bioconductor
##     infer                                1.0.6          2024-01-31 [1] CRAN (R 4.3.1)
##     ini                                  0.3.1          2018-05-20 [1] CRAN (R 4.3.0)
##     innsight                             0.3.0          2023-12-21 [1] CRAN (R 4.3.1)
##     insight                              0.19.8         2024-01-31 [1] CRAN (R 4.3.1)
##     InteractionSet                       1.30.0         2023-10-26 [1] Bioconductor
##     interactiveDisplayBase               1.40.0         2023-10-26 [1] Bioconductor
##     interp                               1.1-6          2024-01-26 [1] CRAN (R 4.3.1)
##     ipred                                0.9-14         2023-03-09 [1] CRAN (R 4.3.0)
##     IRanges                              2.36.0         2023-10-26 [1] Bioconductor
##     irlba                                2.3.5.1        2022-10-03 [1] CRAN (R 4.3.0)
##     isoband                              0.2.7          2022-12-20 [1] CRAN (R 4.3.0)
##     ISOcodes                             2024.02.12     2024-02-12 [1] CRAN (R 4.3.1)
##     iterators                            1.0.14         2022-02-05 [1] CRAN (R 4.3.0)
##     itertools                            0.1-3          2014-03-12 [1] CRAN (R 4.3.0)
##     jamba                                0.0.96.900     2023-10-12 [1] Github (jmw86069/jamba@40c1a1c)
##     jamma                                0.0.33.900     2023-10-12 [1] Github (jmw86069/jamma@169b1d7)
##     janeaustenr                          1.0.0          2022-08-26 [1] CRAN (R 4.3.0)
##     jpeg                                 0.1-10         2022-11-29 [1] CRAN (R 4.3.0)
##     jquerylib                            0.1.4          2021-04-26 [1] CRAN (R 4.3.0)
##     jsonlite                             1.8.8          2023-12-04 [1] CRAN (R 4.3.1)
##     kableExtra                           1.4.0          2024-01-24 [1] CRAN (R 4.3.1)
##     KEGGREST                             1.42.0         2023-10-26 [1] Bioconductor
##     keras                                2.13.0         2023-08-15 [1] CRAN (R 4.3.0)
##     kernlab                              0.9-32         2023-01-31 [1] CRAN (R 4.3.0)
##     KernSmooth                           2.23-22        2023-07-10 [1] CRAN (R 4.3.0)
##     KGExplorer                           0.99.0         2024-03-15 [1] Bioconductor
##     knitr                                1.45           2023-10-30 [1] CRAN (R 4.3.1)
##     KnowledgeNets                        0.99.0         2023-12-10 [1] local
##     ks                                   1.14.2         2024-01-15 [1] CRAN (R 4.3.1)
##     kSamples                             1.2-10         2023-10-07 [1] CRAN (R 4.3.1)
##     labdsv                               2.1-0          2023-04-10 [1] CRAN (R 4.3.0)
##     labeling                             0.4.3          2023-08-29 [1] CRAN (R 4.3.0)
##     labelled                             2.12.0         2023-06-21 [1] CRAN (R 4.3.0)
##     lambda.r                             1.2.4          2019-09-18 [1] CRAN (R 4.3.0)
##     languageserver                       0.3.16         2023-08-18 [1] CRAN (R 4.3.0)
##     later                                1.3.2          2023-12-06 [1] CRAN (R 4.3.1)
##     lattice                              0.22-5         2023-10-24 [1] CRAN (R 4.3.1)
##     latticeExtra                         0.6-30         2022-07-04 [1] CRAN (R 4.3.0)
##     lava                                 1.8.0          2024-03-05 [1] CRAN (R 4.3.1)
##     lavaan                               0.6-17         2023-12-20 [1] CRAN (R 4.3.1)
##     lazyeval                             0.2.2          2019-03-15 [1] CRAN (R 4.3.0)
##     leaflet                              2.2.1          2023-11-13 [1] CRAN (R 4.3.1)
##     leaflet.providers                    2.0.0          2023-10-17 [1] CRAN (R 4.3.1)
##     leaps                                3.1            2020-01-16 [1] CRAN (R 4.3.0)
##     leiden                               0.4.3.1        2023-11-17 [1] CRAN (R 4.3.1)
##     leidenbase                           0.1.27         2023-12-01 [1] CRAN (R 4.3.1)
##     lemur                                1.0.5          2023-12-06 [1] Bioconductor 3.18 (R 4.3.1)
##     lhs                                  1.1.6          2022-12-17 [1] CRAN (R 4.3.0)
##     libcoin                              1.0-10         2023-09-27 [1] CRAN (R 4.3.1)
##     lifecycle                            1.0.4          2023-11-07 [1] CRAN (R 4.3.1)
##     limma                                3.58.1         2023-10-31 [1] Bioconductor
##     lintr                                3.1.1          2023-11-07 [1] CRAN (R 4.3.1)
##     listenv                              0.9.1          2024-01-29 [1] CRAN (R 4.3.1)
##     lme4                                 1.1-35.1       2023-11-05 [1] CRAN (R 4.3.1)
##     lmerTest                             3.1-3          2020-10-23 [1] CRAN (R 4.3.0)
##     lmom                                 3.0            2023-08-29 [1] CRAN (R 4.3.0)
##     lmtest                               0.9-40         2022-03-21 [1] CRAN (R 4.3.0)
##     locfit                               1.5-9.9        2024-03-01 [1] CRAN (R 4.3.1)
##     LoomExperiment                       1.20.0         2023-10-24 [1] Bioconductor
##     loomR                                0.2.0          2023-10-10 [1] Github (mojaveazure/loomR@df0144b)
##     lubridate                            1.9.3          2023-09-27 [1] CRAN (R 4.3.1)
##     luz                                  0.4.0          2023-04-17 [1] CRAN (R 4.3.0)
##     MACSr                                1.10.0         2023-10-26 [1] Bioconductor
##     magick                               2.8.3          2024-02-18 [1] CRAN (R 4.3.1)
##     MAGMA.Celltyping                     2.0.11         2023-09-20 [1] Github (neurogenomics/MAGMA_Celltyping@b4b9192)
##     magrittr                             2.0.3          2022-03-30 [1] CRAN (R 4.3.0)
##     maotai                               0.2.5          2023-03-29 [1] CRAN (R 4.3.0)
##     mapproj                              1.2.11         2023-01-12 [1] CRAN (R 4.3.0)
##     maps                                 3.4.2          2023-12-15 [1] CRAN (R 4.3.1)
##     markdown                             1.12           2023-12-06 [1] CRAN (R 4.3.1)
##     MASS                                 7.3-60.0.1     2024-01-13 [1] CRAN (R 4.3.1)
##     MAST                                 1.28.0         2023-10-24 [1] Bioconductor
##     Matrix                               1.6-5          2024-01-11 [1] CRAN (R 4.3.1)
##     MatrixGenerics                       1.14.0         2023-10-26 [1] Bioconductor
##     MatrixModels                         0.5-3          2023-11-06 [1] CRAN (R 4.3.1)
##     matrixStats                          1.2.0          2023-12-11 [1] CRAN (R 4.3.1)
##     mclust                               6.1            2024-02-23 [1] CRAN (R 4.3.1)
##     mclustcomp                           0.3.3          2021-06-13 [1] CRAN (R 4.3.0)
##     memoise                              2.0.1.9000     2023-12-21 [1] Github (r-lib/memoise@40db995)
##   P methods                            * 4.3.1          2023-06-16 [1] local
##     metR                                 0.15.0         2024-02-09 [1] CRAN (R 4.3.1)
##     mgcv                                 1.9-1          2023-12-21 [1] CRAN (R 4.3.1)
##     mgsub                                1.7.3          2021-07-28 [1] CRAN (R 4.3.0)
##     microbenchmark                       1.4.10         2023-04-28 [1] CRAN (R 4.3.0)
##     mime                                 0.12           2021-09-28 [1] CRAN (R 4.3.0)
##     miniUI                               0.1.1.1        2018-05-18 [1] CRAN (R 4.3.0)
##     minpack.lm                           1.2-4          2023-09-11 [1] CRAN (R 4.3.0)
##     minqa                                1.2.6          2023-09-11 [1] CRAN (R 4.3.0)
##     mixsqp                               0.3-54         2023-12-20 [1] CRAN (R 4.3.1)
##     mlogit                               1.1-1          2020-10-02 [1] CRAN (R 4.3.0)
##     mnormt                               2.1.1          2022-09-26 [1] CRAN (R 4.3.0)
##     mockery                              0.4.4          2023-09-26 [1] CRAN (R 4.3.1)
##     modeldata                            1.3.0          2024-01-21 [1] CRAN (R 4.3.1)
##     modelenv                             0.1.1          2023-03-08 [1] CRAN (R 4.3.0)
##     ModelMetrics                         1.2.2.2        2020-03-17 [1] CRAN (R 4.3.0)
##     modelr                               0.1.11         2023-03-22 [1] CRAN (R 4.3.0)
##     modeltools                           0.2-23         2020-03-05 [1] CRAN (R 4.3.0)
##     MOFA2                                1.12.1         2024-01-13 [1] Bioconductor 3.18 (R 4.3.2)
##     monarchr                             0.2.1          2024-03-14 [1] local
##     monocle                              2.30.0         2023-10-26 [1] Bioconductor
##     monocle3                             1.3.4          2023-10-10 [1] Github (cole-trapnell-lab/monocle3@2b17745)
##     motifbreakR                          2.16.0         2023-10-26 [1] Bioconductor
##     MotifDb                              1.44.0         2023-10-26 [1] Bioconductor
##     motifmatchr                          1.24.0         2023-10-24 [1] Bioconductor
##     motifStack                           1.46.0         2023-10-24 [1] Bioconductor
##     MPO.db                               0.99.7         2023-05-31 [1] Bioconductor
##     MSTExplorer                          1.0.0          2024-03-18 [1] Bioconductor
##     multcomp                             1.4-25         2023-06-20 [1] CRAN (R 4.3.0)
##     multcompView                         0.1-10         2024-03-08 [1] CRAN (R 4.3.1)
##     multicool                            1.0.1          2024-02-05 [1] CRAN (R 4.3.1)
##     MultiEWCE                            1.0.0          2024-02-24 [1] Bioconductor
##     MungeSumstats                        1.11.6         2024-02-11 [1] Github (neurogenomics/MungeSumstats@009dfd8)
##     munsell                              0.5.0          2018-06-12 [1] CRAN (R 4.3.0)
##     mvtnorm                              1.2-4          2023-11-27 [1] CRAN (R 4.3.1)
##     nabor                                0.5.0          2018-07-11 [1] CRAN (R 4.3.0)
##     nanotime                             0.3.7          2022-10-24 [1] CRAN (R 4.3.0)
##     natserv                              1.0.0          2020-05-16 [1] CRAN (R 4.3.0)
##     Nebulosa                             1.12.1         2024-03-02 [1] Bioconductor 3.18 (R 4.3.2)
##     neo2R                                2.4.2          2024-01-18 [1] CRAN (R 4.3.1)
##     neo4r                                0.1.1          2019-02-15 [1] CRAN (R 4.3.0)
##     network                              1.18.2         2023-12-05 [1] CRAN (R 4.3.1)
##     networkD3                            0.4            2017-03-18 [1] CRAN (R 4.3.0)
##     nlme                                 3.1-164        2023-11-27 [1] CRAN (R 4.3.1)
##     nloptr                               2.0.3          2022-05-26 [1] CRAN (R 4.3.0)
##     NLP                                  0.2-1          2020-10-14 [1] CRAN (R 4.3.0)
##     nnet                                 7.3-19         2023-05-03 [1] CRAN (R 4.3.1)
##     nortest                              1.0-4          2015-07-30 [1] CRAN (R 4.3.0)
##     numDeriv                             2016.8-1.1     2019-06-06 [1] CRAN (R 4.3.0)
##     oaqc                                 1.0            2017-11-14 [1] CRAN (R 4.3.0)
##     OmaDB                                2.18.0         2023-10-26 [1] Bioconductor
##     ontologyIndex                        2.12           2024-02-27 [1] CRAN (R 4.3.1)
##     ontologyPlot                         1.7            2024-02-20 [1] CRAN (R 4.3.1)
##     ontologySimilarity                   2.5            2021-02-10 [1] CRAN (R 4.3.0)
##     OntologyTermAggregator               0.1.0          2023-12-10 [1] Github (KrishnaTO/OntologyTermAggregator@4c71ac6)
##     ontoProc                             1.24.0         2023-10-26 [1] Bioconductor
##     openalexR                            1.2.3          2023-11-16 [1] CRAN (R 4.3.1)
##     openssl                              2.1.1          2023-09-25 [1] CRAN (R 4.3.1)
##     openxlsx                             4.2.5.2        2023-02-06 [1] CRAN (R 4.3.0)
##     operator.tools                       1.6.3          2017-02-28 [1] CRAN (R 4.3.0)
##     optimParallel                        1.0-2          2021-02-11 [1] CRAN (R 4.3.0)
##     optparse                             1.7.4          2024-01-16 [1] CRAN (R 4.3.1)
##     org.Hs.eg.db                         3.18.0         2023-10-19 [1] Bioconductor
##     OrganismDbi                          1.44.0         2023-10-26 [1] Bioconductor
##     orthogene                            1.9.1          2023-12-22 [1] Bioconductor
##     osfr                                 0.2.9          2022-09-25 [1] CRAN (R 4.3.0)
##     osqp                                 0.6.3.2        2023-10-20 [1] CRAN (R 4.3.1)
##     packrat                              0.9.2          2023-09-05 [1] CRAN (R 4.3.0)
##     padr                                 0.6.2          2022-11-23 [1] CRAN (R 4.3.0)
##     pagedown                             0.20           2022-12-13 [1] CRAN (R 4.3.0)
##     paintmap                             1.0            2016-08-31 [1] CRAN (R 4.3.0)
##     paletteer                            1.6.0          2024-01-21 [1] CRAN (R 4.3.1)
##     palmerpenguins                       0.1.1          2022-08-15 [1] CRAN (R 4.3.0)
##     pals                                 1.9            2024-01-26 [1] Github (kwstat/pals@73eea8f)
##     pandoc                               0.2.0          2023-08-24 [1] CRAN (R 4.3.0)
##     parallel                             4.3.1          2023-06-16 [?] local
##     parallelly                           1.37.1         2024-02-29 [1] CRAN (R 4.3.1)
##     parameters                           0.21.5         2024-02-07 [1] CRAN (R 4.3.1)
##     parsnip                              1.2.0          2024-02-16 [1] CRAN (R 4.3.1)
##     patchwork                            1.2.0          2024-01-08 [1] CRAN (R 4.3.1)
##     pbapply                              1.7-2          2023-06-27 [1] CRAN (R 4.3.0)
##     pbivnorm                             0.6.0          2015-01-23 [1] CRAN (R 4.3.0)
##     pbkrtest                             0.5.2          2023-01-19 [1] CRAN (R 4.3.0)
##     pbmcapply                            1.5.1          2022-04-28 [1] CRAN (R 4.3.0)
##     pcaMethods                           1.94.0         2023-10-26 [1] Bioconductor
##     pdftools                             3.4.0          2023-09-25 [1] CRAN (R 4.3.1)
##     PeakyFinders                         0.99.4         2023-10-19 [1] Github (neurogenomics/PeakyFinders@f918067)
##     performance                          0.10.9         2024-02-17 [1] CRAN (R 4.3.1)
##     PerformanceAnalytics                 2.0.4          2020-02-06 [1] CRAN (R 4.3.0)
##     permute                              0.9-7          2022-01-27 [1] CRAN (R 4.3.0)
##     phangorn                             2.11.1         2023-01-23 [1] CRAN (R 4.3.0)
##     pheatmap                             1.0.12         2019-01-04 [1] CRAN (R 4.3.0)
##     phenomix                             0.99.6         2024-03-16 [1] Bioconductor
##     phenoRx                              0.99.0         2024-03-01 [1] local
##     phylobase                            0.8.12         2024-01-30 [1] CRAN (R 4.3.1)
##     phytools                             2.1-1          2024-01-09 [1] CRAN (R 4.3.1)
##     piggyback                            0.1.5          2023-07-10 [1] CRAN (R 4.3.0)
##     pillar                               1.9.0          2023-03-22 [1] CRAN (R 4.3.0)
##     pingr                                2.0.3          2023-12-10 [1] CRAN (R 4.3.1)
##     pixmap                               0.4-12         2021-01-29 [1] CRAN (R 4.3.0)
##     pkgbuild                             1.4.3          2023-12-10 [1] CRAN (R 4.3.1)
##     pkgconfig                            2.0.3          2019-09-22 [1] CRAN (R 4.3.0)
##     pkgdown                              2.0.7          2022-12-14 [1] CRAN (R 4.3.0)
##     pkgload                              1.3.4          2024-01-16 [1] CRAN (R 4.3.1)
##     pkgnet                               0.4.2          2021-12-23 [1] CRAN (R 4.3.0)
##     plogr                                0.2.0          2018-03-25 [1] CRAN (R 4.3.0)
##     plotly                               4.10.4         2024-01-13 [1] CRAN (R 4.3.1)
##     plotrix                              3.8-4          2023-11-10 [1] CRAN (R 4.3.1)
##     PlotTools                            0.3.0          2023-10-30 [1] CRAN (R 4.3.1)
##     pluralize                            0.2.0          2020-06-09 [1] CRAN (R 4.3.0)
##     plyr                                 1.8.9          2023-10-02 [1] CRAN (R 4.3.1)
##     plyranges                            1.22.0         2023-10-24 [1] Bioconductor
##     PMCMRplus                            1.9.10         2023-12-10 [1] CRAN (R 4.3.1)
##     png                                  0.1-8          2022-11-29 [1] CRAN (R 4.3.0)
##     Polychrome                           1.5.1          2022-05-03 [1] CRAN (R 4.3.0)
##     polyclip                             1.10-6         2023-09-27 [1] CRAN (R 4.3.1)
##     polynom                              1.4-1          2022-04-11 [1] CRAN (R 4.3.0)
##     poweRlaw                             0.80.0         2024-01-25 [1] CRAN (R 4.3.1)
##     pracma                               2.4.4          2023-11-10 [1] CRAN (R 4.3.1)
##     praise                               1.0.0          2015-08-11 [1] CRAN (R 4.3.0)
##     preprocessCore                       1.64.0         2023-10-26 [1] Bioconductor
##     prettyunits                          1.2.0          2023-09-24 [1] CRAN (R 4.3.1)
##     prismatic                            1.1.1          2022-08-15 [1] CRAN (R 4.3.0)
##     pROC                                 1.18.5         2023-11-01 [1] CRAN (R 4.3.1)
##     processx                             3.8.3          2023-12-10 [1] CRAN (R 4.3.1)
##     prodlim                              2023.08.28     2023-08-28 [1] CRAN (R 4.3.0)
##     profvis                              0.3.8          2023-05-02 [1] CRAN (R 4.3.0)
##     progress                             1.2.3          2023-12-06 [1] CRAN (R 4.3.1)
##     progressr                            0.14.0         2023-08-10 [1] CRAN (R 4.3.0)
##     promises                             1.2.1          2023-08-10 [1] CRAN (R 4.3.0)
##     ProtGenerics                         1.34.0         2023-10-26 [1] Bioconductor
##     proxy                                0.4-27         2022-06-09 [1] CRAN (R 4.3.0)
##     ps                                   1.7.6          2024-01-18 [1] CRAN (R 4.3.1)
##     pscl                                 1.5.9          2024-01-31 [1] CRAN (R 4.3.1)
##     pubmedR                              0.0.3          2020-07-09 [1] CRAN (R 4.3.0)
##     purrr                                1.0.2          2023-08-10 [1] CRAN (R 4.3.0)
##     qap                                  0.1-2          2022-06-27 [1] CRAN (R 4.3.0)
##     qlcMatrix                            0.9.7          2018-04-20 [1] CRAN (R 4.3.0)
##     qpdf                                 1.3.2          2023-03-17 [1] CRAN (R 4.3.0)
##     quadprog                             1.5-8          2019-11-20 [1] CRAN (R 4.3.0)
##     Quandl                               2.11.0         2021-08-11 [1] CRAN (R 4.3.0)
##     quantmod                             0.4.26         2024-02-14 [1] CRAN (R 4.3.1)
##     quantreg                             5.97           2023-08-19 [1] CRAN (R 4.3.0)
##     quartificate                         0.0.0.9000     2024-03-08 [1] Github (ropenscilabs/quartificate@bed4c63)
##     quarto                               1.4            2024-03-06 [1] CRAN (R 4.3.1)
##     qvalue                               2.34.0         2023-10-26 [1] Bioconductor
##     R.cache                              0.16.0         2022-07-21 [1] CRAN (R 4.3.0)
##     R.methodsS3                          1.8.2          2022-06-13 [1] CRAN (R 4.3.0)
##     R.oo                                 1.26.0         2024-01-24 [1] CRAN (R 4.3.1)
##     R.utils                              2.12.3         2023-11-18 [1] CRAN (R 4.3.1)
##     R6                                   2.5.1          2021-08-19 [1] CRAN (R 4.3.0)
##     ragg                                 1.3.0          2024-03-13 [1] CRAN (R 4.3.1)
##     RANN                                 2.6.1          2019-01-08 [1] CRAN (R 4.3.0)
##     rappdirs                             0.3.3          2021-01-31 [1] CRAN (R 4.3.0)
##     raster                               3.6-26         2023-10-14 [1] CRAN (R 4.3.1)
##     ratelimitr                           0.4.1          2018-10-07 [1] CRAN (R 4.3.0)
##     RBGL                                 1.78.0         2023-10-26 [1] Bioconductor
##     rbibutils                            2.2.16         2023-10-25 [1] CRAN (R 4.3.1)
##     RCircos                              1.2.2          2021-12-19 [1] CRAN (R 4.3.0)
##     rcmdcheck                            1.4.0          2021-09-27 [1] CRAN (R 4.3.0)
##     RColorBrewer                         1.1-3          2022-04-03 [1] CRAN (R 4.3.0)
##     Rcpp                                 1.0.12         2024-01-09 [1] CRAN (R 4.3.1)
##     RcppAnnoy                            0.0.22         2024-01-23 [1] CRAN (R 4.3.1)
##     RcppArmadillo                        0.12.8.1.0     2024-03-03 [1] CRAN (R 4.3.1)
##     RcppCCTZ                             0.2.12         2022-11-06 [1] CRAN (R 4.3.0)
##     RcppDate                             0.0.3          2021-05-19 [1] CRAN (R 4.3.0)
##     RcppDE                               0.1.7          2022-12-20 [1] CRAN (R 4.3.0)
##     RcppDist                             0.1.1          2018-10-28 [1] CRAN (R 4.3.0)
##     RcppEigen                            0.3.4.0.0      2024-02-28 [1] CRAN (R 4.3.1)
##     RcppGSL                              0.3.13         2023-01-13 [1] CRAN (R 4.3.0)
##     RcppHNSW                             0.6.0          2024-02-04 [1] CRAN (R 4.3.1)
##     RcppInt64                            0.0.4          2023-12-09 [1] CRAN (R 4.3.1)
##     RcppParallel                         5.1.7          2023-02-27 [1] CRAN (R 4.3.0)
##     RcppProgress                         0.4.2          2020-02-06 [1] CRAN (R 4.3.0)
##     RcppRoll                             0.3.0          2018-06-05 [1] CRAN (R 4.3.0)
##     RcppSpdlog                           0.0.16         2024-01-12 [1] CRAN (R 4.3.1)
##     RcppTOML                             0.2.2          2023-01-29 [1] CRAN (R 4.3.0)
##     RcppZiggurat                         0.1.6          2020-10-20 [1] CRAN (R 4.3.0)
##     RCurl                                1.98-1.14      2024-01-09 [1] CRAN (R 4.3.1)
##     Rdiagnosislist                       1.2            2023-04-18 [1] CRAN (R 4.3.0)
##     Rdimtools                            1.1.2          2022-12-15 [1] CRAN (R 4.3.0)
##     Rdpack                               2.6            2023-11-08 [1] CRAN (R 4.3.1)
##     readr                                2.1.5          2024-01-10 [1] CRAN (R 4.3.1)
##     readxl                               1.4.3          2023-07-06 [1] CRAN (R 4.3.0)
##     recipes                              1.0.10         2024-02-18 [1] CRAN (R 4.3.1)
##     reghelper                            1.1.2          2023-09-02 [1] CRAN (R 4.3.0)
##     regioneR                             1.34.0         2023-10-26 [1] Bioconductor
##     registry                             0.5-1          2019-03-05 [1] CRAN (R 4.3.0)
##     remaCor                              0.0.18         2024-02-08 [1] CRAN (R 4.3.1)
##     rematch                              2.0.0          2023-08-30 [1] CRAN (R 4.3.0)
##     rematch2                             2.1.2          2020-05-01 [1] CRAN (R 4.3.0)
##     remotes                              2.4.2.9000     2023-11-17 [1] Github (r-lib/remotes@6fe8836)
##     rentrez                              1.2.3          2020-11-10 [1] CRAN (R 4.3.0)
##     renv                                 1.0.5          2024-02-29 [1] CRAN (R 4.3.1)
##     repmis                               0.5            2016-02-07 [1] CRAN (R 4.3.0)
##     reprex                               2.1.0          2024-01-11 [1] CRAN (R 4.3.1)
##     reshape                              0.8.9          2022-04-12 [1] CRAN (R 4.3.0)
##     reshape2                             1.4.4          2020-04-09 [1] CRAN (R 4.3.0)
##     ResidualMatrix                       1.12.0         2023-10-24 [1] Bioconductor
##     restfulr                             0.0.15         2022-06-16 [1] CRAN (R 4.3.0)
##     reticulate                           1.35.0         2024-01-31 [1] CRAN (R 4.3.1)
##     rex                                  1.2.1          2021-11-26 [1] CRAN (R 4.3.0)
##     Rfast                                2.1.0          2023-11-09 [1] CRAN (R 4.3.1)
##     rgl                                  1.3.1          2024-03-05 [1] CRAN (R 4.3.1)
##     Rgraphviz                            2.46.0         2023-10-26 [1] Bioconductor
##     rhdf5                                2.46.1         2023-12-02 [1] Bioconductor 3.18 (R 4.3.2)
##     rhdf5filters                         1.14.1         2023-11-06 [1] Bioconductor
##     Rhdf5lib                             1.24.2         2024-02-10 [1] Bioconductor 3.18 (R 4.3.2)
##     RhpcBLASctl                          0.23-42        2023-02-11 [1] CRAN (R 4.3.0)
##     Rhtslib                              2.4.1          2024-01-20 [1] Bioconductor 3.18 (R 4.3.2)
##     riingo                               0.3.1          2020-09-12 [1] CRAN (R 4.3.0)
##     RISmed                               2.3.0          2021-07-05 [1] CRAN (R 4.3.0)
##     ritis                                1.0.0          2021-02-02 [1] CRAN (R 4.3.0)
##     rJava                                1.0-11         2024-01-26 [1] CRAN (R 4.3.1)
##     rjson                                0.2.21         2022-01-09 [1] CRAN (R 4.3.0)
##     RJSONIO                              1.3-1.9        2023-11-27 [1] CRAN (R 4.3.1)
##     rlang                                1.1.3          2024-01-10 [1] CRAN (R 4.3.1)
##     rlist                                0.4.6.2        2021-09-03 [1] CRAN (R 4.3.0)
##     rmarkdown                            2.26           2024-03-05 [1] CRAN (R 4.3.1)
##     rmio                                 0.4.0          2022-02-17 [1] CRAN (R 4.3.0)
##     Rmpfr                                0.9-5          2024-01-21 [1] CRAN (R 4.3.1)
##     RMySQL                               0.10.27        2023-12-04 [1] CRAN (R 4.3.1)
##     rncl                                 0.8.7          2023-01-08 [1] CRAN (R 4.3.0)
##     RNeXML                               2.4.11         2023-02-01 [1] CRAN (R 4.3.0)
##     RNOmni                               1.0.1.2        2023-09-11 [1] CRAN (R 4.3.0)
##     ROCR                                 1.0-11         2020-05-02 [1] CRAN (R 4.3.0)
##     rols                                 2.30.2         2024-02-17 [1] Bioconductor 3.18 (R 4.3.2)
##     ROMOP                                0.3.0          2023-11-16 [1] Github (BenGlicksberg/ROMOP@dc37ea9)
##     rootSolve                            1.8.2.4        2023-09-21 [1] CRAN (R 4.3.1)
##     rorcid                               0.7.0          2021-01-20 [1] CRAN (R 4.3.0)
##     rotl                                 3.1.0          2023-06-15 [1] CRAN (R 4.3.0)
##     roxygen2                             7.3.1          2024-01-22 [1] CRAN (R 4.3.1)
##     rpart                                4.1.23         2023-12-05 [1] CRAN (R 4.3.1)
##     rphenoscape                          0.3.0          2024-01-26 [1] Github (phenoscape/rphenoscape@5842b56)
##     rphylopic                            1.3.0          2023-12-20 [1] CRAN (R 4.3.1)
##     rprojroot                            2.0.4          2023-11-05 [1] CRAN (R 4.3.1)
##     rredlist                             0.7.1          2022-11-11 [1] CRAN (R 4.3.0)
##     rsample                              1.2.0          2023-08-23 [1] CRAN (R 4.3.0)
##     Rsamtools                            2.18.0         2023-10-26 [1] Bioconductor
##     rsconnect                            1.2.1          2024-01-31 [1] CRAN (R 4.3.1)
##     rscopus                              0.6.6          2019-09-17 [1] CRAN (R 4.3.0)
##     RSpectra                             0.16-1         2022-04-24 [1] CRAN (R 4.3.0)
##     RSQLite                              2.3.5          2024-01-21 [1] CRAN (R 4.3.1)
##     rstackdeque                          1.1.1          2015-04-13 [1] CRAN (R 4.3.0)
##     rstatix                              0.7.2          2023-02-01 [1] CRAN (R 4.3.0)
##     rstudioapi                           0.15.0         2023-07-07 [1] CRAN (R 4.3.0)
##     rsvd                                 1.0.5          2021-04-16 [1] CRAN (R 4.3.0)
##     rsvg                                 2.6.0          2023-10-08 [1] CRAN (R 4.3.1)
##     rtracklayer                          1.62.0         2023-10-26 [1] Bioconductor
##     Rtsne                                0.17           2023-12-07 [1] CRAN (R 4.3.1)
##     RUnit                                0.4.33         2024-02-22 [1] CRAN (R 4.3.1)
##     rvcheck                              0.2.1          2021-10-22 [1] CRAN (R 4.3.0)
##     rversions                            2.1.2          2022-08-31 [1] CRAN (R 4.3.0)
##     rvest                                1.0.4          2024-02-12 [1] CRAN (R 4.3.1)
##     rworkflows                           1.0.1          2024-01-03 [1] Bioconductor
##     s2                                   1.1.6          2023-12-19 [1] CRAN (R 4.3.1)
##     S4Arrays                             1.2.1          2024-03-05 [1] Bioconductor 3.18 (R 4.3.2)
##     S4Vectors                            0.40.2         2023-11-25 [1] Bioconductor 3.18 (R 4.3.2)
##     safetensors                          0.1.2          2023-09-12 [1] CRAN (R 4.3.0)
##     sandwich                             3.1-0          2023-12-11 [1] CRAN (R 4.3.1)
##     sass                                 0.4.8          2023-12-06 [1] CRAN (R 4.3.1)
##     SAVER                                1.1.2          2019-11-13 [1] CRAN (R 4.3.0)
##     ScaledMatrix                         1.10.0         2023-10-24 [1] Bioconductor
##     scales                               1.3.0          2023-11-28 [1] CRAN (R 4.3.1)
##     scattermore                          1.2            2023-06-12 [1] CRAN (R 4.3.0)
##     scatterpie                           0.2.1          2023-06-07 [1] CRAN (R 4.3.0)
##     scatterplot3d                        0.3-44         2023-05-05 [1] CRAN (R 4.3.0)
##     sceasy                               0.0.7          2023-10-10 [1] Github (cellgeni/sceasy@0cfc0e3)
##     scKirby                              0.1.4          2023-11-29 [1] Bioconductor
##     scNLP                                0.1.2          2023-10-10 [1] Github (neurogenomics/scNLP@db0dddd)
##     scOntoMatch                          0.1.1          2023-10-27 [1] CRAN (R 4.3.1)
##     SCopeLoomR                           0.13.0         2023-10-10 [1] Github (aertslab/SCopeLoomR@20f4e0a)
##     scs                                  3.2.4          2023-04-11 [1] CRAN (R 4.3.0)
##     sctransform                          0.4.1          2023-10-19 [1] CRAN (R 4.3.1)
##     scuttle                              1.12.0         2023-10-24 [1] Bioconductor
##     secretbase                           0.3.0.1        2024-03-01 [1] CRAN (R 4.3.1)
##     segmented                            2.0-3          2024-02-16 [1] CRAN (R 4.3.1)
##     selectr                              0.4-2          2019-11-20 [1] CRAN (R 4.3.0)
##     seqinr                               4.2-36         2023-12-08 [1] CRAN (R 4.3.1)
##     seqLogo                              1.68.0         2023-10-26 [1] Bioconductor
##     seqminer                             9.4            2024-02-03 [1] CRAN (R 4.3.1)
##     seqPattern                           1.34.0         2023-10-26 [1] Bioconductor
##     seriation                            1.5.4          2023-12-12 [1] CRAN (R 4.3.1)
##     servr                                0.29           2024-02-09 [1] CRAN (R 4.3.1)
##     sessioninfo                          1.2.2          2021-12-06 [1] CRAN (R 4.3.0)
##     Seurat                               5.0.2          2024-02-29 [1] CRAN (R 4.3.1)
##     SeuratDisk                           0.0.0.9020     2023-10-10 [1] Github (mojaveazure/seurat-disk@9b89970)
##     SeuratObject                         5.0.1          2023-11-17 [1] CRAN (R 4.3.1)
##     SeuratWrappers                       0.3.4          2024-03-07 [1] Github (satijalab/seurat-wrappers@d9594f6)
##     sf                                   1.0-15         2023-12-18 [1] CRAN (R 4.3.1)
##     shadowtext                           0.1.3          2024-01-19 [1] CRAN (R 4.3.1)
##     shape                                1.4.6.1        2024-02-23 [1] CRAN (R 4.3.1)
##     shapes                               1.2.7          2023-02-03 [1] CRAN (R 4.3.0)
##     shiny                                1.8.0          2023-11-17 [1] CRAN (R 4.3.1)
##     shinycssloaders                      1.0.0          2020-07-28 [1] CRAN (R 4.3.0)
##     shinydashboard                       0.7.2          2021-09-30 [1] CRAN (R 4.3.0)
##     shinydashboardPlus                   2.0.4.9000     2023-10-12 [1] Github (RinteRface/shinydashboardPlus@96d0150)
##     shinyjqui                            0.4.1          2022-02-03 [1] CRAN (R 4.3.0)
##     shinyjs                              2.1.0          2021-12-23 [1] CRAN (R 4.3.0)
##     shinythemes                          1.2.0          2021-01-25 [1] CRAN (R 4.3.0)
##     shinyWidgets                         0.8.2          2024-03-01 [1] CRAN (R 4.3.1)
##     showtext                             0.9-7          2024-03-02 [1] CRAN (R 4.3.1)
##     showtextdb                           3.0            2020-06-04 [1] CRAN (R 4.3.0)
##     Signac                               1.12.0         2023-11-08 [1] CRAN (R 4.3.1)
##     simona                               1.0.10         2024-02-06 [1] Bioconductor 3.18 (R 4.3.2)
##     SingleCellExperiment                 1.24.0         2023-10-24 [1] Bioconductor
##     sitmo                                2.0.2          2021-10-13 [1] CRAN (R 4.3.0)
##     slam                                 0.1-50         2022-01-08 [1] CRAN (R 4.3.0)
##     slider                               0.3.1          2023-10-12 [1] CRAN (R 4.3.1)
##     sna                                  2.7-2          2023-12-06 [1] CRAN (R 4.3.1)
##     snow                                 0.4-4          2021-10-27 [1] CRAN (R 4.3.0)
##     SnowballC                            0.7.1          2023-04-25 [1] CRAN (R 4.3.0)
##     SNPlocs.Hsapiens.dbSNP144.GRCh37     0.99.20        2023-10-20 [1] Bioconductor
##     SNPlocs.Hsapiens.dbSNP144.GRCh38     0.99.20        2023-10-20 [1] Bioconductor
##     snpStats                             1.52.0         2023-10-26 [1] Bioconductor
##     solrium                              1.2.0          2021-05-19 [1] CRAN (R 4.3.0)
##     sourcetools                          0.1.7-1        2023-02-01 [1] CRAN (R 4.3.0)
##     sp                                   2.1-3          2024-01-30 [1] CRAN (R 4.3.1)
##     spam                                 2.10-0         2023-10-23 [1] CRAN (R 4.3.1)
##     sparklyr                             1.8.4          2023-10-30 [1] CRAN (R 4.3.1)
##     SparseArray                          1.2.4          2024-02-10 [1] Bioconductor 3.18 (R 4.3.2)
##     SparseM                              1.81           2021-02-18 [1] CRAN (R 4.3.0)
##     sparseMatrixStats                    1.14.0         2023-10-26 [1] Bioconductor
##     sparsesvd                            0.2-2          2023-01-14 [1] CRAN (R 4.3.0)
##     spatial                              7.3-17         2023-07-20 [1] CRAN (R 4.3.0)
##     spatstat.data                        3.0-4          2024-01-15 [1] CRAN (R 4.3.1)
##     spatstat.explore                     3.2-6          2024-02-01 [1] CRAN (R 4.3.1)
##     spatstat.geom                        3.2-9          2024-02-28 [1] CRAN (R 4.3.1)
##     spatstat.random                      3.2-3          2024-02-29 [1] CRAN (R 4.3.1)
##     spatstat.sparse                      3.0-3          2023-10-24 [1] CRAN (R 4.3.1)
##     spatstat.utils                       3.0-4          2023-10-24 [1] CRAN (R 4.3.1)
##     spData                               2.3.0          2023-07-06 [1] CRAN (R 4.3.0)
##     spdep                                1.3-3          2024-02-07 [1] CRAN (R 4.3.1)
##     spdl                                 0.0.5          2023-06-18 [1] CRAN (R 4.3.0)
##     speedglm                             0.3-5          2023-05-06 [1] Github (cran/speedglm@1e34560)
##     splicejam                            0.0.77.900     2023-10-12 [1] Github (jmw86069/splicejam@04d7c2d)
##     splines                              4.3.1          2023-06-16 [?] local
##     splitstackshape                      1.4.8          2019-04-21 [1] CRAN (R 4.3.0)
##     SqlRender                            1.16.1         2023-10-07 [1] CRAN (R 4.3.1)
##     SQUAREM                              2021.1         2021-01-13 [1] CRAN (R 4.3.0)
##     statmod                              1.5.0          2023-01-06 [1] CRAN (R 4.3.0)
##     statnet.common                       4.9.0          2023-05-24 [1] CRAN (R 4.3.0)
##   P stats                              * 4.3.1          2023-06-16 [1] local
##     stats4                               4.3.1          2023-06-16 [?] local
##     statsExpressions                     1.5.3          2024-01-13 [1] CRAN (R 4.3.1)
##     stopwords                            2.3            2021-10-28 [1] CRAN (R 4.3.0)
##     stringdist                           0.9.12         2023-11-28 [1] CRAN (R 4.3.1)
##     stringi                              1.8.3          2023-12-11 [1] CRAN (R 4.3.1)
##     stringr                              1.5.1          2023-11-14 [1] CRAN (R 4.3.1)
##     styler                               1.10.2         2023-08-29 [1] CRAN (R 4.3.0)
##     SummarizedExperiment                 1.32.0         2023-10-24 [1] Bioconductor
##     SuppDists                            1.1-9.7        2022-01-03 [1] CRAN (R 4.3.0)
##     supraHex                             1.40.0         2023-10-26 [1] Bioconductor
##     survival                             3.5-8          2024-02-14 [1] CRAN (R 4.3.1)
##     susieR                               0.12.35        2023-02-17 [1] CRAN (R 4.3.0)
##     svglite                              2.1.3          2023-12-08 [1] CRAN (R 4.3.1)
##     sys                                  3.4.2          2023-05-23 [1] CRAN (R 4.3.0)
##     sysfonts                             0.8.9          2024-03-02 [1] CRAN (R 4.3.1)
##     sysreqs                              1.0.0.9000     2024-01-22 [1] Github (r-hub/sysreqs@f068afa)
##     systemfonts                          1.0.6          2024-03-07 [1] CRAN (R 4.3.1)
##     targets                              1.6.0          2024-03-13 [1] CRAN (R 4.3.1)
##     taxize                               0.9.100        2022-04-22 [1] CRAN (R 4.3.0)
##     tcltk                                4.3.1          2023-06-16 [?] local
##     templateR                            0.99.0         2023-12-09 [1] local
##     tensor                               1.5            2012-05-05 [1] CRAN (R 4.3.0)
##     tensorflow                           2.15.0         2024-01-31 [1] CRAN (R 4.3.1)
##     terra                                1.7-71         2024-01-31 [1] CRAN (R 4.3.1)
##     testthat                             3.2.1          2023-12-02 [1] CRAN (R 4.3.1)
##     textnets                             0.1.1          2023-10-06 [1] Github (cbail/textnets@42d2366)
##     textshaping                          0.3.7          2023-10-09 [1] CRAN (R 4.3.1)
##     textutils                            0.3-2          2023-04-01 [1] CRAN (R 4.3.0)
##     tfautograph                          0.3.2          2021-09-17 [1] CRAN (R 4.3.0)
##     TFBSTools                            1.40.0         2023-10-24 [1] Bioconductor
##     TFMPvalue                            0.0.9          2022-10-21 [1] CRAN (R 4.3.0)
##     tfruns                               1.5.2          2024-01-26 [1] CRAN (R 4.3.1)
##     TH.data                              1.1-2          2023-04-17 [1] CRAN (R 4.3.0)
##     thesis                               0.98.0         2023-10-23 [1] local
##     threed                               0.1.2          2023-10-06 [1] Github (coolbutuseless/threed@35d1085)
##     tibble                               3.2.1          2023-03-20 [1] CRAN (R 4.3.0)
##     tidygraph                            1.3.1          2024-01-30 [1] CRAN (R 4.3.1)
##     tidyjson                             0.3.2          2023-01-07 [1] CRAN (R 4.3.0)
##     tidymodels                           1.1.1          2023-08-24 [1] CRAN (R 4.3.0)
##     tidypmc                              1.7            2019-08-01 [1] CRAN (R 4.3.0)
##     tidyquant                            1.0.7          2023-03-31 [1] CRAN (R 4.3.0)
##     tidyr                                1.3.1          2024-01-24 [1] CRAN (R 4.3.1)
##     tidyselect                           1.2.1          2024-03-11 [1] CRAN (R 4.3.1)
##     tidytext                             0.4.1          2023-01-07 [1] CRAN (R 4.3.0)
##     tidytree                             0.4.6          2023-12-12 [1] CRAN (R 4.3.1)
##     tidyverse                            2.0.0          2023-02-22 [1] CRAN (R 4.3.0)
##     tiledb                               0.24.0         2024-02-22 [1] CRAN (R 4.3.1)
##   R tiledbsoma                           <NA>           <NA>       [?] <NA>
##     timechange                           0.3.0          2024-01-18 [1] CRAN (R 4.3.1)
##     timeDate                             4032.109       2023-12-14 [1] CRAN (R 4.3.1)
##     timetk                               2.9.0          2023-10-31 [1] CRAN (R 4.3.1)
##     tinytex                              0.49           2023-11-22 [1] CRAN (R 4.3.1)
##     tm                                   0.7-12         2024-03-11 [1] CRAN (R 4.3.1)
##     tokenizers                           0.3.0          2022-12-22 [1] CRAN (R 4.3.0)
##   P tools                                4.3.1          2023-06-16 [1] local
##     topGO                                2.54.0         2023-10-26 [1] Bioconductor
##     torch                                0.12.0         2023-12-15 [1] CRAN (R 4.3.1)
##     torchaudio                           0.3.1          2023-02-08 [1] CRAN (R 4.3.0)
##     torchvision                          0.5.1          2023-04-14 [1] CRAN (R 4.3.0)
##     trackdown                            1.1.1          2021-12-19 [1] CRAN (R 4.3.0)
##     treeio                               1.26.0         2023-10-24 [1] Bioconductor
##     TreeTools                            1.10.0         2023-08-19 [1] CRAN (R 4.3.0)
##     triebeard                            0.4.1          2023-03-04 [1] CRAN (R 4.3.0)
##     tseries                              0.10-55        2023-12-06 [1] CRAN (R 4.3.1)
##     tsfeatures                           1.1.1          2023-08-28 [1] CRAN (R 4.3.0)
##     TSP                                  1.2-4          2023-04-04 [1] CRAN (R 4.3.0)
##     TTR                                  0.24.4         2023-11-28 [1] CRAN (R 4.3.1)
##     tufte                                0.13           2023-06-22 [1] CRAN (R 4.3.0)
##     tune                                 1.1.2          2023-08-23 [1] CRAN (R 4.3.0)
##     tweenr                               2.0.3          2024-02-26 [1] CRAN (R 4.3.1)
##     TxDb.Hsapiens.UCSC.hg19.knownGene    3.2.2          2023-10-13 [1] Bioconductor
##     TxDb.Hsapiens.UCSC.hg38.knownGene    3.18.0         2023-10-19 [1] Bioconductor
##     TxDb.Mmusculus.UCSC.mm10.knownGene   3.10.0         2023-10-13 [1] Bioconductor
##     TxDb.Mmusculus.UCSC.mm9.knownGene    3.2.2          2023-10-13 [1] Bioconductor
##     tzdb                                 0.4.0          2023-05-12 [1] CRAN (R 4.3.0)
##     udpipe                               0.8.11         2023-01-06 [1] CRAN (R 4.3.0)
##     umap                                 0.2.10.0       2023-02-01 [1] CRAN (R 4.3.0)
##     units                                0.8-5          2023-11-28 [1] CRAN (R 4.3.1)
##     UpSetR                               1.4.0          2019-05-22 [1] CRAN (R 4.3.0)
##     urca                                 1.3-3          2022-08-29 [1] CRAN (R 4.3.0)
##     urlchecker                           1.0.1          2021-11-30 [1] CRAN (R 4.3.0)
##     urltools                             1.7.3          2019-04-14 [1] CRAN (R 4.3.0)
##     usethis                              2.2.3          2024-02-19 [1] CRAN (R 4.3.1)
##     utf8                                 1.2.4          2023-10-22 [1] CRAN (R 4.3.1)
##   P utils                              * 4.3.1          2023-06-16 [1] local
##     uuid                                 1.2-0          2024-01-14 [1] CRAN (R 4.3.1)
##     uwot                                 0.1.16         2023-06-29 [1] CRAN (R 4.3.0)
##     V8                                   4.4.2          2024-02-15 [1] CRAN (R 4.3.1)
##     VarfromPDB                           2.2.10         2018-09-13 [1] CRAN (R 4.3.0)
##     variancePartition                    1.32.5         2024-02-17 [1] Bioconductor 3.18 (R 4.3.2)
##     VariantAnnotation                    1.48.1         2023-11-18 [1] Bioconductor 3.18 (R 4.3.2)
##     vcr                                  1.2.2          2023-06-25 [1] CRAN (R 4.3.0)
##     vctrs                                0.6.5          2023-12-01 [1] CRAN (R 4.3.1)
##     vegan                                2.6-4          2022-10-11 [1] CRAN (R 4.3.0)
##     VGAM                                 1.1-10         2024-02-29 [1] CRAN (R 4.3.1)
##     vipor                                0.4.7          2023-12-18 [1] CRAN (R 4.3.1)
##     viridis                              0.6.5          2024-01-29 [1] CRAN (R 4.3.1)
##     viridisLite                          0.4.2          2023-05-02 [1] CRAN (R 4.3.0)
##     visNetwork                           2.1.2          2022-09-29 [1] CRAN (R 4.3.0)
##     vroom                                1.6.5          2023-12-05 [1] CRAN (R 4.3.1)
##     waiter                               0.2.5          2022-01-03 [1] CRAN (R 4.3.0)
##     waldo                                0.5.2          2023-11-02 [1] CRAN (R 4.3.1)
##     warp                                 0.2.1          2023-11-02 [1] CRAN (R 4.3.1)
##     webmockr                             0.9.0          2023-02-28 [1] CRAN (R 4.3.0)
##     webshot                              0.5.5          2023-06-26 [1] CRAN (R 4.3.0)
##     webshot2                             0.1.1          2023-08-11 [1] CRAN (R 4.3.0)
##     websocket                            1.4.1          2021-08-18 [1] CRAN (R 4.3.0)
##     wesanderson                          0.3.7          2023-10-31 [1] CRAN (R 4.3.1)
##     WGCNA                                1.72-5         2023-12-07 [1] CRAN (R 4.3.1)
##     whisker                              0.4.1          2022-12-05 [1] CRAN (R 4.3.0)
##     WikidataQueryServiceR                1.0.0          2020-06-16 [1] CRAN (R 4.3.0)
##     WikidataR                            2.3.3          2021-11-16 [1] CRAN (R 4.3.0)
##     WikipediR                            1.5.0          2017-02-05 [1] CRAN (R 4.3.0)
##     wikitaxa                             0.4.0          2020-06-29 [1] CRAN (R 4.3.0)
##     withr                                3.0.0          2024-01-16 [1] CRAN (R 4.3.1)
##     wk                                   0.9.1          2023-11-29 [1] CRAN (R 4.3.1)
##     workflows                            1.1.4          2024-02-19 [1] CRAN (R 4.3.1)
##     workflowsets                         1.0.1          2023-04-06 [1] CRAN (R 4.3.0)
##     worrms                               0.4.3          2023-06-20 [1] CRAN (R 4.3.0)
##     writexl                              1.5.0          2024-02-09 [1] CRAN (R 4.3.1)
##     WRS2                                 1.1-6          2024-03-15 [1] CRAN (R 4.3.1)
##     xfun                                 0.42           2024-02-08 [1] CRAN (R 4.3.1)
##     xgboost                              1.7.7.1        2024-01-25 [1] CRAN (R 4.3.1)
##     XGR                                  1.1.9          2023-09-20 [1] Github (hfang-bristol/XGR@7b94708)
##     xlsx                                 0.6.5          2020-11-10 [1] CRAN (R 4.3.0)
##     xlsxjars                             0.6.1          2014-08-22 [1] CRAN (R 4.3.0)
##     XML                                  3.99-0.16.1    2024-01-22 [1] CRAN (R 4.3.1)
##     xml2                                 1.3.6          2023-12-04 [1] CRAN (R 4.3.1)
##     XML2R                                0.0.6          2014-03-10 [1] CRAN (R 4.3.0)
##     xmlconvert                           0.1.2          2021-03-27 [1] CRAN (R 4.3.0)
##     xmlparsedata                         1.0.5          2021-03-06 [1] CRAN (R 4.3.0)
##     xopen                                1.0.0          2018-09-17 [1] CRAN (R 4.3.0)
##     xtable                               1.8-4          2019-04-21 [1] CRAN (R 4.3.0)
##     xts                                  0.13.2         2024-01-21 [1] CRAN (R 4.3.1)
##     XVector                              0.42.0         2023-10-26 [1] Bioconductor
##     yaml                                 2.3.8          2023-12-11 [1] CRAN (R 4.3.1)
##     yardstick                            1.3.0          2024-01-19 [1] CRAN (R 4.3.1)
##     yesno                                0.1.2          2020-07-10 [1] CRAN (R 4.3.0)
##     yulab.utils                          0.1.4          2024-01-28 [1] CRAN (R 4.3.1)
##     zeallot                              0.1.0          2018-01-28 [1] CRAN (R 4.3.0)
##     zellkonverter                        1.12.1         2023-11-14 [1] Bioconductor
##     zip                                  2.3.1          2024-01-27 [1] CRAN (R 4.3.1)
##     zlibbioc                             1.48.0         2023-10-26 [1] Bioconductor
##     zoo                                  1.8-12         2023-04-13 [1] CRAN (R 4.3.0)
##  
##   [1] /Library/Frameworks/R.framework/Versions/4.3-arm64/Resources/library
##  
##   P ── Loaded and on-disk path mismatch.
##   R ── Package was removed from disk.
##  
##  ─ Python configuration ────────────────────────────────────────────────────
##   Python is not available
##  
##  ───────────────────────────────────────────────────────────────────────────
```
:::



:::
