# A minimal Python  package

## Try this minimal package:

Install it with:

```bash
pip install git+https://github.com/cmcouto-silva/minimal-python-package.git
```

Then, run:

```python
from my_package import utils
utils.hello()
```

# Instructions

## Code structure

You can structure your code like this:

```bash
your-package-name/
│
├── your_package/
│   ├── __init__.py
│   └── module.py
│
├── setup.py
└── README.md
```

Organize your functions inside modules (_e.g._, `module.py`). Alternatively, you can place them directly inside the `__init__.py` file.

## Package installation

Once you've pushed your code to GitHub, install your package with:

```bash
pip install git+https://github.com/yourusername/your-package-name.git
```

Easy peasy!

If you want to test your package locally before pushing it code to GitHub, you should first build the package with:

```bash
python setup.py bdist_wheel
```

It creates a dist folder with a .whl file (_e.g._, my_package-0.1.0-py3-none-any.whl). To install it, use:

```bash
pip install dist/my_package-0.1.0-py3-none-any.whl
```

## Using your package

After installing your package, you're free to use it! In case you've organized your functions in modules, you can load them with:

```python
from my_package import module
module.function()
```

In case you've placed your functions directly to the `__init__.py` file, use:

```python
from my_package import function
function()
```

## Conclusion

That's all it takes to create and reuse your Python functions effectively!

## Notes

Of course, there is a lot more to learn in order to build effective Python packages, like unit tests, linting, versioning, etc. 

Also, please note that `setup.py` is the "old-school" method. Currently, we can use `pyproject.toml` instead, with tools like `poetry` and `ruff`.

Nevertheless, it's a good starting point, right? Enjoy :)
