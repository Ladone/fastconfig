```
 _____            _      _____            ___  _      
|   __| ___  ___ | |_   |     | ___  ___ |  _||_| ___ 
|   __|| .'||_ -||  _|  |   --|| . ||   ||  _|| || . |
|__|   |__,||___||_|    |_____||___||_|_||_|  |_||_  |
                                                 |___|
```

About
=====

Fast Config — it's bash tool how help fast change configs for Yii2 projects.

Table of Contents
=================

<!--ts-->
* [About](#about)
* [Table of Contents](#table-of-contents)
* [Plans](#plans)
* [Usage](#usage)
  * [Install](#install)
  * [Generate config](#generate-config)
  * [Switch config](#switch-config)
* [License](#license)
<!--te-->

Plans
=====
1. Init project
2. Add new alias to fastconfig
3. Copy source file from Yii project to directory (with generate command)
4. Switch project


Usage
=====

Params of fastconfig.ini
------------------------
1. root — it's directive how set project root folder;  
2. output_file_name — it's directive how change name your config when you use `switch` command;  
3. source_file — directive how you need set source file. From this file generate file for future switch file;  
4. output_file – path to generated file how put after use command switch.  


Init project
------------


Config
---------------
Config contains from alias name how create square brackets and some directives.
For example config:
```
[example]
source_file = path/to/config.php
source_config_name = config_name
output_dir = path/to/config.php
output_file_name = output_file_name
```

1. [alias_name] — it's head block how say fastconfig alias name;
2. source_file — need set path to your current file for this alias;
3. output_dir — path to work project how source_file be put when user use switch;
4. output_file_name — output file name in working dir.


Directives
==========

source_file = path/to/config.php
source_config_name = YOURNAME
output_dir = path/to/config.php
output_file_name = output_file_name

Switch config
-------------

License
=======