====
mona

Fork of Corelan’s mona.py for x64dbg. mona is a Windows exploit development swiss army knife. It supports ROP techniques, SEH, cyclic patterns, etc.

### What is mona.py?

Mona.py is a python script that can be used to automate and speed up specific searches while developing exploits (typically for the Windows platform).
It runs on Immunity Debugger and WinDBG, and requires python 2.7.
Although it runs in WinDBG x64, the majority of its features were written specifically for 32bit processes.

For more info on mona.py and how to use it, please consider taking one of Corelan's exploit development classes:

https://www.corelan-training.com



Installation instructions
-------------------------

### x64dbg
First, get [x64dbgpy](https://github.com/x64dbg/x64dbgpy) for x64dbg Python support. You can grab a release [here](https://ci.appveyor.com/project/mrexodia/x64dbg-python/build/artifacts). Drop the contents of the `plugins` directory into your x64dbg `plugins` folder. 

Then, put `mona.py` into the `plugins/x64dbgpy` folder. You will also need the `pykd.py` and `x64dbgpylib.py` files from https://github.com/x64dbg/x64dbgpylib. Finally, put the `clean_mona.py` script in `x64dbgpy/x64dbgpy/autorun`. 
 
Now, run mona commands at the x64dbg Python command line with `mona.mona(“command”)`.

### Immunity Debugger
1. drop mona.py into the 'PyCommands' folder (inside the Immunity Debugger application folder).
2. install Python 2.7.14 (or a higher 2.7.xx version) into c:\python27, thus overwriting the version that was bundled with Immunity. This is needed to avoid TLS issues when trying to update mona.  Make sure you are installing the 32bit version of python.

### WinDBG
See https://github.com/corelan/windbglib



notes
-----

mona.py has been inventoried at Rawsec's CyberSecurity Inventory
[![Rawsec's CyberSecurity Inventory](https://inventory.rawsec.ml/img/badges/Rawsec-inventoried-FF5050_plastic.svg)](https://inventory.rawsec.ml/)