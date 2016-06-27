# Pupil "Research" Plugin Suite
Plugin suite for running custom Python scripts interacting with [Pupil](https://github.com/pupil-labs/pupil).

- `psychopy_pupil_utils` is a set of PsychoPy classes which are used to visualize calibration and surface markers. The calibration markers are drawn using multiple Circle objects on top of each other. The surface markers use pre-rendered images generated by [`make_square_markers.py`](https://github.com/pupil-labs/pupil-helpers/blob/master/make_square_markers.py).

- `pupil_interface` is a Python module which uses `Pupil Sync` to remote control `Pupil` software.

**Note:** Pupil [v0.8](https://github.com/pupil-labs/pupil/releases/tag/v0.8) introduces a new communication pattern (see [IPC Backbone](https://github.com/pupil-labs/pupil/wiki/Pupil-Interprocess-and-Network-Communication)). `Pupil Interface` is being rewritten to work with the IPC Backbone. A stable version without time synchronization can be found in the branch [`ipc-version`](https://github.com/papr/Pupil-Research-Plugin-Suite/tree/ipc-version). It will be merge into `master` as soon time sync is implemented.