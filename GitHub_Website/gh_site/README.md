# Gravity-adaptive gait control for a bipedal robot

Bachelor thesis project by Nikesh Gahatraj (ID 2317390), Smart Computing, Kyungdong University Global. Supervisor: Dr. Nyrod Villa.

**Website:** open `index.html` through GitHub Pages (see below). It replays the recorded results of the simulation for Earth, Moon and Mars, and shows the physical robot from the previous semester.

## Folders

| Folder | Content |
|---|---|
| `index.html`, `assets/` | The website (replay viewer, photos, video) |
| `simulation/` | The Python / PyBullet simulation (`simulate.py`, `run_all.py`, `tune_gait.py`, `biped.urdf`, tuned parameters, Colab notebook) |
| `data/` | CSV results used by the website and the thesis |

## Run the simulation yourself

```
cd simulation
pip install -r requirements.txt
python simulate.py --gravity Moon --controller Adaptive --gait tuned --gui
```

Or open `simulation/Run_in_Colab.ipynb` in Google Colab.

## Limits

The website replays saved results; it does not run the physics engine in the browser. Nothing was measured on the real robot, which did not walk. Leg angles in the viewer are rebuilt from the gait equations and drawn as a schematic.
