# legacy/

Original notebooks of this repo (2023–2024), kept untouched with their outputs. They were replaced by the notebooks in [`notebooks/`](../notebooks/).

| File | What it was | Replaced by |
|---|---|---|
| `raster.ipynb` | World map of Global Map Percent Tree Cover. Does not run with matplotlib ≥ 3.9 (`cm.get_cmap` was removed) and expects a local `data/` folder. | [`01_world_forests.ipynb`](../notebooks/01_world_forests.ipynb) |
| `load_satellite_data.ipynb` | Sentinel-2 L2A via STAC + odc-stac over Antalya, red/green/blue bands plotted separately. Still runs, but picks the first scene without a cloud filter (81 % clouds). | [`02_sentinel2_stac.ipynb`](../notebooks/02_sentinel2_stac.ipynb) |
| `data/raster_forest.png` | The world forests figure saved by `raster.ipynb`. | `docs/img/world_forests.png` |

The 87 MB `gm_ve_v1.tif` that used to live in `Notebook/data/` is no longer in the tree: the new notebook downloads it at run time.
