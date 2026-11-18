# PlantScience.si

**Towards plant science superintelligence.**

This repository holds the landing page at **[plantscience.si](https://plantscience.si)**. The page sets out the vision for PlantScience.si, the next step for [PlantScience.ai](https://plantscience.ai): an intelligence system that draws on all of plant science at once, from the literature and its images to plant databases, and answers with the evidence behind each claim.

## The vision

Plant science knowledge is scattered across millions of papers, images and specialised databases, and it grows every year. A researcher asking what is known about a gene, a breeder narrowing a trait interval and a student learning to weigh evidence still assemble that picture by hand.

PlantScience.si brings it together. Papers with their figures, plant databases and a gene orthology network build one knowledge graph. An AI agent reasons across it and answers each person with the evidence behind every claim.

It builds on PlantScience.ai, an AI virtual scientist for plant science whose knowledge graph holds 9.66 million entities and 47.2 million relationships, extracted from 480,253 open-access articles and each linked to its source publication.

## Four new capabilities

| Capability | What it adds |
| --- | --- |
| **Visual evidence** | Phenotype photographs, micrographs and plots from the open literature, linked to the genes, tissues and findings they show. |
| **Database integration** | Skills that query established plant bioinformatics databases directly, so answers carry real identifiers, releases and links. |
| **Education** | A teaching mode in which the AI asks the question, the student finds the evidence, and the student reaches the conclusion. |
| **Evolutionary insight** | A gene orthology network across plant genomes, showing which functions are conserved, which have diverged and where evidence is missing. |

## How it earns trust

- **Traceable.** Every statement links to the publication or database record it came from.
- **Labelled.** Literature-supported and database-supported claims are marked as such.
- **Honest about gaps.** Inferences across species are hypotheses with confidence levels, and missing evidence is shown as missing.
- **Open.** Versioned releases, an open benchmark, and an API any AI agent can use.

## Plant Science AI Initiative

PlantScience.si is meant to be built and steered by its community. Researchers, breeders, educators and database providers can contribute database skills, submit and review benchmark questions, and rank priorities on a public roadmap.

## What is on the page

1. **Hero.** A plant growing from a knowledge graph, with one leaf for each capability.
2. **PlantScience.ai today.** The numbers behind the existing platform.
3. **Supporters.** A scrolling strip of the organisations whose colleagues support the work.
4. **The vision.** An animated overview: sources, knowledge graph, AI agent, people.
5. **Capabilities.** Four cards, each with its own animated concept figure.
6. **In use.** An illustrative mock-up for a plant scientist, a wheat breeder and a student.
7. **Trust principles** and the **Plant Science AI Initiative** release cycle.
8. **Project leads.**

## About the code

The site is a single static page with no build step and no external dependencies.

```
index.html          the whole page: markup, CSS and JavaScript inline
assets/people/      portraits of the project leads
assets/logos/       logos of supporting organisations
robots.txt
sitemap.xml
```

- All concept figures are hand-written inline SVG, animated with CSS and SMIL.
- The hero background is a small canvas particle network.
- The layout adapts to phones and tablets. Below 900 px the overview figure switches to a vertical version.
- Animations are reduced for visitors who ask their system for less motion.

### Preview locally

```bash
git clone https://github.com/atlasbioinfo/PlantScience.si.git
cd PlantScience.si
python3 -m http.server 8000
```

Then open <http://localhost:8000>. Opening `index.html` directly in a browser also works.

### Deploy

Copy the repository contents to any static web host. No server-side code is needed.

## Team

- **Yiliang Ding**, Project lead. Professor and Group Leader, John Innes Centre.
- **Haopeng Yu**, Project co-lead. Principal Investigator, Sainsbury Laboratory, University of Cambridge (SLCU).

## Reference

Yu H *et al.* (2026). *Molecular Plant*. [doi:10.1016/j.molp.2026.03.010](https://doi.org/10.1016/j.molp.2026.03.010)

## Notes on assets

The logos in `assets/logos/` are trademarks of their respective organisations and are shown only to acknowledge support. They are not covered by any licence granted for this repository. The chat shown under "In use" is an illustrative mock-up, not output from a live system.
