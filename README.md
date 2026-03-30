# Detecting unexploded ordinance using synthetic electromagnetic data

The idea comes from the master's thesis of Leonard Pasion who showed that the response of a buried metal object can be described using a small set of parameters, related to its physical properties. In real surveys most detected objects are not actually ordnance and there can be over a hundred non ordnance items for every real UXO. If we can identify which targets are likely UXO before digging then we save time, effort and money.

## Installation
Use conda force to install geoana
```bash
conda install -c conda-forge geoana
```
If Numpy, Matplotlib and SciPy not installed...
```bash
pip install numpy matplotlib scipy
```

## Usage
```python
import geoana

from geoana import utils, spatial
from geoana.em import static
```
```python
# part of building the dipole and pole in a wholespace
dipole = static.MagneticDipoleWhileSpace(location, orientation, moment)

# creates a grid to plot dipoles on
xyz = utils.ngrid([x,y,np.r_[1.]]))
```

## Contributing

Pull requests are welcome, if there is a major issue that needs attention please open an issue first to discuss.

## License
[MIT](https://choosealicense.com/licenses/mit/)
