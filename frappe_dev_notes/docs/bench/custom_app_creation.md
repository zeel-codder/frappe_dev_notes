# Create Custom App in Frappe

In this part, we will cover how to create a custom app in Frappe and install it on a site.

## Steps

1. **Create Custom App**

Use the `bench new-app` command to create the custom app in Frappe.

```bash
bench new-app my_app
```

You will be prompted to provide the following details:

```
App Title [My App]: 
App Description: The is test app
App Publisher: zeelprajapati321@gmail.com
App Email: zeelprajapati321@gmail.com
App License (agpl-3.0, apache-2.0, bsd-2-clause, bsd-3-clause, bsl-1.0, cc0-1.0, epl-2.0, gpl-2.0, gpl-3.0, lgpl-2.1, mit, mpl-2.0, unlicense) [mit]: 
Create GitHub Workflow action for unittests [y/N]: n
'my_app' created at /workspace/frappe-bench/apps/my_app
```

2. **Install App on Site**

```bash
bench install-app my_app
```

3. **Check if the App is Installed on the Site**

```bash
bench list-apps
```