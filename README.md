# PyYAML
The next generation YAML parser and emitter for Python.

# Install
```bash
pip install pyyaml
```
or
```bash
git clone https://github.com/yaml/pyyaml.git
cd pyyaml
python setup.py install
```
Note: By default, the `setup.py` script checks whether LibYAML is installed
and if so, builds and installs LibYAML bindings.  To skip the check
and force installation of LibYAML bindings, use the option `--with-libyaml`:
`python setup.py --with-libyaml install`.  To disable the check and
skip building and installing LibYAML bindings, use `--without-libyaml`:
`python setup.py --without-libyaml install`.

# Usage
When LibYAML bindings are installed, you may use fast LibYAML-based
parser and emitter as follows:
```python
>>> import yaml
>>> yaml.load(stream, Loader=yaml.CLoader)
>>> yaml.dump(data, Dumper=yaml.CDumper)
```

If you don't trust the input stream, you should use:
```python
>>> import yaml
>>> yaml.safe_load(stream)
```

PyYAML includes a comprehensive test suite.  To run the tests,
type `python setup.py test`.

# Links
- For more information, check the PyYAML homepage: https://github.com/yaml/pyyaml.

- For PyYAML tutorial and reference, see: http://pyyaml.org/wiki/PyYAMLDocumentation.

- Discuss PyYAML with the maintainers in IRC `#pyyaml` [irc.freenode.net](irc.freenode.net).

- You may also use the YAML-Core mailing list: http://lists.sourceforge.net/lists/listinfo/yaml-core.

- Submit bug reports and feature requests to the PyYAML bug tracker: https://github.com/yaml/pyyaml/issues.

- The PyYAML module was written by Kirill Simonov <xi@resolvent.net>. It is currently maintained by the YAML and Python communities.

# License
PyYAML is released under the MIT license. See the file LICENSE for more details.
