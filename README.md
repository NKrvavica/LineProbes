# OpenFOAM water level probes

Python script for generating water-level time series data from VOF data at line probes (from *alpha.water.xy files).
Water elevation is computed at each time step as the depth at which alpha=0.5
The results are writen to a .csv file with columns corresponding to line probes and rows corresponding to time steps.

# Requirements

Python 3+, Numpy, Pandas, Scipy

# Installation

Download the file [`get_line_probes.py`](get_line_probes.py) and put it in the case OpenFOAM directory, where postProcess is located, and run it by typing:
```bash
$ python get_line_probes.py
```

If you wish to use it repeatedly, a good idea would be to make it executable and add it to your $PATH, which simplifies usage and makes it possible to use it in any directory:
```bash
$ get_line_probes
```

# License

[MIT license](LICENSE)
