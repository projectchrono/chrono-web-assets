# Assets of the "DEM Validation" documentation page

The folder `dem_validation` next to this file holds the images and clips of the page, to be uploaded through the
chrono-web-assets repository. This file is not part of the upload. Each asset is a byte copy of a delivered file in
`element_tests\out`, whose note (`out\<note>`) gives how the runs behind it were set up.

| Asset | Source in `out` | Note | Page section |
|---|---|---|---|
| `dem_shear_jenike_curves.png` | `ds_jenike_curves.png` | `ds_jenike_curves.md` | Direct shear, Jenike cell |
| `dem_shear_jenike_plateau.png` | `ds_rolling.png` | `ds_rolling.md` | Direct shear, Jenike cell |
| `dem_shear_jenike_porosity.png` | `ds_porosity.png` | `ds_porosity.md` | Direct shear, Jenike cell |
| `dem_shear_box_curves.png` | `ds_curves.png` | `ds_curves.md` | Direct shear, square box |
| `dem_shear_box_forcenet.mp4` | `ds_forcenet.mp4` | `ds_forcenet.md` | Direct shear, square box (clip) |
| `dem_shear_box_forcenet_poster.png` | `ds_forcenet_poster.png` | `ds_forcenet.md` | poster frame of the clip |
| `dem_shear_history_curves.png` | `ds_history_curves.png` | `ds_history_curves.md` | Direct shear, contact history |
| `dem_shear_history_networks.png` | `ds_history_networks.png` | `ds_history_networks.md` | Direct shear, contact history |
| `dem_triaxial_lab.png` | `tri_curves.png` | `tri_curves.md` | Triaxial, against the laboratory |
| `dem_triaxial_csl_pq.png` | `tri_csl_pq.png` | `tri_csl_pq.md` | Triaxial, critical state |
| `dem_triaxial_csl_lnp.png` | `tri_ncl_lnp.png` | `tri_ncl_lnp.md` | Triaxial, critical state |
| `dem_triaxial_density.png` | `tri_density.png` | `tri_density.md` | Triaxial, density |
| `dem_triaxial_history.png` | `tri_history.png` | `tri_history.md` | Triaxial, contact history |
| `dem_triaxial_rate.png` | `tri_speed.png` | `tri_speed.md` | Triaxial, loading rate |
| `dem_triaxial_forcenet.mp4` | `tri_forcenet.mp4` | `tri_forcenet.md` | Triaxial (clip) |
| `dem_triaxial_forcenet_poster.png` | `tri_forcenet_poster.png` | `tri_forcenet.md` | poster frame of the clip |

Images: PNG at 300 dpi, 1341 to 1980 px wide (the clip posters 1144 x 1080 and 648 x 1080), shown at 600 to 800 px
like the other manual pages. Clips: H.264 (High profile, yuv420p), 30 fps, 9.9 s, loopable, with the index at the
start of the file, so a browser can start playing before the download ends.

Doxygen (1.8.16 here) escapes a bare `<video>` tag into text, but passes it through inside `\htmlonly ...
\endhtmlonly`, so the page shows each clip as:

```
\htmlonly
<video controls loop muted playsinline preload="none" width="..." poster="<url of the poster>">
  <source src="<url of the clip>" type="video/mp4">
</video>
\endhtmlonly
```
