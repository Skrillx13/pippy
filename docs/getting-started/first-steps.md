# First Steps with Pippy

This document will guide you through the basics of pippy. This includes, installing a package, managing multiple packages, and the `Pippy` file.

## Installing a package

Alright. So first, navigate to the directory you wish for the package to be installed in. For this example, we will be installing [requests](https://github.com/psf/requests). Now, run this command:

``` console
pippy install requests
```

Automatically, Pippy will create a virtual enviroment for you to work with. You will notice a `venv` folder appearing in your project. If `venv` has not been added to a `.gitignore`, Pippy will automatically do that for you.

## Introduction to `Pippy` file

You will also notice a `Pippy` file appearing in your project. This is the main file for handling all your packages. It should look something like this:

!!! info "The `Pipfile` is actually authored in YAML format, as it was the easiest to read and work with."

``` yaml
packages:
  - requests==2.32.3
  - charset-normalizer==3.4.0
  - idna==3.10
  - urllib3==2.2.3
```

You will see that the requests package has been listed, along with it's dependencies. More about `Pipfile` can be read [here](#).