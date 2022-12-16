# openMINDS_specimenPrep
A metadata model for specimen preparation in neuroscience; an openMINDS extension

<a href="/img/light_openMINDS-specimenPrep-logo.png">
    <img src="/img/light_openMINDS-logo.png" alt="openMINDS specimenPrep logo" title="openMINDS specimen preparation" align="right" height="70" />
</a>

The **openMINDS_specimenPrep** repository is part of the **open** **M**etadata **I**nitiative for **N**euroscience **D**ata Structures (**openMINDS**). It extends openMINDS core, by providing schema-templates for adding metadata about specimen preparation (cell culture, surgery, tissue slicing, etc.)

The major versions are developed and maintained in different version-branches. The default branch is always the latest version-branch.
**Each version can be accessed by checking out the corresponding version-branch.** No major version branch has yet been released. This README describes the development branch ("main").

For more information on openMINDS in general and the processing pipelines for the schema-templates please go to the main repository: https://github.com/HumanBrainProject/openMINDS

## schemas
The computation schemas are defined as JSON-schema inspired templates with only a few customized technical properties (prefixed with `"_"`). These simplified schema-templates are easy to read and can be robustly translated to other, well known target formats (e.g., HTML, JSON-schema, etc.).

## tests
In **tests** you can find JSON-LD documents designed to test the validation behaviour of each schema.
Each document follows the naming convention `{schema_name}-{custom_test_name}.jsonld`. For test cases supposed to fail the validation, the suffix **`-nok`** should be attached (`{schema_name}-{custom_test_name}-nok.jsonld`). The tests are validated every time a change is introduced and therefore ensure the correct behavior of the schemas.

## examples
In **examples** you will find several possible serializations of the openMINDS_computation metadata model. The scope of each example is described in its README. The correspondingly generated JSON-LD documents may be further structured (e.g., grouped according to the schema they are validated against).

## How to contribute
Please check our [contribution document](./CONTRIBUTING.md).

## License
This work is licensed under the MIT License.
