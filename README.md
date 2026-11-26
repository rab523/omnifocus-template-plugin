# Template Chooser for OmniFocus

Adds a user interface to OmniFocus for creating projects from TaskPaper templates. Turn reusable project plans into tasks with planned dates and due dates calculated from a date you choose. Adapt the templates for your own use.

## Install and use

1. Download [Template Chooser](https://github.com/rab523/omnifocus-template-plugin/raw/refs/heads/main/TemplateChooser-Shared.zip) and unzip it.
2. Open `TemplateChooser-Shared.omnifocusjs` with OmniFocus and follow its plug-in installation prompt. This requires an OmniFocus version that supports Omni Automation.
3. Choose **Template Chooser - Shared** from the Automation menu.
4. Select **Plan a Trip**, **Host a Dinner**, or **Organize a Room**, fill in the requested fields, and choose **Create Project**.

The shared plug-in has its own identifier so it can coexist with another Template Chooser. Keep customized personal templates in a separate local copy.

## Customize

Edit the `TEMPLATES` section in a text editor. Each template has a name, placeholder definitions, and TaskPaper text. Text placeholders use `«projectname»`; date placeholders can use offsets such as `«duedate» -14d`, `-4w`, or `-2d 3pm`. Put date placeholders inside TaskPaper date tags, such as `@due(«duedate» -7d)`.

The included examples are generic. Replace them locally with your own templates.
