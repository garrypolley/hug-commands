# hug-commands

This is a fun repo for testing out [hug](http://www.hug.rest/website/quickstart).

The biggest thing to remember is the shebang at the start of the python file and making it excutable. 

```py
#!/usr/bin/env python
"""Description of what it does"""
import hug


@hug.cli()
@hug.get(example='arg1=T&arg2=DD')
@hug.local()
def your_func():
    pass

if __name__ == '__main__':
    your_func.interface.cli()
```

Then make your file executable.

```sh
chmod a+x your_func.py
```

Now you can run the file: `./your_func.py`

