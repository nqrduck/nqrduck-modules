# NQRduck Modules
This repository contains a json file with different modules used for the nqrduck program. 
It is manually maintained and updated.

## Structure
Different modules can be added to the json file `modules.json`. 

Every module in the json file start with the `name` key. The value of the key is a string which is the name of the module.

Additionally, the json also has the option to add a `description` for the module.

A `platform` can be specified for the module. This is done by adding a `platform` key to the module. The value of the key is a string which is the platform the module is intended for. For windows, the value should be `win`. For linux, the value should be `linux`

One can add a `source` for the module which can be either a link to a git repository or a simple string. 
If the `source` is a simple string, the module is assumed to be available via PyPi.

Dependencies between different nqrduck modules can be specified in the json file. This is done by adding a `dependencies` key to the module. The value of the key is a list of strings. Each string is the name of a module that the current module depends on.

## Example
Check the `modules.json` file for an example of how the json file should be structured.