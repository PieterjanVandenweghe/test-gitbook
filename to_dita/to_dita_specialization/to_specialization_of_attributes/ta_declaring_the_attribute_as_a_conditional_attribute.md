---
authorinformation:
  - null
  - Pieterjan Vandenweghe
keyword: null
---

# Declaring the attribute as a conditional attribute

We continue in the topic.dtd file.

1. Search for DOMAINS ATTRIBUTE OVERRIDE.

   You find a list of included domains:

   ```text
   <!ENTITY included-domains
                             "&reference-att;
                              &abbrev-d-att;
                              &deliveryTargetAtt-d-att;
                              &equation-d-att;
                              &hazard-d-att;
                              &hi-d-att;
                              &indexing-d-att;
                              &markup-d-att;
                              &mathml-d-att;
                              &pr-d-att;
                              &relmgmt-d-att;
                              &sw-d-att;
                              &svg-d-att;
                              &ui-d-att;
                              &ut-d-att;
                              &xml-d-att;
     "
   >
   ```

2. Go to the next line and add `&` followed by the name of the attribute `ngs_system` and end `-d-att;`.

   ```text
   <!ENTITY included-domains
                             "&reference-att;
                              &abbrev-d-att;
                              &deliveryTargetAtt-d-att;
                              &equation-d-att;
                              &hazard-d-att;
                              &hi-d-att;
                              &indexing-d-att;
                              &markup-d-att;
                              &mathml-d-att;
                              &pr-d-att;
                              &relmgmt-d-att;
                              &sw-d-att;
                              &svg-d-att;
                              &ui-d-att;
                              &ut-d-att;
                              &xml-d-att;
                              **&ngs\_system-d-att;
   **  "
   >
   ```

3. Save the file.

You completed all changes in the DTD file.

Now we will declare the DTD files in the DITA-OT plug-in: [Declaring files in the DITA catalog file](declaring_files_in_the_dita_catalog.md)

