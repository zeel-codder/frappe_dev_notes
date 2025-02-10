# Introduction to Bench CLI

Bench is a CLI tool used to manage Frappe sites. It allows you to create sites, apps, and set up the Frappe environment. Bench includes a variety of commands for different use cases. In this part, we will cover all basic aspects of the Bench CLI.

## Table of Contents

1. [bench restart](#bench-restart)
2. [bench start](#bench-start)
3. [bench list-apps](#bench-list-apps)
4. [bench get-app](#bench-get-app)
5. [bench install-app](#bench-install-app)
6. [bench uninstall-app](#bench-uninstall-app)
7. [bench remove-app](#bench-remove-app)
8. [bench reinstall](#bench-reinstall)
9. [bench setup](#bench-setup)
10. [bench migrate](#bench-migrate)
11. [bench update](#bench-update)
12. [bench build](#bench-build)
13. [bench clear-cache](#bench-clear-cache)

### bench restart

The `bench restart` command is used to restart all the workers and queues of a Frappe site. It also helps to reflect code changes in production mode.

```bash
bench restart
```

### bench start

This command is used to start the Frappe site.

```bash
bench start
```

### bench list-apps

This command lists the installed apps in the specified site.

```bash
bench --site frappe-tutorial.localhost list-apps
```

> Note: You can use the `bench use {site_name}` command to set the default site, so you don't need to pass `--site` in bench commands.

### bench get-app

To download Frappe apps, we use the `get-app` command. This will add the app code to the `/apps` directory.

```bash
bench get-app erpnext
bench get-app erpnext --branch develop
# Overwrite of app exits
bench get-app --branch=develop --overwrite=erpnext
# Download app with github link
bench get-app  https://github.com/frappe/helpdesk.git --branch=develop
```

### bench install-app

Installs the specified app in the Frappe site.

```bash
bench install-app --site frappe-tutorial.localhost erpnext
# or
bench install-app erpnext
```

### bench uninstall-app

Uninstalls the specified app from the Frappe site.

```bash
bench uninstall-app --site frappe-tutorial.localhost erpnext
# or
bench uninstall-app erpnext
```

### bench remove-app

Removes the specified app from the `/apps` directory.

```bash
bench remove-app erpnext
# or
bench rm erpnext
```

### bench reinstall

Reinstalls the specified site in Frappe, resetting the entire database to its initial state.

```bash
bench reinstall
```

### bench setup

Setup includes many subcommands, but we will only cover a few in this section.

#### bench setup requirements

This command is used to update the Python and Node environments of the system.

```bash
bench setup requirements
bench setup requirements --node
bench setup requirements --python
bench setup requirements erpnext
```

### bench migrate

This command updates the database tables as per doctype fields/custom fields and runs patches.

```bash
bench migrate
```

### bench update

Used to update the specified app version in the Frappe site.

```bash
bench update --apps erpnext frappe
```

### bench build

Generates JavaScript/CSS bundles of apps.

```bash
bench build
bench build --app erpnext
```

### bench clear-cache

Clears the page cache in the Frappe site as well as the JavaScript/CSS file cache.

```bash
bench clear-cache
bench clear-website-cache
```

GitHub Repository: https://github.com/zeel-codder/frappe_dev_notes

YT: https://www.youtube.com/watch?v=4Lgj77s_fc4