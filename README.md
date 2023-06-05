# Pianum

```bash
pip install git+https://github.com/chemtrails/pianum
```

```py
import pianum as pn
from pianum.struct import Interval, Scale, Chord

root = 3

interval = pn.interval(root, Interval.M3)
print(interval)

scale = pn.scale(root, Scale.major)
print(scale)

chord = pn.chord(root, Chord.major7)
print(chord)

inversion = pn.invert_up(chord)
print(inversion)

notes = pn.ints_to_notes(inversion)
print(notes)
```

```bash
[3, 7]
[3, 5, 7, 8, 10, 12, 14]
[3, 7, 10, 14]
[7, 10, 14, 15]
['E', 'G', 'B', 'C']
```
