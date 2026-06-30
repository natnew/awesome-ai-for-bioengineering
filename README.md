# Awesome AI for Bioengineering [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of high-quality resources on AI for bioengineering, including biological foundation models, protein design, molecular generation, self-driving laboratories, datasets, benchmarks, tooling, and responsible release practices.

This list tracks AI engineering resources relevant to bioengineering: the models, tools, datasets, benchmarks, and practices used to build and evaluate AI systems for biology. It is curated from an AI engineering perspective, with an emphasis on canonical sources, technical substance, and durable value.

> **Scope and safety.** This list is for technical research mapping and AI engineering awareness. It does not provide medical, clinical, biological laboratory, or experimental instructions. Entries stay at the level of what AI systems model, predict, or generate. See [SECURITY.md](SECURITY.md).

## Contents

- [Foundations and Surveys](#foundations-and-surveys)
- [Biological Foundation Models](#biological-foundation-models)
- [Protein Language Models](#protein-language-models)
- [Protein Structure and Function Prediction](#protein-structure-and-function-prediction)
- [Generative Protein Design](#generative-protein-design)
- [Molecular Generation and Drug Discovery](#molecular-generation-and-drug-discovery)
- [DNA and RNA Modelling](#dna-and-rna-modelling)
- [Biomolecular Simulation](#biomolecular-simulation)
- [AI Agents for Science](#ai-agents-for-science)
- [Self-Driving Laboratories](#self-driving-laboratories)
- [Lab Automation and Closed-Loop Systems](#lab-automation-and-closed-loop-systems)
- [Synthetic Biology Tooling](#synthetic-biology-tooling)
- [Datasets](#datasets)
- [Benchmarks and Evaluation](#benchmarks-and-evaluation)
- [Reproducibility and Validation](#reproducibility-and-validation)
- [Safety, Security, and Responsible Release](#safety-security-and-responsible-release)
- [Academic Labs and Research Groups](#academic-labs-and-research-groups)
- [Companies and Platforms](#companies-and-platforms)
- [Open-Source Tools](#open-source-tools)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)
- [Contributors](#contributors)

## Foundations and Surveys

- [A guide to machine learning for biologists](https://doi.org/10.1038/s41580-021-00407-0) - Review introducing core machine-learning concepts for biological research.
- [Opportunities and obstacles for deep learning in biology and medicine](https://doi.org/10.1098/rsif.2017.0387) - Survey of deep-learning applications and limitations across biology and medicine.
- [Scientific discovery in the age of artificial intelligence](https://doi.org/10.1038/s41586-023-06221-2) - Perspective on how AI is reshaping the scientific discovery process.

## Biological Foundation Models

- [Evo](https://github.com/evo-design/evo) - DNA foundation model for sequence modelling and design at genome scale.
- [Evo 2](https://github.com/ArcInstitute/evo2) - Genome foundation model spanning domains of life, built on the StripedHyena 2 architecture.
- [Geneformer](https://huggingface.co/ctheodoris/Geneformer) - Transformer foundation model pretrained on single-cell transcriptomes for gene-network tasks.
- [Nucleotide Transformer](https://github.com/instadeepai/nucleotide-transformer) - Family of genomic language models for DNA sequence understanding and prediction.
- [scGPT](https://github.com/bowang-lab/scGPT) - Generative foundation model for single-cell multi-omics analysis.

## Protein Language Models

- [Ankh](https://github.com/agemagician/Ankh) - General-purpose protein language model focused on parameter and compute efficiency.
- [ESM](https://github.com/facebookresearch/esm) - Evolutionary Scale Modeling: transformer protein language models for sequence representation and structure.
- [ESM (EvolutionaryScale)](https://github.com/evolutionaryscale/esm) - Successor protein models including ESM C and ESMFold-based structure prediction.
- [ProGen2](https://github.com/salesforce/progen) - Autoregressive protein language models for sequence generation and fitness prediction.
- [ProtTrans](https://github.com/agemagician/ProtTrans) - Collection of transformer protein language models and embeddings for downstream tasks.

## Protein Structure and Function Prediction

- [AlphaFold](https://github.com/google-deepmind/alphafold) - Deep-learning system for predicting protein three-dimensional structure from sequence.
- [AlphaFold 3](https://github.com/google-deepmind/alphafold3) - Model for predicting the structure of proteins, nucleic acids, and their complexes.
- [Boltz](https://github.com/jwohlwend/boltz) - Open biomolecular model for joint structure and protein-ligand binding-affinity prediction.
- [ColabFold](https://github.com/sokrypton/ColabFold) - Accessible structure prediction combining fast sequence search with AlphaFold and related models.
- [OpenFold](https://github.com/aqlaboratory/openfold) - Trainable open-source reimplementation of AlphaFold for structure prediction research.
- [RoseTTAFold All-Atom](https://github.com/baker-laboratory/RoseTTAFold-All-Atom) - Model predicting assemblies of proteins, nucleic acids, small molecules, and modifications.

## Generative Protein Design

- [Chroma](https://github.com/generatebio/chroma) - Generative diffusion model for programmable protein design.
- [LigandMPNN](https://github.com/dauparas/LigandMPNN) - Sequence-design model conditioned on structural and ligand context, extending ProteinMPNN.
- [ProteinMPNN](https://github.com/dauparas/ProteinMPNN) - Message-passing model for protein sequence design given a target backbone.
- [RFdiffusion](https://github.com/RosettaCommons/RFdiffusion) - Diffusion model for generating protein backbones for design tasks.

## Molecular Generation and Drug Discovery

- [DiffDock](https://github.com/gcorso/DiffDock) - Diffusion generative model that predicts small-molecule binding poses (blind docking).
- [DiffSBDD](https://github.com/arneschneuing/DiffSBDD) - SE(3)-equivariant diffusion model generating ligands conditioned on a protein pocket.
- [E(3) Equivariant Diffusion Model](https://github.com/ehoogeboom/e3_diffusion_for_molecules) - Reference diffusion model jointly generating 3D atom coordinates and types.
- [REINVENT4](https://github.com/MolecularAI/REINVENT4) - Toolkit for de novo molecular generation and optimisation via reinforcement and transfer learning.

## DNA and RNA Modelling

- [Caduceus](https://github.com/kuleshov-group/caduceus) - Bi-directional equivariant architecture for long-range DNA sequence modelling.
- [DNABERT-2](https://github.com/MAGICS-LAB/DNABERT_2) - Foundation model and benchmark for multi-species genome understanding.
- [Enformer](https://github.com/google-deepmind/deepmind-research/tree/master/enformer) - Model predicting gene expression from DNA sequence using long-range attention.
- [RNA-FM](https://github.com/ml4bio/RNA-FM) - Pretrained language model for RNA sequences supporting structure and function tasks.

## Biomolecular Simulation

- [DeePMD-kit](https://github.com/deepmodeling/deepmd-kit) - Toolkit for machine-learning interatomic potentials and molecular dynamics.
- [MACE](https://github.com/ACEsuit/mace) - Higher-order equivariant message-passing machine-learning interatomic potentials.
- [OpenMM](https://github.com/openmm/openmm) - High-performance toolkit for molecular simulation with support for ML potentials.
- [SchNetPack](https://github.com/atomistic-machine-learning/schnetpack) - Toolbox for building and training neural networks for atomistic systems.
- [TorchMD-NET](https://github.com/torchmd/torchmd-net) - Neural-network potentials and training framework for molecular dynamics.

## AI Agents for Science

- [Biomni](https://github.com/snap-stanford/Biomni) - General-purpose biomedical AI agent for autonomous research tasks.
- [ChemCrow](https://github.com/ur-whitelab/chemcrow-public) - LLM agent that integrates chemistry tools for reasoning-intensive tasks.
- [Coscientist](https://doi.org/10.1038/s41586-023-06792-0) - Study on autonomous chemical research driven by large language models.
- [The AI Scientist](https://github.com/SakanaAI/AI-Scientist) - System for automated, open-ended scientific research and paper generation.

## Self-Driving Laboratories

- [A mobile robotic chemist](https://doi.org/10.1038/s41586-020-2442-2) - Study on an autonomous mobile robot conducting experimental optimisation.
- [Acceleration Consortium](https://acceleration.utoronto.ca) - Research initiative on self-driving laboratories for materials and molecular discovery.

## Lab Automation and Closed-Loop Systems

- [Atlas](https://github.com/aspuru-guzik-group/atlas) - Bayesian optimisation library for self-driving laboratories.
- [BayBE](https://github.com/emdgroup/baybe) - Bayesian optimisation and design-of-experiments back end for experimental campaigns.
- [Olympus](https://github.com/aspuru-guzik-group/olympus) - Benchmarking framework for optimisation algorithms in experimental science.
- [Opentrons](https://github.com/Opentrons/opentrons) - Software for programmable liquid-handling laboratory robots.
- [PyLabRobot](https://github.com/PyLabRobot/pylabrobot) - Hardware-agnostic SDK for laboratory automation.
- [Summit](https://github.com/sustainable-processes/summit) - Library for optimising reactions and processes with machine learning.

## Synthetic Biology Tooling

- [Cello](https://github.com/CIDARLAB/cello) - Design-automation software that compiles logic specifications into genetic circuit designs.
- [SBOL](https://sbolstandard.org) - Synthetic Biology Open Language, a standard for representing biological designs.
- [SynBioHub](https://github.com/SynBioHub/synbiohub) - Web application for browsing, uploading, and sharing synthetic biology designs.

## Datasets

- [AlphaFold Protein Structure Database](https://alphafold.ebi.ac.uk) - Predicted protein structures covering a large fraction of known sequences.
- [ChEMBL](https://www.ebi.ac.uk/chembl/) - Curated database of bioactive molecules with drug-like properties.
- [ENCODE](https://www.encodeproject.org) - Encyclopedia of functional DNA elements across the human and mouse genomes.
- [Protein Data Bank](https://www.rcsb.org) - Archive of experimentally determined three-dimensional structures of biomolecules.
- [UniProt](https://www.uniprot.org) - Comprehensive resource of protein sequence and functional annotation.
- [ZINC20](https://zinc20.docking.org) - Database of commercially available compounds for virtual screening.

## Benchmarks and Evaluation

- [CASP](https://predictioncenter.org) - Community assessment of protein structure prediction methods.
- [GuacaMol](https://github.com/BenevolentAI/guacamol) - Benchmark suite for de novo molecular design.
- [MoleculeNet](https://moleculenet.org) - Benchmark collection for molecular machine-learning tasks.
- [MOSES](https://github.com/molecularsets/moses) - Benchmarking platform for molecular generation models.
- [PoseBusters](https://github.com/maabuu/posebusters) - Test suite for checking the physical validity of predicted ligand poses.
- [ProteinGym](https://github.com/OATML-Markslab/ProteinGym) - Benchmarks for protein fitness prediction and variant effect models.
- [TAPE](https://github.com/songlab-cal/tape) - Tasks Assessing Protein Embeddings, a benchmark for learned protein representations.
- [Therapeutics Data Commons](https://github.com/mims-harvard/TDC) - Datasets, tasks, and leaderboards spanning therapeutic discovery and development.

## Reproducibility and Validation

- [DOME recommendations](https://doi.org/10.1038/s41592-021-01205-4) - Reporting recommendations for machine-learning studies in biology.
- [Reproducibility standards for machine learning in the life sciences](https://doi.org/10.1038/s41592-021-01256-7) - Proposed standards for reproducible ML research in biology.
- [Transparency and reproducibility in artificial intelligence](https://doi.org/10.1038/s41586-020-2766-y) - Analysis of transparency and reproducibility issues in applied AI.

## Safety, Security, and Responsible Release

- [IBBIS](https://ibbis.bio) - International Biosecurity and Biosafety Initiative for Science, including DNA-synthesis screening.
- [Johns Hopkins Center for Health Security](https://centerforhealthsecurity.org) - Research centre covering biosecurity and emerging-technology risk.
- [NTI | bio](https://www.nti.org/about/biosecurity/) - Programme on reducing biological risks, including AI and biosecurity.
- [Responsible AI x Biodesign](https://responsiblebiodesign.ai) - Community values and commitments for responsible AI protein design.

## Academic Labs and Research Groups

- [AlQuraishi Lab](https://www.aqlab.io) - Columbia University group working on machine learning for molecular and systems biology.
- [Debora Marks Lab](https://www.deboramarkslab.com) - Harvard Medical School group on evolutionary sequence modelling and variant effect prediction.
- [Institute for Protein Design](https://www.ipd.uw.edu) - University of Washington institute (Baker Lab) for computational protein design.
- [Matter Lab](https://www.matter.toronto.edu) - University of Toronto group (Aspuru-Guzik) on AI for discovery and self-driving labs.

## Companies and Platforms

- [Chai Discovery](https://www.chaidiscovery.com) - Company developing models for biomolecular structure and interaction prediction.
- [Cradle](https://www.cradle.bio) - Protein-engineering platform using machine learning for sequence optimisation.
- [EvolutionaryScale](https://www.evolutionaryscale.ai) - Company developing the ESM family of protein foundation models.
- [Generate Biomedicines](https://www.generatebiomedicines.com) - Company applying generative models to protein and therapeutic design.
- [Isomorphic Labs](https://www.isomorphiclabs.com) - Company applying AI to drug discovery, building on structure-prediction research.
- [Profluent](https://www.profluent.bio) - Company using protein language models to design functional proteins.
- [Recursion](https://www.recursion.com) - Company combining high-throughput biology with machine learning for drug discovery.

## Open-Source Tools

- [Biopython](https://github.com/biopython/biopython) - Library of tools for computational molecular biology.
- [DeepChem](https://github.com/deepchem/deepchem) - Library of deep-learning models, featurisers, and datasets for the molecular sciences.
- [Graphein](https://github.com/a-r-j/graphein) - Library for geometric deep learning on biomolecular structures and networks.
- [RDKit](https://github.com/rdkit/rdkit) - Cheminformatics toolkit for working with molecular data.
- [TorchDrug](https://github.com/DeepGraphLearning/torchdrug) - PyTorch-based machine-learning toolbox for drug discovery.

## Related Awesome Lists

- [Awesome AI-based Protein Design](https://github.com/opendilab/awesome-AI-based-protein-design) - Curated papers on AI for protein design.
- [Awesome Cheminformatics](https://github.com/hsiaoyi0504/awesome-cheminformatics) - Curated cheminformatics libraries and software.
- [Awesome Protein Representation Learning](https://github.com/LirongWu/awesome-protein-representation-learning) - Curated papers on protein representation learning.
- [Awesome Single Cell](https://github.com/seandavi/awesome-single-cell) - Curated software and resources for single-cell analysis.

## Contributing

Contributions are welcome. Please read [CONTRIBUTING.md](CONTRIBUTING.md) and the [safety boundaries](SECURITY.md) before suggesting a resource. One resource per pull request is preferred, with a short note on why it belongs. New to the list? Start with a [good first issue](https://github.com/natnew/awesome-ai-for-bioengineering/labels/good%20first%20issue).

## Contributors

This list is built and improved by the community, and every contributor is credited here.

[![All Contributors](https://img.shields.io/badge/all_contributors-0-brightgreen.svg)]

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->
<!-- ALL-CONTRIBUTORS-LIST:END -->

Recognition is handled with the [all-contributors](https://allcontributors.org) specification. After your contribution is merged, you are added to the list above.
