# Flow Cytometry Tools

These are the flow cytometry tools from napari_jflowcyte but don't include references to napari for easier import.  Here are the included modules:

importflowcyte: codes to import .fcs files; getFCSFile(path) is the key function that returns channel names, column values, and metadata.  For easier functionality use the compensateflowcyte getFileAsDF2 function.
exportflowcyte: codes to export .fcs files; write_data(path,chnames,data,meta) is the key function.
compensateflowcyte: codes to compensate and read .fcs files.  getFileAsDF2(fpath) reads a file and returns a pandas dataframde and metadata dictionary.  saveDF(fpath,df,metadict) saves an fcs file from a dataframe.  Metadict can be empty.
gateflowcyte2: codes to gate flow cytometry data (omitting the napari functions).

Dependencies are numpy, pandas, matplotlib, and numba

To install run
```bash
pip install git+https://github.com/jayunruh/flowcytetools
```
