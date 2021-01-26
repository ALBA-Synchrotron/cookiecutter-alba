# ALBA cookiecutter

Use it to bootstrap an ALBA python software project:

```console
$ cookiecutter https://github.com/alba-synchrotron/cookiecutter-alba
full_name [ALBA computing team]: ALBA controls team
email [computing@cells.es]: constrols-software@cells.es
github_username [alba-synchrotron]: 
project_name [ALBA software]: ALBA HPLab
project_slug [alba-hplab]: 
py_package [hplab]: 
project_short_description [ALBA's python software package]: ALBA's HPLab control software
version [0.0.1]: 
min_python [3.5]: 
use_pytest [y]: 
add_pyup_badge [y]: 
create_author_file [y]: 
use_taurus [y]: 
use_sardana [n]: 
Select open_source_license:
1 - GNU General Public License v3
2 - MIT license
3 - BSD license
4 - ISC license
5 - Apache Software License 2.0
6 - Not open source
Choose from 1, 2, 3, 4, 5, 6 [1]:
```

Notice that we only need to type a few values. for most options we try to have a sane default value.

Also notice that the package name is simply `hplab`. All packages created with this recipe will be
under the namespace `alba`. So the full package name is `alba.hplab`.
If you need something other than this then maybe this is not the best recipe for you.

This will create the directory structure:

```
alba-hplab/
├── alba
│   ├── hplab
│   │   └── __init__.py
│   └── __init__.py
├── AUTHORS.md
├── CONTRIBUTING.md
├── HISTORY.md
├── LICENSE
├── Makefile
├── MANIFEST.in
├── README.md
├── requirements_dev.txt
├── setup.cfg
├── setup.py
├── tests
│   ├── __init__.py
│   └── test_hplab.py
└── tox.ini

3 directories, 15 files
```

