# CrimeAndDynamicPanelData

# Motivation
The findings of this [study](study|https://www.ifo.de/publikationen/2025/aufsatz-zeitschrift/steigert-migration-die-kriminalitaet-ein-datenbasierter-blick) by the ifo institute [were](https://www.zdf.de/nachrichten/politik/deutschland/auslaender-kriminalitaet-studie-ifo-polizeiliche-kriminalstatistik-100.html) [reported](https://www.dw.com/en/study-finds-immigration-has-not-raised-german-crime-rate/a-71691228) [widely](https://www.reuters.com/world/europe/higher-proportion-migrants-does-not-mean-more-crime-german-institute-says-2025-02-18/) and generated a lot of [discussion](https://www.reddit.com/r/Wirtschaftsweise/comments/1ivsimq/das_problem_mit_der_migration_f%C3%BChrt_nicht_zu_mehr/).
Inspired by the research of Lange et. al 2024 which found a positive impact of migration on crime after including a lag of one year I want to analyze, whether including a lag introduces a causal relationship between crime and migration. Furthermore, I want to analyse non-linear and context specific effects leading to an increased crime rate.

# Methodology
This approach needs methods specific to dynamic panel data. We consider crime at t-1 as a lagged indicator and t-2 as a deeper lagged indicator serving as the IV. I use the Arellano and Bond estimator. For the second research question a causal forest will be used.

# Data Source
Destatis and PKS tables from BKA. All data is district level ranging from 2018 to 2023.
