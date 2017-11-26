====
mona

Corelan Repository for mona.py


Installation instructions
-------------------------

### Immunity Debugger
Simply drop mona.py into the 'PyCommands' folder (inside the Immunity Debugger application folder).

### WinDBG
See https://github.com/corelan/windbglib

### x64dbg
First, get [x64dbgpy](https://github.com/x64dbg/x64dbgpy). You can grab a release [here](https://ci.appveyor.com/project/mrexodia/x64dbg-python/build/artifacts).

Drop the `plugins` directory in your `x64dbg` application folder, either `x32` or `x64`. Then, put `mona.py` into the `plugins/x64dbgpy` folder. You will also need the `pykd.py` and `x64dbgpylib.py` files from https://github.com/x64dbg/x64dbgpylib. 

Finally, put the `clean_mona.py` script inside `x64dbgpy/x64dbgpy/autorun`. 

Now, run mona commands at the x64dbg Python command line with `mona.mona(“command”)`.
