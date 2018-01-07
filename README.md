# Florid Scanner
An active scanner specially for CTF Games

### Usage:

```
python florid.py -h
python florid.py -u "http://testphp.vulnweb.com/product.php?pic=1" -m "gitcheck, vimdown"
python florid.py -u "http://testphp.vulnweb.com/product.php?pic=1" -m ALL
```

![](./DOCUMENT/show.png)

### Note

Modules to run before the check starts should be placed in `./module/phase_one`

Modules for checking URLs should be placed in `./module/phase_two/`

You are expected to develop your modules referring to `./module/phase_two/sample-2.py`

### To do List

* Turn those URLs transferred between components into URL object, so that the scnner need't to redundant request.  
* Accelerate the crawling by multi-thread spider instead of the current single-thread one.
* Multi-threading Lock should be added although there is no problem with the shared virables.

### Update Log


#### v 3.2.4
* New module "djangodebug" added
* Modification to warning information
* By the way, does multi-threading crawler really help?

#### v 3.2.3
* Module "pathleak" added
* Comment added
* Directory _config_ added
* Headers for request modified
* Skip parser when picture found

#### v 3.2.2
* Fix bugs
* Add comment
* Try to allow customed configuration

#### v 3.2.1
* Configuration file added
* Two modes available after you terminate the scanning process

#### v 3.2.0

* "Ctrl+C" can terminate the url crawling.You wont's lose the result you have found.
* Modification to the module "sample-2"
* Modification to word-lists

#### v 3.1.1

* New interface
* Screenshot update
* Readme file update
* Bugs fix
