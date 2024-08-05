# Introduction to Module

Every Frappe app is divided into multiple modules. A module includes desk pages, reports, website pages, templates, public files, DocTypes etc.

```bash
.
├── config
├── custom_module
│   └── doctype
│       └── custom_doctype
├── my_app
│   └── doctype
│       ├── child
│       ├── parent
│       ├── single
│       ├── tree
│       └── virtual
├── public
│   ├── css
│   └── js
├── templates
│   ├── includes
│   └── pages
└── www

20 directories
```


> Note: Every app has a default module with the app name, and this module holds the `hooks.py` file.


## Create a Module in Frappe

With the help of the `Module Def` DocType, we can create a custom module in Frappe.

![module_create](./images/module_create.png)
