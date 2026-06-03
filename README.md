# Big Data Analytics Project

## Authors

- Beatris Daicu - 20221854
- Diogo Carvalho - 20221935
- Ricardo Pereira - 20250343
- Yehor Malakhov - 20221691

## Installation

The data used in the notebooks can be found in
<files.diogohlcarvalho.pt/shared/data-G13/data-G13.zip>. Note that this is a
selfhosted environment, and as such, there may be downtimes. If that is the
case, a backup can be downloaded from
<https://liveeduisegiunl-my.sharepoint.com/:u:/g/personal/20221935_novaims_unl_pt/IQBL6M7jnAqpTqWA-fUWDcJ4AbtDCn4XbrjE1svC_ZWCm10?e=UWkWEM>.
The data must be placed in a data folder in the root of the project.

### With Dev Container

If you have docker installed, you can install the Dev Containers VSCode
extension and use the provided dev container to setup the environment for you.
The dev container automatically installs the correct Python version, the
required packages, and Java. You can create and enter the dev container by using
the command "Dev Containers: Reopen in Container" in the VSCode command pallette
(CTRL + Shift + P).

### Without Dev Container

Java 21 was used in the project, you must install it and confirm its
installation path. Replace all references of path in os.environ["JAVA_HOME"] =
path in the notebooks with the path to your Java 21 installation.

If you're using pip, create a virtual environment with Python 3.14 before
installing the packages to avoid conflicts with other versions of packages. If
you're using [uv](https://docs.astral.sh/uv/), this is automatically handled for
you.

The code has not been tested on other Python versions, the versions of the
packages that were used might only be compatible with Python 3.14.

#### Using pip

```bash
pip install -r "requirements.txt"
```

#### Using uv

```bash
uv sync
```
