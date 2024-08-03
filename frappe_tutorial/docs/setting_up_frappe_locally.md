In this part of the course, we are going to set up Frappe locally using [Frappe Manager (FM)](https://github.com/rtCamp/Frappe-Manager/).

> Note: You can also set up Frappe locally by following the [official documentation](https://frappeframework.com/docs/user/en/installation).

1. First, ensure Docker is installed on your system. Then, install Frappe Manager locally using the following command:

```bash
pip install frappe-manager
```

2. Next, create a new site with the command below. This example uses Frappe version 15, but you can specify a different version if needed:

```bash
fm create frappe-tutorial --frappe-branch version-15
fm code frappe-tutorial
```

3. Visit the given URL to see the site: http://frappe-tutorial.localhost/#login

GitHub Repository: https://github.com/zeel-codder/frappe_tutorial

YT: https://www.youtube.com/watch?v=6tPyFglNklU
