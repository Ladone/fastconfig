```
 _____            _      _____            ___  _      
|   __| ___  ___ | |_   |     | ___  ___ |  _||_| ___ 
|   __|| .'||_ -||  _|  |   --|| . ||   ||  _|| || . |
|__|   |__,||___||_|    |_____||___||_|_||_|  |_||_  |
                                                 |___|
```

About
=====

Fast Config — it's bash tool how help fast change configs for your projects.

Table of Contents
=================

<!--ts-->
* [About](#about)
* [Table of Contents](#table-of-contents)
* [Quick Start](#table-of-contents)
* [Usage](#usage)
  * [Params of fastconfig.ini](#params-of-fastconfigini)
  * [Config](#config)
  * [Switch config](#switch-config)
* [License](#license)
<!--te-->

Quick Start
===========
FastConfig can has been installed for some steps:
1. Clone project to your folder: `git clone git@github.com:Ladone/fastconfig.git`;
2. Enter to directory FastConfig: `cd fastconfig`;
3. Add alias to FastConfig `./fastconfig -a myFirstAlias`
When you do this steps in root directory FastConfig has been created fastconfig.ini,
how contains your alias. For this alias need edit directives for correct paths and names
for your project;
4. And you need call command how copy to FastConfig file from your project `./fastconfig -g`;
5. Edit your config in FastConfig config directory and call `./fastconfig -s myFirstAlias`
how copy your config to project directory with name how set in `output_file`.

Usage
=====
Params of fastconfig.ini
------------------------
1. root — it's directive how set project root folder;  
2. output_file_name — it's directive how change name your config when you use `switch` command;  
3. source_file — directive how you need set source file. From this file generate file for future switch file;  
4. output_file – path to generated file how put after use command switch.  


Config
---------------
Config file it's `fastconfig.ini` how place on the root folder fastConfig. FastConfig contains from alias name how create square brackets and some directives.
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


Switch config
-------------
Before switch config you need prepare FastConfig alias and use `./fasconfig -s aliasname`

License
=======
MIT License

Copyright (c) 2020 Vladislav Pototskiy

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.