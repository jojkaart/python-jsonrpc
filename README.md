python-jsonrpc
==============

Fork of Jan-Klaas Kollhof's jsonrpc-Implementation ( http://json-rpc.org/wiki/python-json-rpc )

His implementation is pretty cool, because it comes with it's own mod_python-handler. 

The reason i needed to fork is the fact, that i need uft8 strings in my json. The json-implementation that came with python-jsonrpc was not able to transport unicodestrings properly (at least in my tests). Python comes with it's own better-tested json module, so i changed python-jsonrpc into using Python's own module.
Since the bazaar-repository has not been changed since 2007, i forked the project instead of submitting a patch.

I like the library, because it is very lightweight. When i eventually discover other issues while using python-jsonrpc in my main project, i will submit fixes to this repository here.

This version has a slight modification by Joel Kaartinen <jkaartinen@iki.fi> to modify the behauviour when reading decimal numbers from a json file. This version now reads them with Decimal.

license
-------

python-jsonrpc is licensed under the GNU LGPL (see Copyrightnotices in Code from original Author Jan-Klaas Kollhof for Details.)
