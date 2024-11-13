# Installation

Pippy first has to be installed on a user-wide basis, which can easily be done with the help of our installation scripts.

!!! note

    Our installation scripts are developed in a [seperate repository](https://youtu.be/xvFZjo5PgG0?si=60lS8wgxL7CVYSwr). Please consider contributing! :material-heart:

=== "MacOS/Linux"

    ``` console
    curl -LsSf https://github.com/Skrillx13/Pippy-Scripts/tree/main/install.sh | sh
    ```

=== "Windows"

    ``` console
    powershell -ExecutionPolicy ByPass -c "irm https://github.com/Skrillx13/Pippy-Scripts/tree/main/install.sh | iex"
    ```

This will install Pippy onto your system. You can then verify that Pippy is installed by opening a new terminal, and running:

``` console
pippy -v
```

## Installing a specific version

While we typically recommend going for the [stable release](#installation) of Pippy, you can also choose to download specific versions. Copy the installation scripts, and replace the number "3.1" with your desired version.

=== "MacOS/Linux"

    ``` console
    curl -LsSf https://github.com/Skrillx13/Pippy-Scripts/tree/main/3.1/install.sh | sh
    ```

=== "Windows"

    ``` console
    powershell -ExecutionPolicy ByPass -c "irm https://github.com/Skrillx13/Pippy-Scripts/tree/main/3.1/install.sh | iex"
    ```

## Installing for development

We also offer a developer version of Pippy. **Under no circumstances should this be used for production, only for Pippy development.**

=== "MacOS/Linux"

    ``` console
    curl -LsSf https://github.com/Skrillx13/Pippy-Scripts/tree/main/dev/install.sh | sh
    ```

=== "Windows"

    ``` console
    powershell -ExecutionPolicy ByPass -c "irm https://github.com/Skrillx13/Pippy-Scripts/tree/main/dev/install.sh | iex"
    ```

## Managing multiple versions

When Pippy is installed onto your computer, it stores itself in a folder. For each version of pippy you download, it will store itself in a new folder, ensuring there are no conflicts between versions.

To use a specific version of Pippy (or the development version), you can run the command:

``` console
pippy -v 3.1
```

Replace 3.1 with your desired version. If you are using the dev build, replace 3.1 with "dev".

## Uninstallation

While we are sad to see you go, we understand. Perhaps you didn't like Pippy. or found a better tool.

Pippy will self-uninstall with this command:

``` console
pippy -s uninstall
```

!!! danger

    Running `pippy -s uninstall` will delete **all** versions of Pippy on your system. To uninstall a version, add the version number before uninstall, like so: `pippy -s 3.1 uninstall`.