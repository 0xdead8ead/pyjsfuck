PyJSFuck - Python Library for creating JSFuck Payloads
======================================================

Module for Python to create obfuscated javascript using [JSFuck](http://www.jsfuck.com/)

Utilizes a lightly modified version of [jsfuck.js](https://github.com/aemkei/jsfuck/blob/master/jsfuck.js) - [JSFuck Project](https://github.com/aemkei/jsfuck)

Big Thanks to [Martin Kleppe](http://twitter.com/aemkei) for making JSFuck! - [http://aem1k.com](http://aem1k.com)


# Dependencies

Python 2.7 - [https://www.python.org/](https://www.python.org/)
Node JS 8.5.9 - [https://nodejs.org/](https://nodejs.org/)
PyExecJs - [https://github.com/doloopwhile/PyExecJS](https://github.com/doloopwhile/PyExecJS)


# Example Usage

PyJSFuck Example Usage:

```python
from pyjsfuck import JSFuck

if __name__ == '__main__':

    ## Code to be obfuscated with JSFuck
    code = 'alert(1);'

    ## Instance of JSFuck
    jsf = JSFuck()
    
    ## Ecodes Javascript with JSFuck (Expects Single Line of Javascript)
    jsfuck_payload = jsf.encode(code)
    
    print jsfuck_payload
```



