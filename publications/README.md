# Publications Catalog

> A curated bibliography for **Awesome Mosquito Acoustics**, covering mosquito acoustic biology, sensing, datasets, AI recognition, and related bioacoustic methods.

## Scope and verification

- **65 seed references** were transcribed from the bibliography of the supplied review manuscript (dated 10 November 2026). This is a **seed catalog**, not an exhaustive or systematic literature search.
- Every record retains its original citation text and review reference number in [`papers.csv`](papers.csv). The source manuscript is not redistributed in this repository.
- `direct-mosquito` denotes work directly concerning mosquitoes (including mosquito surveillance context); `related-bioacoustics` refers to research on other animals/insects or broader bioacoustics; `general-methods` refers to transferable statistical or ML methods. These are curator-assigned categories, not claims of experimental validation.
- **Metadata not independently verified** is labelled `source-transcribed-unverified`. No DOI, public code URL, or dataset URL is fabricated. Selected links have been checked against an authoritative source.
- `references.bib` is a preliminary BibTeX transcription; check author spellings, journal, volume, pagination, DOI and BibTeX entry type against publishers before using it in a manuscript.

## Browse

| Section | Focus |
|---|---|
| [Acoustic Biology](#acoustic-biology) | 8 tagged entries |
| [Behavioural Acoustics](#behavioural-acoustics) | 7 tagged entries |
| [Sensing Technologies](#sensing-technologies) | 11 tagged entries |
| [Traditional Machine Learning](#traditional-machine-learning) | 2 tagged entries |
| [Deep Learning](#deep-learning) | 8 tagged entries |
| [Transfer & Self-Supervised Learning](#transfer--self-supervised-learning) | 8 tagged entries |
| [Domain Generalization](#domain-generalization) | 8 tagged entries |
| [Field Monitoring](#field-monitoring) | 8 tagged entries |
| [Datasets & Benchmarks](#datasets--benchmarks) | 7 tagged entries |
| [Uncertainty & Model Reliability](#uncertainty--model-reliability) | 7 tagged entries |
| [Reviews & Perspectives](#reviews--perspectives) | 11 tagged entries |
| [Ecological Methods (Background)](#ecological-methods-background) | 18 tagged entries |

## Featured resources

- **Mobile-phone mosquito surveillance** — Mukundarajan et al. (2017), *eLife*. [Publisher article](https://doi.org/10.7554/eLife.27854).
- **Cross-domain benchmark** — Hou et al. (2026), *BioDCASE CD-MSC*. [Official task](https://biodcase.github.io/challenge2026/task5) · [Baseline code](https://github.com/Yuanbo2020/CD-MSC).

## Publications by topic

Entries appear in multiple categories when relevant. Titles are transcribed from the manuscript bibliography, with spelling/capitalization preserved pending verification.

### Acoustic Biology

- **2026** · Proximate determinants of the frequency of mosquito sounds: separating species-specific effects from environmentally driven variations-implications for ai species recognition — J. Augustin, S. Zsebők, D. Kovács, Z. Jánki, A. Bánhalmi, Z. Soltész, P. Seffer, V. Bilicki, L. Z. Garamszegi. `[ma-021]` · `direct-mosquito`
- **2024** · Effect of physiological and environmental factors on mosquito wingbeat frequency — D. Kim, T. J. DeBriere, N. D. Burkett-Cadena. `[ma-024]` · `direct-mosquito`
- **2021** · Harmonic convergence coordinates swarm mating by enhancing mate detection in the malaria mosquito anopheles gambiae — S. S. Garcia Castillo, K. S. Pritts, R. S. Krishnan, L. C. Harrington, G. P. League. `[ma-026]` · `direct-mosquito`
- **2020** · Buzzkill: targeting the mosquito auditory system — M. Andrés, M. P. Su, J. Albert, L. J. Cator. `[ma-017]` · `direct-mosquito`
- **2016** · A role for acoustic distortion in novel rapid frequency modulation behaviour in free-flying male mosquitoes — P. M. Simões, R. A. Ingham, G. Gibson, I. J. Russell. `[ma-008]` · `direct-mosquito`
- **2016** · Quantitative analysis of harmonic convergence in mosquito auditory interactions — A. Aldersley, A. Champneys, M. Homer, D. Robert. `[ma-025]` · `direct-mosquito`
- **2014** · Mosquito (aedes aegypti) flight tones: Frequency, harmonicity, spherical spreading, and phase relationships — B. J. Arthur, K. S. Emr, R. A. Wyttenbach, R. R. Hoy. `[ma-006]` · `direct-mosquito`
- **2009** · Harmonic convergence in the love songs of the dengue vector mosquito — L. J. Cator, B. J. Arthur, L. C. Harrington, R. R. Hoy. `[ma-005]` · `direct-mosquito`

### Behavioural Acoustics

- **2021** · Harmonic convergence coordinates swarm mating by enhancing mate detection in the malaria mosquito anopheles gambiae — S. S. Garcia Castillo, K. S. Pritts, R. S. Krishnan, L. C. Harrington, G. P. League. `[ma-026]` · `direct-mosquito`
- **2020** · Buzzkill: targeting the mosquito auditory system — M. Andrés, M. P. Su, J. Albert, L. J. Cator. `[ma-017]` · `direct-mosquito`
- **2018** · Keeping track of mosquitoes: a review of tools to track, record and analyse mosquito flight — J. Spitzen, W. Takken. `[ma-002]` · `direct-mosquito`
- **2016** · Daily rhythms in mosquitoes and their consequences for malaria transmission — S. S. Rund, A. J. O’Donnell, J. E. Gentile, S. E. Reece. `[ma-001]` · `direct-mosquito`
- **2016** · A role for acoustic distortion in novel rapid frequency modulation behaviour in free-flying male mosquitoes — P. M. Simões, R. A. Ingham, G. Gibson, I. J. Russell. `[ma-008]` · `direct-mosquito`
- **2016** · Quantitative analysis of harmonic convergence in mosquito auditory interactions — A. Aldersley, A. Champneys, M. Homer, D. Robert. `[ma-025]` · `direct-mosquito`
- **2009** · Harmonic convergence in the love songs of the dengue vector mosquito — L. J. Cator, B. J. Arthur, L. C. Harrington, R. R. Hoy. `[ma-005]` · `direct-mosquito`

### Sensing Technologies

- **2024** · Field evaluation of an automated mosquito surveillance system which classifies aedes and culex mosquitoes by genus and sex — M. I. González-Pérez, B. Faulhaber, C. Aranda, M. Williams, P. Villalonga, M. Silva, H. Costa Osório, J. Encarnaçao, S. Talavera, N. Busquets. `[ma-004]` · `direct-mosquito`
- **2024** · Monitoring mosquito abundance: Comparing an optical sensor with a trapping method — T. Saha, A. P. Genoud, G. M. Williams, G. J. Russell, B. P. Thomas. `[ma-061]` · `direct-mosquito`
- **2021** · Infrared light sensors permit rapid recording of wingbeat frequency and bioacoustic species identification of mosquitoes — D. Kim, T. J. DeBriere, S. Cherukumalli, G. S. White, N. D. Burkett-Cadena. `[ma-023]` · `direct-mosquito`
- **2021** · Humbug–an acoustic mosquito monitoring tool for use on budget smartphones — M. E. Sinka, D. Zilli, Y. Li, I. Kiskin, D. Msaky, J. Kihonda, G. Mkandawile, E. Kaindoa, G. Killeen, J. Zanga, et al.. `[ma-029]` · `direct-mosquito`
- **2020** · An annotated dataset of bioacoustic sensing and features of mosquitoes — D. Vasconcelos, N. J. Nunes, J. Gomes. `[ma-009]` · `direct-mosquito`
- **2019** · Automated electronic approaches for detecting disease vectors mosquitoes through the wing-beat frequency — D. A. Santos, J. J. Rodrigues, V. Furtado, K. Saleem, V. Korotaev. `[ma-016]` · `direct-mosquito`
- **2018** · Keeping track of mosquitoes: a review of tools to track, record and analyse mosquito flight — J. Spitzen, W. Takken. `[ma-002]` · `direct-mosquito`
- **2018** · Audiomoth: Evaluation of a smart open acoustic device for monitoring biodiversity and the environment — A. P. Hill, P. Prince, E. Piña Covarrubias, C. P. Doncaster, J. L. Snaddon, A. Rogers. `[ma-047]` · `related-bioacoustics`
- **2017** · [Using mobile phones as acoustic sensors for high-throughput mosquito surveillance](https://doi.org/10.7554/eLife.27854) — H. Mukundarajan, F. J. H. Hol, E. A. Castillo, C. Newby, M. Prakash. `[ma-027]` · `direct-mosquito`
- **2016** · Measuring the fundamental frequency and the harmonic properties of the wingbeat of a large number of mosquitoes in flight using 2d optoacoustic sensors — I. Potamitis, I. Rigakis. `[ma-022]` · `direct-mosquito`
- **2014** · Mosquito (aedes aegypti) flight tones: Frequency, harmonicity, spherical spreading, and phase relationships — B. J. Arthur, K. S. Emr, R. A. Wyttenbach, R. R. Hoy. `[ma-006]` · `direct-mosquito`

### Traditional Machine Learning

- **2019** · Automated electronic approaches for detecting disease vectors mosquitoes through the wing-beat frequency — D. A. Santos, J. J. Rodrigues, V. Furtado, K. Saleem, V. Korotaev. `[ma-016]` · `direct-mosquito`
- **2017** · [Using mobile phones as acoustic sensors for high-throughput mosquito surveillance](https://doi.org/10.7554/eLife.27854) — H. Mukundarajan, F. J. H. Hol, E. A. Castillo, C. Newby, M. Prakash. `[ma-027]` · `direct-mosquito`

### Deep Learning

- **2026** · Learning domain-robust bioacoustic representations for mosquito species classification with contrastive learning and distribution alignment — Y. Hou, Z. Liu, X. Shen, S. Roberts. `[ma-032]` · `direct-mosquito`
- **2024** · Mosquitosong+: A noise-robust deep learning model for mosquito classification from wingbeat sounds — A. Supratak, P. Haddawy, M. S. Yin, T. Ziemer, W. Siritanakorn, K. Assawavinijkulchai, K. Chiamsakul, T. Chantanalertvilai, W. Suchalermkul, C. Sa-Ngamuang, et al.. `[ma-035]` · `direct-mosquito`
- **2023** · A deep learning-based pipeline for mosquito detection and classification from wingbeat sounds — M. S. Yin, P. Haddawy, T. Ziemer, F. Wetjen, A. Supratak, K. Chiamsakul, W. Siritanakorn, T. Chantanalertvilai, P. Sriwichai, C. Sa-ngamuang. `[ma-034]` · `direct-mosquito`
- **2022** · A resnet attention model for classifying mosquitoes from wing-beating sounds — X. Wei, M. Z. Hossain, K. A. Ahmed. `[ma-036]` · `direct-mosquito`
- **2021** · Detecting aedes aegypti mosquitoes through audio classification with convolutional neural networks — M. S. Fernandes, W. Cordeiro, M. Recamonde-Mendoza. `[ma-011]` · `direct-mosquito`
- **2021** · Automatic acoustic mosquito tagging with bayesian neural networks — I. Kiskin, A. D. Cobb, M. Sinka, K. Willis, S. J. Roberts. `[ma-012]` · `direct-mosquito`
- **2020** · Bioacoustic detection with wavelet-conditioned convolutional neural networks — I. Kiskin, D. Zilli, Y. Li, M. Sinka, K. Willis, S. Roberts. `[ma-033]` · `direct-mosquito`
- **2018** · Mosquito wingbeat analysis and classification using deep learning — E. Fanioudakis, M. Geismar, I. Potamitis. `[ma-028]` · `direct-mosquito`

### Transfer & Self-Supervised Learning

- **2026** · Learning domain-robust bioacoustic representations for mosquito species classification with contrastive learning and distribution alignment — Y. Hou, Z. Liu, X. Shen, S. Roberts. `[ma-032]` · `direct-mosquito`
- **2026** · Foundation models for bioacoustics–a comparative review — R. Schwinger, P. V. Zadeh, L. Rauch, M. Kurz, T. Hauschild, S. Lapp, S. Tomforde. `[ma-040]` · `related-bioacoustics`
- **2026** · Tweetybert: Automated parsing of birdsong through self-supervised machine learning — G. Vengrovski, M. R. Hulsey-Vincent, M. A. Bemrose, T. J. Gardner. `[ma-043]` · `related-bioacoustics`
- **2024** · Advanced montane bird monitoring using self-supervised learning and transformer on passive acoustic data — Y.-C. Wei, W.-L. Chen, M.-N. Tuanmu, S.-S. Lu, M.-T. Shiao. `[ma-039]` · `related-bioacoustics`
- **2024** · Leveraging transfer learning and active learning for data annotation in passive acoustic monitoring of wildlife — H. Kath, P. P. Serafini, I. B. Campos, T. S. Gouvêa, D. Sonntag. `[ma-042]` · `related-bioacoustics`
- **2023** · Global birdsong embeddings enable superior transfer learning for bioacoustic classification — B. Ghani, T. Denton, S. Kahl, H. Klinck. `[ma-037]` · `related-bioacoustics`
- **2023** · Aves: Animal vocalization encoder based on self-supervision — M. Hagiwara. `[ma-038]` · `related-bioacoustics`
- **2023** · Learning to detect an animal sound from five examples — I. Nolasco, S. Singh, V. Morfi, V. Lostanlen, et al.. `[ma-041]` · `related-bioacoustics`

### Domain Generalization

- **2026** · Proximate determinants of the frequency of mosquito sounds: separating species-specific effects from environmentally driven variations-implications for ai species recognition — J. Augustin, S. Zsebők, D. Kovács, Z. Jánki, A. Bánhalmi, Z. Soltész, P. Seffer, V. Bilicki, L. Z. Garamszegi. `[ma-021]` · `direct-mosquito`
- **2026** · [Biodcase 2026 challenge baseline for cross-domain mosquito species classification](https://biodcase.github.io/challenge2026/task5) — Y. Hou, V. Zdravkovic, M. Sinka, Y. Li, W. Wang, M. D. Plumbley, K. Willis, S. Roberts. `[ma-031]` · `direct-mosquito`
- **2026** · Learning domain-robust bioacoustic representations for mosquito species classification with contrastive learning and distribution alignment — Y. Hou, Z. Liu, X. Shen, S. Roberts. `[ma-032]` · `direct-mosquito`
- **2026** · Foundation models for bioacoustics–a comparative review — R. Schwinger, P. V. Zadeh, L. Rauch, M. Kurz, T. Hauschild, S. Lapp, S. Tomforde. `[ma-040]` · `related-bioacoustics`
- **2026** · Studying domain shifts in bioacoustic recording style between focal and soundscape recordings with acoustic indices — S. Perry, T. Zhang, S. Kamboj, A. Jajodia, D. Tomar, R. Kastner. `[ma-059]` · `related-bioacoustics`
- **2024** · Mosquitosong+: A noise-robust deep learning model for mosquito classification from wingbeat sounds — A. Supratak, P. Haddawy, M. S. Yin, T. Ziemer, W. Siritanakorn, K. Assawavinijkulchai, K. Chiamsakul, T. Chantanalertvilai, W. Suchalermkul, C. Sa-Ngamuang, et al.. `[ma-035]` · `direct-mosquito`
- **2023** · In search for a generalizable method for source free domain adaptation — M. Boudiaf, T. Denton, B. Van Merriënboer, V. Dumoulin, E. Triantafillou. `[ma-060]` · `general-methods`
- **2019** · Can you trust your model’s uncertainty? evaluating predictive uncertainty under dataset shift — Y. Ovadia, et al.. `[ma-045]` · `general-methods`

### Field Monitoring

- **2024** · Field evaluation of an automated mosquito surveillance system which classifies aedes and culex mosquitoes by genus and sex — M. I. González-Pérez, B. Faulhaber, C. Aranda, M. Williams, P. Villalonga, M. Silva, H. Costa Osório, J. Encarnaçao, S. Talavera, N. Busquets. `[ma-004]` · `direct-mosquito`
- **2024** · Monitoring mosquito abundance: Comparing an optical sensor with a trapping method — T. Saha, A. P. Genoud, G. M. Williams, G. J. Russell, B. P. Thomas. `[ma-061]` · `direct-mosquito`
- **2022** · A review of the surveillance techniques for aedes albopictus — Q.-M. Liu, Z.-Y. Gong, Z. Wang. `[ma-003]` · `direct-mosquito`
- **2021** · Humbug–an acoustic mosquito monitoring tool for use on budget smartphones — M. E. Sinka, D. Zilli, Y. Li, I. Kiskin, D. Msaky, J. Kihonda, G. Mkandawile, E. Kaindoa, G. Killeen, J. Zanga, et al.. `[ma-029]` · `direct-mosquito`
- **2019** · Emerging opportunities and challenges for passive acoustics in ecological assessment and monitoring — R. Gibb, E. Browning, P. Glover-Kapfer, K. E. Jones. `[ma-050]` · `related-bioacoustics`
- **2018** · Keeping track of mosquitoes: a review of tools to track, record and analyse mosquito flight — J. Spitzen, W. Takken. `[ma-002]` · `direct-mosquito`
- **2018** · Audiomoth: Evaluation of a smart open acoustic device for monitoring biodiversity and the environment — A. P. Hill, P. Prince, E. Piña Covarrubias, C. P. Doncaster, J. L. Snaddon, A. Rogers. `[ma-047]` · `related-bioacoustics`
- **2017** · [Using mobile phones as acoustic sensors for high-throughput mosquito surveillance](https://doi.org/10.7554/eLife.27854
        
        
        
        ) — H. Mukundarajan, F. J. H. Hol, E. A. Castillo, C. Newby, M. Prakash. `[ma-027]` · `direct-mosquito`

### Datasets & Benchmarks

- **2026** · [Biodcase 2026 challenge baseline for cross-domain mosquito species classification](https://biodcase.github.io/challenge2026/task5) — Y. Hou, V. Zdravkovic, M. Sinka, Y. Li, W. Wang, M. D. Plumbley, K. Willis, S. Roberts. `[ma-031]` · `direct-mosquito`
- **2024** · Mosquitosong+: A noise-robust deep learning model for mosquito classification from wingbeat sounds — A. Supratak, P. Haddawy, M. S. Yin, T. Ziemer, W. Siritanakorn, K. Assawavinijkulchai, K. Chiamsakul, T. Chantanalertvilai, W. Suchalermkul, C. Sa-Ngamuang, et al.. `[ma-035]` · `direct-mosquito`
- **2021** · Humbugdb: A large-scale acoustic mosquito dataset — I. Kiskin, M. Sinka, A. D. Cobb, W. Rafique, L. Wang, D. Zilli, B. Gutteridge, R. Dam, T. Marinos, Y. Li, D. Msaky, E. Kaindoa, G. Killeen, E. Herreros-Moya, K. Willis, S. J. Roberts. `[ma-010]` · `direct-mosquito`
- **2020** · An annotated dataset of bioacoustic sensing and features of mosquitoes — D. Vasconcelos, N. J. Nunes, J. Gomes. `[ma-009]` · `direct-mosquito`
- **2020** · Humbug zooniverse: A crowd-sourced acoustic mosquito dataset — I. Kiskin, A. D. Cobb, L. Wang, S. Roberts. `[ma-030]` · `direct-mosquito`
- **2018** · Mosquito wingbeat analysis and classification using deep learning — E. Fanioudakis, M. Geismar, I. Potamitis. `[ma-028]` · `direct-mosquito`
- **2016** · Measuring the fundamental frequency and the harmonic properties of the wingbeat of a large number of mosquitoes in flight using 2d optoacoustic sensors — I. Potamitis, I. Rigakis. `[ma-022]` · `direct-mosquito`

### Uncertainty & Model Reliability

- **2025** · A classification-occupancy model based on automatically identified species data — R. Ogawa, F. Gosselin, K. F. Darras, S. Roilo, A. F. Cord. `[ma-049]` · `general-methods`
- **2021** · Automatic acoustic mosquito tagging with bayesian neural networks — I. Kiskin, A. D. Cobb, M. Sinka, K. Willis, S. J. Roberts. `[ma-012]` · `direct-mosquito`
- **2019** · Can you trust your model’s uncertainty? evaluating predictive uncertainty under dataset shift — Y. Ovadia, et al.. `[ma-045]` · `general-methods`
- **2017** · On calibration of modern neural networks — C. Guo, G. Pleiss, Y. Sun, K. Q. Weinberger. `[ma-044]` · `general-methods`
- **2016** · A baseline for detecting misclassified and out-of-distribution examples in neural networks — D. Hendrycks, K. Gimpel. `[ma-046]` · `general-methods`
- **2015** · Modeling false positive detections in species occurrence data under different study designs — T. Chambert, D. A. Miller, J. D. Nichols. `[ma-057]` · `general-methods`
- **2011** · Improving occupancy estimation when two types of observational error occur: Non-detection and species misidentification — D. A. Miller, J. D. Nichols, B. T. McClintock, E. H. C. Grant, L. L. Bailey, L. A. Weir. `[ma-052]` · `general-methods`

### Reviews & Perspectives

- **2026** · A review of acoustic systems for insect monitoring: From recording technologies to species recognition performance — B. Fengler, C. Seyidbayli, A. Reinhardt, M. Anders, C. Westphal. `[ma-015]` · `related-bioacoustics`
- **2026** · Foundation models for bioacoustics–a comparative review — R. Schwinger, P. V. Zadeh, L. Rauch, M. Kurz, T. Hauschild, S. Lapp, S. Tomforde. `[ma-040]` · `related-bioacoustics`
- **2024** · From buzzes to bytes: a systematic review of automated bioacoustics models used to detect, classify and monitor insects — A. B. Kohlberg, C. R. Myers, L. L. Figueroa. `[ma-014]` · `related-bioacoustics`
- **2023** · Using acoustic indices in ecology: Guidance on study design, analyses and interpretation — T. Bradfer-Lawrence, C. Desjonqueres, A. Eldridge, A. Johnston, O. Metcalf. `[ma-051]` · `related-bioacoustics`
- **2022** · A review of the surveillance techniques for aedes albopictus — Q.-M. Liu, Z.-Y. Gong, Z. Wang. `[ma-003]` · `direct-mosquito`
- **2022** · Computational bioacoustics with deep learning: a review and roadmap — D. Stowell. `[ma-013]` · `related-bioacoustics`
- **2020** · Buzzkill: targeting the mosquito auditory system — M. Andrés, M. P. Su, J. Albert, L. J. Cator. `[ma-017]` · `direct-mosquito`
- **2019** · Automated electronic approaches for detecting disease vectors mosquitoes through the wing-beat frequency — D. A. Santos, J. J. Rodrigues, V. Furtado, K. Saleem, V. Korotaev. `[ma-016]` · `direct-mosquito`
- **2019** · Emerging opportunities and challenges for passive acoustics in ecological assessment and monitoring — R. Gibb, E. Browning, P. Glover-Kapfer, K. E. Jones. `[ma-050]` · `related-bioacoustics`
- **2018** · Keeping track of mosquitoes: a review of tools to track, record and analyse mosquito flight — J. Spitzen, W. Takken. `[ma-002]` · `direct-mosquito`
- **2013** · Estimating animal population density using passive acoustics — T. A. Marques, L. Thomas, S. W. Martin, D. K. Mellinger, J. A. Ward, D. J. Moretti, D. Harris, P. L. Tyack. `[ma-053]` · `general-methods`

### Ecological Methods (Background)

- **2025** · A classification-occupancy model based on automatically identified species data — R. Ogawa, F. Gosselin, K. F. Darras, S. Roilo, A. F. Cord. `[ma-049]` · `general-methods`
- **2024** · Towards automated animal density estimation with acoustic spatial capture-recapture — Y. Wang, J. Ye, X. Li, D. L. Borchers. `[ma-063]` · `related-bioacoustics`
- **2024** · All thresholds barred: direct estimation of call density in bioacoustic data — A. K. Navine, T. Denton, M. J. Weldy, P. J. Hart. `[ma-064]` · `related-bioacoustics`
- **2024** · Counting the chorus: A bioacoustic indicator of population density — A. K. Navine, R. J. Camp, M. J. Weldy, T. Denton, P. J. Hart. `[ma-065]` · `related-bioacoustics`
- **2023** · Using acoustic indices in ecology: Guidance on study design, analyses and interpretation — T. Bradfer-Lawrence, C. Desjonqueres, A. Eldridge, A. Johnston, O. Metcalf. `[ma-051]` · `related-bioacoustics`
- **2021** · A spatial capture–recapture model to estimate call rate and population density from passive acoustic surveys — B. C. Stevenson, P. van Dam-Bates, C. K. Young, J. Measey. `[ma-062]` · `related-bioacoustics`
- **2019** · Dynamic wildlife occupancy models using automated acoustic monitoring data — C. Balantic, T. Donovan. `[ma-048]` · `general-methods`
- **2019** · Emerging opportunities and challenges for passive acoustics in ecological assessment and monitoring — R. Gibb, E. Browning, P. Glover-Kapfer, K. E. Jones. `[ma-050]` · `related-bioacoustics`
- **2018** · A new framework for analysing automated acoustic species detection data: Occupancy estimation and optimization of recordings post-processing — T. Chambert, J. H. Waddle, D. A. Miller, S. C. Walls, J. D. Nichols. `[ma-020]` · `general-methods`
- **2018** · On the reliability of N-mixture models for count data — R. J. Barker, M. R. Schofield, W. A. Link, J. R. Sauer. `[ma-055]` · `general-methods`
- **2018** · On the robustness of n-mixture models — W. A. Link, M. R. Schofield, R. J. Barker, J. R. Sauer. `[ma-056]` · `general-methods`
- **2015** · Modeling false positive detections in species occurrence data under different study designs — T. Chambert, D. A. Miller, J. D. Nichols. `[ma-057]` · `general-methods`
- **2013** · Estimating animal population density using passive acoustics — T. A. Marques, L. Thomas, S. W. Martin, D. K. Mellinger, J. A. Ward, D. J. Moretti, D. Harris, P. L. Tyack. `[ma-053]` · `general-methods`
- **2011** · Improving occupancy estimation when two types of observational error occur: Non-detection and species misidentification — D. A. Miller, J. D. Nichols, B. T. McClintock, E. H. C. Grant, L. L. Bailey, L. A. Weir. `[ma-052]` · `general-methods`
- **2011** · Integrated population models: a novel analysis framework for deeper insights into population dynamics — M. Schaub, F. Abadi. `[ma-058]` · `general-methods`
- **2004** · N-mixture models for estimating population size from spatially replicated counts — J. A. Royle. `[ma-019]` · `general-methods`
- **2002** · Estimating site occupancy rates when detection probabilities are less than one — D. I. MacKenzie, J. D. Nichols, G. B. Lachman, S. Droege, J. Andrew Royle, C. A. Langtimm. `[ma-018]` · `general-methods`
- **2002** · Fitting population models incorporating process noise and observation error — P. De Valpine, A. Hastings. `[ma-054]` · `general-methods`

## Registry fields

The machine-readable [`papers.csv`](papers.csv) includes `paper_id`, `source_ref_number`, `title`, `authors`, `year`, `publication_type`, `topic_tags`, `evidence_scope`, `doi`, `primary_url`, `code_url`, `dataset_url`, `metadata_status`, `notes`, and `raw_reference`.

## Contributing and maintenance

1. Check the original publication (publisher, DOI, arXiv or conference proceedings) before adding or editing metadata.
2. Add a stable `paper_id` and one or more `topic_tags`; do not reuse existing IDs.
3. Link to official code and dataset releases rather than uploading copyrighted papers.
4. Distinguish real mosquito evaluations from methods only demonstrated on other taxa.
5. Use a pull request to propose corrections and attach a source link.

## Related research

Statistical models of acoustic-to-ecological inference belong in the separate `acoustic-ecological-inference` project; this catalog retains a clearly labelled background methods section for discoverability.

