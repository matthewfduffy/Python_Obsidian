## **import path**
A list of locations (or [[path entry]]) that are searched by the [[path based finder]] for modules to import.
During import, this list of locations usually comes from *sys.path* but for subpackages it may also come from the parent package's `__path__` attribute.