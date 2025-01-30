# Mappings to External repositories and other standards

This folder contains mappings from the **Wastewater Contextual Data Specification** to external data standards such as INSDC and others. Each mapping is documented in a separate Excel file.

## Contents

- `NCBI_PHA4GE-Wastewater_mapping.xlsx`: Maps fields from the PHA4GE Wastewater Contextual Data Specification to existing attributes packages including; NCBI BioSample SARS-CoV-2_wwsurv and sequence read archive (SRA).
- `ENA_PHA4GE-Wastewater_mapping.xlsx`: Maps fields from the PHA4GE Wastewater Contextual Data Specification to existing packages including; ERC000023: GSC MIxS wastewater sludge and ERC000036 ENA sewage checklist.
- `PHA4GE-to-ODM-dictionary.xlsx`: Maps fields from the PHA4GE Wastewater Contextual Data Specification to the PHES-ODM structure. 

## Excel File Structure

### PHA4GE to NCBI

**SRA_template:** The metadata attributes for SRA submission, including picklists. For reference only.
**SARS-CoV-2_wwsurv_BioSample_template:** The metadata attributes for a BioSample submission, including picklists, for the SARS-CoV-2_wwsurv package. For reference only.
**GenomeTrakr_NWSS_BioSample_template:** The metadata attributes for a BioSample submission, including picklists, for the SARS-CoV-2_wwsurv package. For reference only.
**PHA4GE_to_NCBISRA_fields:** The mapping for the PHA4GE fields to the INSDC equivalent.
- Source ID: The ontology ID attributed to the source field in the PHA4GE Wastewater Contextual Data Specification (e.g., GENEPIO:0001123).
- Source field title: The name/title attributed to the PHA4GE field in the Wastewater Contextual Data Specification.
- Target field title: Corresponding field name in the external standard.
- Target field type: The data type of the target field (e.g., string, integer).
- Transformation rule: A broad category that describes the transformation rule used to map the source field to the target field (e.g., one to one, concatenate).
- Details: Additional information or instructions for the mapping, such as specific considerations or contextual notes (e.g. "in target_field concatenate values from 'sequencing protocol' and 'genomic target enrichment method' ").
**PHA4GE_to_NCBIBioSample_fields:** The mapping for the PHA4GE fields to the INSDC equivalent.
- Source ID: The ontology ID attributed to the source field in the PHA4GE Wastewater Contextual Data Specification (e.g., GENEPIO:0001123).
- Source field title: The name/title attributed to the PHA4GE field in the Wastewater Contextual Data Specification.
- Target field title: Corresponding field name in the external standard.
- Target field type: The data type of the target field (e.g., string, integer).
- Transformation rule: A broad category that describes the transformation rule used to map the source field to the target field (e.g., one to one, concatenate).
- Details: Additional information or instructions for the mapping, such as specific considerations or contextual notes (e.g. "in target_field concatenate values from 'sequencing protocol' and 'genomic target enrichment method' ").
**PHA4GE_to_NCBIALL_values:** The mapping for values from the PHA4GE Wastewater Contextual Data Specification to their NCBI equivalent
- SOURCE_field: The name of the PHA4GE field (e.g. 'sequencing assay') and associated values (e.g. 'Whole genome sequencing')
-TARGET_field: The name of the NCBI equivalent field (e.g. 'library_strategy') and equivalent value (e.g. WGS)

### PHA4GE to ENA

PHA4GEWW_to_ENAERC000023_fields: The mapping for the PHA4GE fields to the INSDC equivalent.

***To be updated***

## How to Use

**Review the mappings:** Open the relevant Excel file to understand how fields in the Wastewater Contextual Data Specification map to the target standard.

**Implement transformations:** Use the provided transformation logic to adapt your data for compatibility with the target standard.

**Contribute updates:** If you notice inaccuracies or have suggestions for improvements, please open an issue or submit a pull request to this repository.

## Contribution Guidelines

Ensure mappings are clear and consistent with the target standard's documentation.
Use examples that accurately reflect the use case of the mapped fields.
Include detailed descriptions and transformation logic where applicable.