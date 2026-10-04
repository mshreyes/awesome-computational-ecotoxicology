# Awesome Computational Ecotoxicology Resources [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

Databases, datasets, software, models, APIs, knowledgebases, and other computational resources for ecotoxicology.

Each resource is listed once, in its most specific category. Cross-references are given where a resource is relevant to several sections.

## Contents

- [Ecotoxicology Databases](#ecotoxicology-databases)
- [Ecotoxicity Datasets](#ecotoxicity-datasets)
- [Chemical and Contaminant Resources](#chemical-and-contaminant-resources)
- [Environmental Fate and Exposure](#environmental-fate-and-exposure)
- [Species and Biodiversity Data](#species-and-biodiversity-data)
- [Ecological Interactions and Networks](#ecological-interactions-and-networks)
- [QSAR and Toxicity Prediction](#qsar-and-toxicity-prediction)
- [Species Sensitivity, Cross-Species Extrapolation and Risk Assessment](#species-sensitivity-cross-species-extrapolation-and-risk-assessment)
- [Adverse Outcome Pathways](#adverse-outcome-pathways)
- [Ecological and Ecosystem Modelling](#ecological-and-ecosystem-modelling)
- [Machine Learning and AI](#machine-learning-and-ai)
- [Cheminformatics](#cheminformatics)
- [R and Python Packages](#r-and-python-packages)
- [APIs and Programmatic Access](#apis-and-programmatic-access)
- [Omics and Mechanistic Resources](#omics-and-mechanistic-resources)
- [Regulatory and Assessment Resources](#regulatory-and-assessment-resources)
- [Learning and Reference Resources](#learning-and-reference-resources)
- [Inclusion Criteria](#inclusion-criteria)
- [Related Projects](#related-projects)
- [Curation Notes](#curation-notes)

---

## Ecotoxicology Databases

Curated sources of experimental ecotoxicity data and regulatory study information.

- [ECOTOX Knowledgebase](https://cfpub.epa.gov/ecotox/) - US EPA database of experimentally observed adverse effects of single chemical stressors on aquatic and terrestrial organisms. A core source for ecotoxicological data and modelling. Bulk ASCII exports are available for local use.
- [EnviroTox](https://envirotoxdatabase.org/) - Curated aquatic toxicity database for ecological threshold-of-concern and risk assessment applications, with PNEC and toxicity-distribution calculation tools.
- [Standartox](https://doi.org/10.5281/zenodo.3785030) - Cleaned, harmonised, and aggregated ecotoxicity test data, accessible through the `standartox` R package.
- [RIVM e-toxBase](https://doi.org/10.5281/zenodo.22660359) - Curated ecotoxicity database supporting species sensitivity distributions and related assessment methods. Version 1.1 (September 2026) contains 255,109 records covering 10,988 chemicals and 2,026 species; restrictions and missing values are documented in the release.
- [NORMAN Ecotoxicology Database](https://www.norman-network.net/nds/ecotox/) - Experimental ecotoxicity endpoints and quality targets used for prioritisation and derivation of environmental quality targets.
- [UBA ETOX](https://webetox.uba.de/webETOX/) - German Environment Agency information system on aquatic and terrestrial ecotoxicity and environmental quality targets.
- [FishBase Ecotoxicology](https://www.fishbase.se/manual/English/fishbasethe_ecotoxicology_table.htm) - Fish-specific ecotoxicological records, including LC50 values and experimental metadata.
- [ECHA CHEM](https://chem.echa.europa.eu/) - European Chemicals Agency database of chemical, regulatory, and study information, including ecotoxicological data from REACH dossiers.
- [eChemPortal](https://www.echemportal.org/) - Global portal to chemical property, hazard, and risk information from participating databases and programmes.

---

## Ecotoxicity Datasets

Benchmark and reusable datasets distributed as files. Large curated databases are listed under Ecotoxicology Databases.

- [ADORE](https://github.com/LiliGasser/ADORE) - Benchmark dataset for machine learning in ecotoxicology, focused on acute mortality in fish, crustaceans, and algae, with chemical, taxonomic, and phylogenetic information and predefined splits. Described in the [Scientific Data descriptor](https://doi.org/10.1038/s41597-023-02612-2).
- [ApisTox](https://github.com/j-adamczyk/ApisTox_dataset) - Benchmark dataset for small-molecule toxicity classification in honey bees, with code for dataset reconstruction and splitting.

### General toxicology benchmarks

These are not ecotoxicity-specific. Include them only when used for environmental chemical or mechanism-focused modelling rather than drug discovery.

- [Tox21](https://tripod.nih.gov/tox21/challenge/) - High-throughput toxicity screening data and challenge benchmark.
- [MoleculeNet](https://moleculenet.org/) - Molecular machine-learning benchmark suite, including toxicity tasks such as Tox21.
- [PyTDC](https://tdcommons.ai/) - Therapeutics Data Commons, with datasets and benchmarks for chemical property prediction. Use only datasets with direct environmental or toxicological relevance.

---

## Chemical and Contaminant Resources

- [CompTox Chemicals Dashboard](https://comptox.epa.gov/dashboard/) - EPA platform integrating chemical identity, physicochemical properties, toxicity, bioactivity (including ToxCast high-throughput data), exposure, and fate information.
- [DSSTox](https://www.epa.gov/comptox-tools/distributed-structure-searchable-toxicity-dsstox-database) - EPA chemical database linking structures with identifiers and toxicological, bioactivity, and physicochemical information.
- [PubChem](https://pubchem.ncbi.nlm.nih.gov/) - Large public resource of chemical structures, identifiers, properties, biological activity, safety, and toxicity information.
- [ChEBI](https://www.ebi.ac.uk/chebi/) - Ontology and database of molecular entities of biological interest.
- [ChemSpider](https://www.chemspider.com/) - Chemical structure and identifier aggregation service.
- [UniChem](https://www.ebi.ac.uk/unichem/) - Cross-reference service connecting chemical identifiers across databases, with an API for programmatic mapping.
- [NORMAN Substance Database](https://www.norman-network.net/nds/susdat/) - Standardised substance inventory supporting emerging contaminant screening and prioritisation.
- [NORMAN Suspect List Exchange](https://www.norman-network.net/nds/SLE/) - Community resource for suspect lists used in non-target and suspect screening.
- [NORMAN MassBank](https://www.norman-network.net/nds/) - Mass spectral information supporting identification of environmental contaminants.

---

## Environmental Fate and Exposure

- [EPI Suite](https://www.epa.gov/tsca-screening-tools/epi-suitetm-estimation-program-interface) - EPA screening-level suite for estimating physicochemical and environmental fate properties. Includes ECOSAR (see QSAR and Toxicity Prediction).
- [BioTransformer](https://biotransformer.ca/) - Predicts xenobiotic metabolism and biotransformation products, useful for transformation and metabolite assessment.
- [USEtox](https://usetox.org/) - Model for characterising human toxicity and freshwater ecotoxicity impacts of chemicals in life cycle assessment.
- [Pesticide Properties DataBase (PPDB)](https://sitem.herts.ac.uk/aeru/ppdb/en/) - University of Hertfordshire resource on pesticide identity, physicochemical properties, environmental fate, and ecotoxicity, developed under the FOOTPRINT project.
- [EPA Models for Pesticide Risk Assessment](https://www.epa.gov/pesticide-science-and-assessing-pesticide-risks/models-pesticide-risk-assessment) - EPA Office of Pesticide Programs screening-level exposure models, including PWC (water concentrations), KABAM (aquatic bioaccumulation), T-REX and T-HERPS (terrestrial residues), TerrPlant, and Bee-REX.
- [NORMAN Chemical Occurrence Database](https://www.norman-network.net/nds/occurrence/) - Geo-referenced environmental monitoring data for emerging substances.
- [EPA ChemExpo](https://chemexpo.epa.gov/) - Chemical use and product information supporting exposure assessment.

---

## Species and Biodiversity Data

Included where species identity, distribution, taxonomy, or biodiversity information is directly useful for ecotoxicological modelling. Programmatic access is listed under APIs and Programmatic Access.

- [GBIF](https://www.gbif.org/) - Global biodiversity data infrastructure providing species occurrence records.
- [OBIS](https://obis.org/) - Ocean Biodiversity Information System, with integrated marine species occurrence data.
- [Catalogue of Life](https://www.catalogueoflife.org/) - Global checklist of species and taxonomic information.
- [ITIS](https://www.itis.gov/) - Taxonomic information system with names, identifiers, and hierarchies.
- [WoRMS](https://www.marinespecies.org/) - World Register of Marine Species, providing authoritative marine taxonomy.
- [FishBase](https://www.fishbase.se/) - Fish species database covering taxonomy, ecology, life history, and distribution.
- [AmphibiaWeb](https://amphibiaweb.org/) - Amphibian species information and conservation-related data.
- [iNaturalist](https://www.inaturalist.org/) - Community biodiversity observations with machine-assisted species identification and API access.

---

## Ecological Interactions and Networks

- [GloBI](https://www.globalbioticinteractions.org/) - Global Biotic Interactions integrates species interaction data into searchable, downloadable ([datasets](https://www.globalbioticinteractions.org/data)), and API-accessible interaction networks. Can be used to assemble trophic networks for exposure and effect analyses.
- [rglobi](https://github.com/ropensci/rglobi) - R interface for querying GloBI.
- [Mangal](https://mangal.io/) - Database and API for ecological networks, including trophic, host-parasite, and pollination networks.

---

## QSAR and Toxicity Prediction

- [OECD QSAR Toolbox](https://qsartoolbox.org/) - Free software for chemical profiling, analogue and category identification, read-across, and (Q)SAR workflows, with extensive ecotoxicological models and data.
- [ECOSAR](https://www.epa.gov/tsca-screening-tools/ecological-structure-activity-relationships-ecosar) - EPA structure-activity models for predicting aquatic toxicity.
- [OPERA](https://github.com/kmansouri/OPERA) - Open-source QSAR models for physicochemical properties, environmental fate, and selected toxicity endpoints, with applicability-domain and accuracy information.
- [VEGA](https://www.vegahub.eu/) - Free platform (VEGA HUB) providing QSAR models and workflows for chemical hazard prediction.
- [TEST](https://www.epa.gov/tsca-screening-tools/toxicity-estimation-software-tool-test) - EPA Toxicity Estimation Software Tool for predicting selected toxicity endpoints from chemical structure.
- [EPA GenRA](https://www.epa.gov/comptox-tools/genra) - Algorithmic read-across approach for reproducible toxicity and bioactivity prediction.
- [QSARDB](https://qsardb.org/) - Repository of QSAR models and datasets with metadata and documentation.
- [JRC QSAR Model Database](https://qsardb.jrc.ec.europa.eu/qmrf/) - Collection of documented QSAR models and QMRF reports.

---

## Species Sensitivity, Cross-Species Extrapolation and Risk Assessment

- [ssdtools](https://github.com/bcgov/ssdtools) - R package for fitting, comparing, averaging, and plotting Species Sensitivity Distributions.
- [ssddata](https://github.com/bcgov/ssddata) - Example ecotoxicity datasets for use with `ssdtools`.
- [SSD Toolbox](https://www.epa.gov/comptox-tools/species-sensitivity-distribution-ssd-toolbox) - EPA tools for analysing species sensitivity distributions and ecological risk.
- [Web-ICE](https://www.epa.gov/comptox-tools/web-ice) - EPA tool for estimating acute toxicity to untested aquatic and terrestrial species by interspecies extrapolation.
- [SeqAPASS](https://seqapass.epa.gov/) - Predicts relative intrinsic susceptibility across species using molecular target conservation and sequence information.

---

## Adverse Outcome Pathways

- [AOP-Wiki](https://aopwiki.org/) - Primary knowledgebase and authoring environment for AOPs, including stressors, molecular initiating events, key events, key event relationships, and adverse outcomes. Structured content is available for download.
- [AOP Knowledge Base (AOP-KB)](https://aopkb.oecd.org/) - OECD-supported platform hosting AOP-Wiki and the eAOP Portal for searching and discovering AOP knowledge.
- [EPA AOP-DB](https://aopdb.epa.gov/) - EPA database integrating AOP data with gene, chemical, pathway, disease, and orthology information.
- [AOP-Wiki RDF](https://github.com/marvinm2/AOPWikiRDF) - Conversion of AOP-Wiki content to RDF with automated updates and semantic-web access.
- [AOP-Wiki RDF Dashboard](https://github.com/marvinm2/AOP-Wiki-RDF-dashboard) - Dashboard for exploring the RDF representation of AOP-Wiki.
- [AOPWiki Explorer](https://github.com/InSilicoVida-Research-Lab/AOPWiki_Explorer) - Graph-based query and exploration interface for AOP-Wiki.
- [AOP HelpFinder](https://aophelpfinder.ineris.fr/) - Text-mining tool linking chemicals, biological events, and AOP information in the literature.
- [OECD Series on Adverse Outcome Pathways](https://www.oecd.org/en/publications/serials/oecd-series-on-adverse-outcome-pathways_g1727132.html) - Published collection of reviewed and endorsed AOP descriptions.

---

## Ecological and Ecosystem Modelling

- [AQUATOX](https://www.epa.gov/hydrowq/aquatox) - EPA process-based model of aquatic ecosystem dynamics, chemical fate, bioaccumulation, toxicity, and ecological responses. Source code and releases are available from the [download page](https://www.epa.gov/hydrowq/aquatox-32-download-page).
- [MCnest](https://www.epa.gov/comptox-tools/ecological-risk-assessment-tools) - Markov-chain model for estimating pesticide effects on avian reproduction.

For toxicokinetic-toxicodynamic (GUTS) modelling see `morse` under R and Python Packages.

---

## Machine Learning and AI

Restricted to ML/AI resources with a meaningful chemical, toxicity, species, or ecotoxicological application. Benchmark datasets are listed under Ecotoxicity Datasets.

- [DeepChem](https://deepchem.io/) - Open-source framework for machine learning on molecules and materials, including toxicity and environmental chemistry applications.
- [Chemprop](https://github.com/chemprop/chemprop) - Message-passing neural network framework for molecular property prediction.
- [DGL-LifeSci](https://github.com/awslabs/dgl-lifesci) - Graph neural network toolkit for molecular and life-science prediction tasks.

---

## Cheminformatics

- [RDKit](https://www.rdkit.org/) - Open-source toolkit for molecular structures, descriptors, fingerprints, similarity, and modelling (Python, C++).
- [CDK](https://cdk.github.io/) - Java-based Chemistry Development Kit for cheminformatics and molecular descriptors. Accessible from R through [`rcdk`](https://cran.r-project.org/package=rcdk).
- [PaDEL-Descriptor](http://www.yapcwsoft.com/dd/padeldescriptor/) - Large collection of molecular descriptors and fingerprints used in QSAR.
- [Mordred](https://github.com/mordred-descriptor/mordred) - Python molecular descriptor calculator for QSAR and machine learning.
- [Open Babel](https://openbabel.org/) - Chemical toolbox for file format conversion and cheminformatics.
- [ToxPrint](https://toxprint.org/) - Chemotypes representing structural features in computational toxicology workflows.

---

## R and Python Packages

Domain-specific packages are listed here by function. SSD packages are under Species Sensitivity, Cross-Species Extrapolation and Risk Assessment; client libraries for biodiversity and chemical APIs are under APIs and Programmatic Access.

### Ecotoxicity data access and processing (R)

- [ECOTOXr](https://cran.r-project.org/package=ECOTOXr) - Builds a local SQLite copy of the US EPA ECOTOX database and supports reproducible querying and sanitising of the data.
- [standartox](https://github.com/andschar/standartox) - Access to harmonised and aggregated test data from the Standartox database.
- [wqbench](https://github.com/bcgov/wqbench) - Downloads, processes, and compiles EPA ECOTOX data for aquatic-life water quality benchmarks.
- [REcoTox](https://github.com/tsufz/REcoTox) - Semi-automated workflow for processing EPA ECOTOX ASCII data.
- [envirotox](https://github.com/poissonconsulting/envirotox) - Species Sensitivity Distribution datasets derived from EnviroTox.

### Dose-response and effect modelling (R)

- [drc](https://cran.r-project.org/package=drc) - Dose-response curve fitting and analysis.
- [bayesnec](https://cran.r-project.org/package=bayesnec) - Bayesian no-effect-concentration and ECx estimation from concentration-response data.
- [morse](https://cran.r-project.org/package=morse) - Survival and reproduction analysis in ecotoxicology, including Bayesian inference of the GUTS toxicokinetic-toxicodynamic model.

### Community ecology (R)

- [vegan](https://cran.r-project.org/package=vegan) - Community ecology and multivariate analysis, including principal response curves (`prc`) for mesocosm and community-level toxicity studies.

---

## APIs and Programmatic Access

- [EPA CTX APIs](https://comptox.epa.gov/ctx-api/docs/) - APIs covering chemical, hazard, bioactivity, and exposure data.
- [EPA Hazard API](https://github.com/USEPA/ccte-api-hazard) - Open-source implementation of the CTX Hazard API.
- [PubChem PUG REST](https://pubchem.ncbi.nlm.nih.gov/docs/pug-rest-tutorial) - Chemical identifiers, structures, properties, and related data.
- [GBIF API](https://techdocs.gbif.org/en/openapi/) - Species occurrence, taxonomy, and bulk download services, including the [Occurrence API](https://techdocs.gbif.org/en/openapi/v1/occurrence).
- [OBIS API](https://api.obis.org/) - Marine biodiversity data. See also [OBIS Data Access](https://portal.obis.org/data/access/) for R tools and GeoParquet bulk access.
- [Catalogue of Life API](https://www.catalogueoflife.org/tools/api) - Taxonomic and checklist data through ChecklistBank.
- [ITIS Web Services](https://www.itis.gov/web_service.html) - Taxonomic name search and hierarchy APIs.
- [GloBI API](https://api.globalbioticinteractions.org/) - Species interaction records.

### Client libraries

- [PubChemPy](https://pubchempy.readthedocs.io/) - Python wrapper for PubChem's PUG REST services.
- [webchem](https://cran.r-project.org/package=webchem) - R package for chemical information retrieval from web sources, including PubChem and the CompTox Dashboard.
- [pygbif](https://github.com/gbif/pygbif) - Python client for GBIF.
- [rgbif](https://cran.r-project.org/package=rgbif) - R client for GBIF.
- [pyobis](https://github.com/iobis/pyobis) - Python client for OBIS.
- [robis](https://cran.r-project.org/package=robis) - R client for OBIS.
- [taxize](https://cran.r-project.org/package=taxize) - R package for taxonomic name resolution across multiple sources.

---

## Omics and Mechanistic Resources

Included where they support mechanistic ecotoxicology, environmental exposure studies, species responses, or toxicogenomics. AOP resources are listed under Adverse Outcome Pathways.

- [GEO](https://www.ncbi.nlm.nih.gov/geo/) - Gene Expression Omnibus, public functional genomics datasets.
- [ArrayExpress / BioStudies](https://www.ebi.ac.uk/biostudies/) - Public repository for functional genomics experiments.
- [PRIDE](https://www.ebi.ac.uk/pride/) - Public proteomics data repository.
- [UniProt](https://www.uniprot.org/) - Protein sequence and functional annotation.
- [Ensembl](https://www.ensembl.org/) - Genomic annotation and comparative genomics.
- [NCBI Gene](https://www.ncbi.nlm.nih.gov/gene/) - Gene information and identifiers.
- [KEGG](https://www.kegg.jp/) - Pathways, molecular functions, and biological systems.
- [Reactome](https://reactome.org/) - Curated biological pathway knowledgebase.
- [STRING](https://string-db.org/) - Protein-protein association networks.
- [CTD](https://ctdbase.org/) - Chemical-gene-phenotype-disease relationships. Use selectively for environmental and ecotoxicological applications.

---

## Regulatory and Assessment Resources

Regulatory data portals (ECHA CHEM, eChemPortal) are listed under Ecotoxicology Databases.

- [OECD Test Guidelines](https://www.oecd.org/en/topics/sub-issues/testing-of-chemicals.html) - Internationally harmonised methods for chemical testing, including environmental endpoints.
- [OECD Adverse Outcome Pathways programme](https://www.oecd.org/en/topics/sub-issues/testing-of-chemicals/adverse-outcome-pathways.html) - OECD framework and guidance for developing, reviewing, and using AOPs in chemical assessment.
- [NORMAN Network](https://www.norman-network.net/) - European network and database infrastructure for emerging contaminants, monitoring, prioritisation, and ecotoxicological assessment.

---

## Learning and Reference Resources

- [EPA CompTox Tools](https://www.epa.gov/comptox-tools) - Documentation and training material for computational toxicology and exposure tools.
- [ECOTOX documentation](https://www.epa.gov/comptox-tools/ecotox-knowledgebase) - ECOTOX user guidance and data access information.
- [OECD QSAR Toolbox support](https://qsartoolbox.org/support/) - Manuals, tutorials, and ecotoxicity-specific workflows.
- [AQUATOX documentation](https://www.epa.gov/hydrowq/aquatox-supporting-documentation) - User manuals, technical documentation, sensitivity analyses, and examples.
- [GBIF documentation](https://docs.gbif.org/) - Documentation and training for biodiversity data discovery and analysis.
- [OBIS manual](https://manual.obis.org/) - Guidance on marine biodiversity data and analysis.
- [SETAC](https://www.setac.org/) - Professional society for environmental toxicology and chemistry, with guidance, publications, and educational material.

---

## Contributing

Contributions are welcome. Please read the [contribution guidelines](contributing.md) first.

---

## Related Projects

- [GitHub topic: toxicology](https://github.com/topics/toxicology) - Repositories tagged with toxicology, useful for discovering adjacent projects.
- [GitHub topic: computational-toxicology](https://github.com/topics/computational-toxicology) - Repositories tagged with computational toxicology.

---

## Curation Notes

This list is intentionally narrower than a general computational toxicology resource list. A resource is included when it can directly support the computational study, prediction, modelling, or assessment of ecological effects.

Resources should be periodically rechecked for availability, maintenance status, licensing, and current URLs.

**Last reviewed:** 4 October 2026

---

[![CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/88x31.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
