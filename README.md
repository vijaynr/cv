# CV (CV Generator for Command Line)

A command-line tool that converts YML into PDF and HTML. The primary use case for this tool is to allow individuals to write their resumes in YML and render them as PDFs using user-defined style templates.

## To-Do List

- [x] Design the workflow of the application
- [ ] Implement the command line options
  - [ ] `create` - Initialize the resume builder
    - [ ] Prompts the user for data to fill in the resume, which must be stored in a YAML file.
    - [ ] Invoking the command a second time should prompt the user to decide whether to overwrite the existing data or create a new one.
  - [ ] `modify` - Modify existing data
    - [ ] Users should be able to edit their data directly from the data files. This command should provide an interactive way for users to modify specific sections and fields of the resume.
  - [ ] `generate` - Generate a PDF file from the stored data
    - [ ] PDF should be the default format for the document produced. The resulting document must be a valid resume that adheres to best resume guidelines.
    - [ ] `--format` - A subcommand necessary to provide options for multiple output formats. For example, the user may want their resume in DOCX or DOC format.
    - [ ] `--style` - A subcommand necessary to offer options for creating documents with different styles. There should be at least 2 or 3 predefined styles to choose from, and these styles must be customizable.
- [ ] Finalize the libraries and tech stack that needs to be used.

## Tech Stack

- Language
  - zig
- Libraries
  - zig-yaml/ymlz - to parse yaml files
  - ? - to create html file
  - ? - to parse css files
  - ? - to convert html to pdf file
