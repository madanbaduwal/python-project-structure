# Error in Github action(workflow)
--------------------------------------
Github action is the debugging place of  github workflows(.yml file debugging in github is github action)

# Path issue
## Relative path

```
/ =  means the root of the current drive, Root directory (mostly we use this)

.   = This location

..  = Up a directory

./ = current directory

../ = Parent of current directory ,not the root directory

../../ = Two directories backwards

```
## Folder location issue : OS module solve this

```

from pathlib import Path

BASE_DIR = Path(__file__).parent


or 


PROJ_PTH = os.path.abspath(__file__) # yo jun .py file bhitra lekhyo tyo file ko location ko absolute path denxa.

CONFIG_PATH = PROJ_PTH.split('/')[:-2]


```
------------------
# Module Error : No module

Run the following command in your terminal.
```
export PYTHONPATH="${PYTHONPATH}:/path/to/your/project/"

Exampple : export PYTHONPATH="${PYTHONPATH}:/home/madan/Desktop/mina/"
```
------------------------
# Packag publishing issue  

* **Use Poetry and virtual environment(setup.py) parallelly**
* pyproject.toml ma text haru, code formatting/styling haru lekhni and setup.py bata publish garya ni hunxa.
* Dubai lai parally use garda ni hunxa.
----------------------

# References

* https://github.com/GokuMohandas/MLOps
