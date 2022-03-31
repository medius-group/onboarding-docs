# Onboarding content repository

This is the repository for content for the Onboarding portal. All files should be written in markdown, preferably adhering to the [CommonMark](https://commonmark.org/help/) specification.

You can use all markdown features when writing content, except for the H1 heading level. H1 heading level is generated automatically based on the frontmatter title field described below. Any H1 content present in the markdown files will be ignored and will NOT be displayed on portal pages.

Visual Studio Code comes with a markdown preview utility - you can use it to preview the documents you are writing before pushing them.

The content repository utilizes two branches ``develop`` and ``master``. All new and updated content is introduced by pull requests from feature branches to ``develop`` branch. Master branch will be used for production-ready content.

- Workflow for contributor:
  - Create feature branch
  - Update content on feature branch
  - Push changes to remote feature branch
  - Create pull request to ``develop`` branch in Bitbucket web UI
- Workflow for maintainer
  - Review pull requests
  - Create pull requests from ``develop`` to ``master`` when it's time for release

*All content in develop is automatically updated to https://onboarding-dev.mediusflow.com*

## Frontmatter

Frontmatter is used as metadata for the files you are creating. The following fields are available for using in frontmatter:

* **path**, e.g. ``"/capture/company-setup/setup-company-structure"`` - path to the page. The page will be available under the path specified here. Note that page path will never be generated automatically. This means the location of the file you are writing will not be taken into account when determining the path to the page.
* **title**, e.g. ``"Set up capture"`` - Title of the page (appears in the browser's title bar)
* **section**, e.g. ``"Company"`` - name of the section. Currently unused.
* **module**, e.g. ``"Capture"`` - name of the module in which the page should appear. Currently, the following modules are available: "MediusFlow", "Capture", "User Import", "ERP Integration".
* **next**, e.g. ``"/import/company-setup/setup-company-responsibles"`` - path to the next page in the documents structure. This field is used to construct and properly order the menu. To add page2 between page1 and page3, you must open page1, set ``next`` to the path specified on page2, and ensure page2 points to page3. A page is omitted from the entire structure if no other page has it specified in the ``next`` field. The last page in the structure should have no ``next`` field at all.
* **tags**, e.g. ``["nav"]`` - table of tags used for filtering the menu. If you specify any tags in this field, the page will be displayed in the menu only if the user checked the matching box on the configuration page.

The following tags are available:
* **general tags:** "tenantCreated"
* **application tags:** "invoice", "match", "procurement", "contract", "document_approval"
* **ERP tags:** "sap", "nav", "business_central", "d365fiop", "ax2012", "api_rest", "api_fx", "erp_other"
* **Capture tags:** "mediusflow_capture", "readsoft_online", "scancloud", "local_edi_xml_import", "capture_other"


