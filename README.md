# LwDITA to DITA2.0 POC
Proof-of-concept for sharing LwDITA and DITA 2.0 spec content

Here we (members of the Lightweight DITA Subcommittee of the OASIS DITA Technical Committee) provide proof-of-concept Lightweight DITA specification topics to demonstrate content reuse between Lightweight DITA and DITA 2.0.

This repository includes draft spec topics for LwDITA components: data, cross reference, short description. `@props` is used as a filtering attribute, with values "dita2.0" and "lwdita".

## Assessments from this exercise

Analysis confirms that the TC's requirement to reuse DITA 2.0 spec content puts a substantial burden on editors of the Lightweight DITA specification, with few benefits. Specifically:

- This level of reuse nullifies the goal of the SC to author the Lightweight DITA specification in any of the initial Lightweight DITA authoring formats. For example, XDITA does not have the DITA `<example>` or `<xmlelement>` tags, which are heavily used in the DITA 2.0 topics.

- (Related) Conref'ing/Keyref'ing directly from DITA 2.0 topics to Lightweight DITA is not possible, except for components provided in Lightweight DITA (namely `<shortdesc>`).

- Many differences in use cases between Lightweight DITA and DITA make sharing content highly tedious. For example, in DITA, the `<data>` element type provides a basis for specialization. In Lightweight DITA, it does not. (At least for Lightweight DITA 1.0, the SC has chosen to de-emphasize specialization). During this exercise, we find ourselves "cherry-picking" content from DITA 2.0 topics, often at the mid-paragraph sentence level.

- The required variations in content between Lightweight DITA and full DITA further increase the complexity of content sharing. Examples: Lightweight DITA spec topics must address three source formats (HDITA, MDITA, and XDITA). The Lightweight DITA SC prefers the term "components" over "elements" or "element types", to explicitly avoid any perception that XML is a preferred Lightweight DITA source format.

## Additional notes

* The LwDITA SC would like to bring its own examples for the LwDITA spec
* We would need to rework/filter indexterms
* In a Lightweight DITA spec, topic titles have to be components and not elements (e.g., short description instead of `<shortdesc>`)
