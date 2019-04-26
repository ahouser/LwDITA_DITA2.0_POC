# LwDITA_DITA2.0_POC
Proof-of-Concept for sharing LwDITA and DITA 2.0 spec content

Here we (members of the Lightweight DITA Subcommittee of the OASIS DITA Technical Committee) provide proof-of-concept Lightweight DITA specification topics and necessary support files (reusable content collections) to demonstrate content sharing between Lightweight DITA and DITA 2.0.

This repository includes:

- draft spec topics for LwDITA components: dita, xref, shortdesc, and b
- ditamap
- reusable content topics: shortdesc.dita and lw_attributes.dita

@props is used as a filtering attribute, with values "dita2.0" and "lwdita".

## Assessments from this exercise

Analysis confirms that the TC's requirement to reuse DITA 2.0 spec content puts a substantial burden on editors of the Lightweight DITA specification, with few benefits. Specifically:

- This level of reuse nullifies the goal of the SC to author the Lightweight DITA specification in Lightweight DITA.

- Many differences in use cases between Lightweight DITA and DITA make sharing content highly tedious. For example, in DITA, the <data> element type provides a basis for specialization. In Lightweight DITA, it does not. (At least for Lightweight DITA 1.0, the SC has chosen to de-emphasize specialization). During this exercise, we find ourselves "cherry-picking" content from DITA 2.0 topics, often at the mid-paragraph sentence level.

- The required variations in content between Lightweight DITA and full DITA further increase the complexity of content sharing. Examples: Lightweigt DITA spec topics must address three source formats (HDITA, MDITA, and XDITA). The Lightweight DITA SC prefers the term "components" over "elements" or "element types", to explicitly avoid any perception that XML is a preferred Lightweight DITA source format.

## Notes from Carlos (unedited)

- Cannot write topics as XDITA/LwDITA (no <example> and other tags)
- Can we bring our own examples?
- Rework/filter indexterms
- Topic titles have to be component and not element (e.g., short description instead of <shortdesc>)
