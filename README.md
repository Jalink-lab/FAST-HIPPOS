# FAST-HIPPOS: FLIM Analysis of Single-cell Traces for Hit Identification of Phenotypes in Pooled Optical Screening
![image](https://github.com/user-attachments/assets/27e8f19d-a5f8-4cbf-94ee-4d4665a7af8f)

FAST-HIPPOS is a collection of Fiji scripts to analyze and visualize multi-cell time-lapse experiments, detect hit cells based on user-set criteria and output their stage coordinates for e.g. photoactivation.
For non-screening applications it can function as a valuable tool for single-cell trace analysis, visualization and inspection.

<hr>

For detailed information, please visit [https://imagej.net/plugins/fast-hippos](https://imagej.net/plugins/fast-hippos).

## Installation

Activate the **FAST-HIPPOS** update site in Fiji (*Help → Update… → Manage Update Sites*), together with the other
update sites listed on the [plugin page](https://imagej.net/plugins/fast-hippos). The commands appear under
*Plugins → Macros*.

## Files

| File | Purpose |
|---|---|
| `FAST-HIPPOS_.ijm` | main macro: segmentation, single-cell traces, visualization and hit selection |
| `Inspect_and_select_traces_.ijm` | interactive inspection of traces and manual selection of hits |
| `Stitch_tiles.ijm` | stitches multi-tile experiments and stores the stage coordinates in the stitched image |
| `Get_stage_coordinates_to_log_window.py` | helper for `Stitch_tiles.ijm`: reads the stage coordinates from a `.lif` file |
| `Get_plot_styles_to_log_window.groovy` | helper: prints the styles of the objects in the active plot |
| `Labkit_FAST_HIPPOS_nuclei_classifier.txt` | default Labkit classifier for refining hit positions on the nuclei |
| `Turbo.lut` | Turbo lookup table |

## Changelog

**v0.9.5**
- Improved the path of hit cells in the `.rgn` output files, and its visualization.

**v0.9.4**
- Hit positions can be refined on the nuclei with a Labkit classifier. A classifier is provided, but can be
  replaced by your own trained classifier.

**v0.9.3**
- Cells can be classified on the intensity of the additional channel, shown in the 'lifetime vs additional
  channel intensity' scatter plot.

**v0.9.2**
- First release.
