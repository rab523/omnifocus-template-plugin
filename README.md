# Template Chooser for OmniFocus

Create projects from reusable TaskPaper templates. Choose a template, enter its name and date, and the plug-in calculates the task dates before importing the project.

## Install and use

1. Download [TemplateChooser-Shared.omnifocusjs](TemplateChooser-Shared.omnifocusjs?raw=true).
2. Open the downloaded file with OmniFocus and follow its plug-in installation prompt. This requires an OmniFocus edition that supports Omni Automation.
3. Choose **Template Chooser - Shared** from the Automation menu.
4. Select **Plan a Trip**, **Host a Dinner**, or **Organize a Room**, fill in the requested fields, and choose **Create Project**.

The shared plug-in has its own identifier so it can coexist with another Template Chooser. Keep customized personal templates in a separate local copy.

## Customize

Edit the `TEMPLATES` section in a text editor. Each template has a name, placeholder definitions, and TaskPaper text. Text placeholders use `«projectname»`; date placeholders can use offsets such as `«duedate» -14d`, `-4w`, or `-2d 3pm`. Put date placeholders inside TaskPaper date tags, such as `@due(«duedate» -7d)`.

The included examples are generic. Replace them locally with your own templates. Avoid committing names, phone numbers, private links, or personal schedules to a public repository.

## Privacy and status

The plug-in runs locally and passes generated TaskPaper to OmniFocus through its URL scheme. It contains no account credentials, personal templates, or external service integration. Projects you create remain in your own OmniFocus database and follow your OmniFocus sync settings.

Version 1.2.1 includes three everyday starter projects and preserves punctuation after text placeholders, including the colon that identifies a TaskPaper project. Syntax and date/template processing were checked with synthetic examples. Installation and project creation in OmniFocus still need a fresh end-to-end check of this shared version.
