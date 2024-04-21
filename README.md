# Ansible Role: Python

Role to download and install the [Python](https://www.python.org/) programming language.

## Requirements

None.

## Role Variables

The following variables will change the behavior of this role (default values
are shown below):

```yaml
# Python SDK version number
python_version: "3.12.1"

# Mirror to download the Python SDK from
python_mirror: "https://www.python.org/ftp/python"

# Directory to store the files downloaded for Python SDK installation
python_download_dir: "/tmp"
```

### Supported Python SDK Versions

The following versions of the Python SDK are supported without any additional
configuration:

* `3.12.1`
* `3.11.7`
* `3.10.13`
* `3.9.18`

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
     - role: reidaa.python
```

```yaml
- hosts: all
  roles:
     - role: reidaa.python
       python_version: "3.9.18"
```
