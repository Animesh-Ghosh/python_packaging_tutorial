# python_packaging_tutorial

Never packaged Python code, now, I have. 🙃
Followed [this](https://packaging.python.org/en/latest/tutorials/packaging-projects/) short tutorial.

## Dependencies

1. `pip` itself
2. `build`, to generate the distribution archive
3. `twine`, to upload the distribution archives to either testpyi or pypi

## Commands

```bash
py -m pip install --upgrade pip
py -m pip install --upgrade build
py -m build

# if you're uploading the archive to testpypi
py -m pip install --upgrade twine
py -m twine upload --repository testpypi dist/*
```

These create the distribution archive then we can then upload to testpyi or pypi. You'd have to create an account though.
