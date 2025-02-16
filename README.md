[![Pylint](https://github.com/m-erhardt/check-cisco-plugins/actions/workflows/pylint.yml/badge.svg)](https://github.com/m-erhardt/check-cisco-plugins/actions/workflows/pylint.yml) [![pycodestyle](https://github.com/m-erhardt/check-cisco-plugins/actions/workflows/pycodestyle.yml/badge.svg)](https://github.com/m-erhardt/check-cisco-plugins/actions/workflows/pycodestyle.yml) [![Release](https://img.shields.io/github/release/m-erhardt/check-cisco-plugins.svg)](https://github.com/m-erhardt/check-cisco-plugins/releases)
# check-cisco-plugins

## About
* this repository contains a collection of Icinga / Nagios plugins to monitor Cisco IOS and NX-OS devices via SNMPv3
* Written for python 3
* Uses SNMPv3 in AuthPriv or authNoPriv mode

### Compatibility
these plugins were developed / tested on the following models:
* Cisco Catalyst 2960-S Series
* Cisco Catalyst 2960-X Series
* Cisco Catalyst 3650 Series
* Cisco Catalyst 9200 Series
* Cisco Catalyst 9300 Series
* Cisco Nexus 3000 Series
* Cisco Nexus 5600 Series

## Documentation
* [check_cisco_cpuload.py](docs/check_cisco_cpuload.md)
* [check_cisco_envtemp.py](docs/check_cisco_envtemp.md)
* [check_cisco_memusage.py](docs/check_cisco_memusage.md)
* [check_cisco_stackmodules.py](docs/check_cisco_stackmodules.md)

### Installing dependencies
* `pip3.6 install -r requirements.txt`

## Contributing
* You're welcome to open pull requests
* When contributing code please make sure if follows the [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide
* Test your code with pep8 and pylint to avoid obvious issues
  * `pycodestyle ./*.py --max-line-length=100`
  * 
    ```bash
    pylint ./*.py \
      --disable=duplicate-code \
      --disable=too-many-branches \
      --disable=too-many-locals
    ```
