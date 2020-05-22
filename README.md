# easiercfg

Python Module for **Config-Files** focused on easy usage.

## Getting Started

#### Prerequisites
This module assumes you have a file called `config.ini` in the same directory as the module.

**`config.ini` should look like this:**
````
[settings]
name = linus
time = 18:00
path = C:\Program Files (x86)
log errors = false
````

#### Installation

````python
pip install easiercfg
````

## Usage

#### Import

````python
from easiercfg import Config

config = Config()
````

#### Get value of key-value-pair

````python
config.Get('name')
config['name']
````

#### Set value of key-value-pair

````python
config.Set('name', 'linus')
config['name'] = 'linus'
````

#### Show all key-value-pairs

````python
config.Show()
````