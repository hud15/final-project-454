# Detecting unexploded ordinance using synthetic electromagnetic data

The idea comes from the master's thesis of Leonard Pasion who showed that the response of a buried metal object can be described using a small set of parameters, related to its physical properties. In real surveys most detected objects are not actually ordnance and there can be over a hundred non ordnance items for every real UXO. If we can identify which targets are likely UXO before digging then we save time, effort and money.

## Installation
```python
git clone https://github.com/hud15/final-project-454.git
cd final-project-454
pip install -e .
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

## Reference

Pasion, L.R. (1999). Detecting unexploded ordnance with time domain electromagnetic induction [Master's dissertation, University of British Columbia]. University of British Columbia Geophysical Inversion Facility.

## License
[MIT](https://choosealicense.com/licenses/mit/)
