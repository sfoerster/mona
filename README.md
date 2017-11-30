====
mona

Fork of Corelan’s mona.py for x64dbg

Installation instructions
-------------------------

### x64dbg
First, get [x64dbgpy](https://github.com/x64dbg/x64dbgpy) for x64dbg Python support. You can grab a release [here](https://ci.appveyor.com/project/mrexodia/x64dbg-python/build/artifacts). Drop the contents of the `plugins` directory into your x64dbg `plugins` folder. 

Then, put `mona.py` into the `plugins/x64dbgpy` folder. You will also need the `pykd.py` and `x64dbgpylib.py` files from https://github.com/x64dbg/x64dbgpylib. Finally, put the `clean_mona.py` script in `x64dbgpy/x64dbgpy/autorun`. 

Now, run mona commands at the x64dbg Python command line with `mona.mona(“command”)`.

### Immunity Debugger
Simply drop mona.py into the 'PyCommands' folder (inside the Immunity Debugger application folder).

### WinDBG
See https://github.com/corelan/windbglib

