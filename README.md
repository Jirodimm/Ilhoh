# Ilhoh

Open data behind the Ilhoh maps. The map that uses these files is at
[ilhoh-map.vercel.app](https://ilhoh-map.vercel.app).

## Köppen-Geiger climate polygons, 1991–2020

| File | Format | Detail |
|---|---|---|
| `koppenge_10m_2020_100.geojson` | GeoJSON | full |
| `koppenge_10m_2020 _topo_100.json` | TopoJSON | full |
| `koppenge_10m_2020_66.json` | GeoJSON | simplified further |
| `koppenge_10m_2020_topo_66.json` | TopoJSON | simplified further |

Each file holds 30 features, one multipolygon per Köppen-Geiger class, in
WGS 84 longitude and latitude. The `DN` property is the class code used by
Beck et al. (2023), from 1 (Af) to 30 (EF).

**Source.** Beck, H. E., McVicar, T. R., Vergopolan, N., Berg, A.,
Lutsko, N. J., Dufour, A., Zeng, Z., Jiang, X., van Dijk, A. I. J. M., &
Miralles, D. G. (2023). High-resolution (1 km) Köppen-Geiger maps for
1901–2099 based on constrained CMIP6 projections. *Scientific Data*, 10,
724. [doi:10.1038/s41597-023-02549-6](https://doi.org/10.1038/s41597-023-02549-6).
Data on Figshare, [doi:10.6084/m9.figshare.21789074.v2](https://doi.org/10.6084/m9.figshare.21789074.v2),
under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

**Changes from the source.** Generalised from the 1 km map for 1991–2020
for use in web maps: resampled to a coarser grid, converted to polygons,
with small patches merged into a neighbouring class, simplified, dissolved
to one multipolygon per class, and coordinates rounded to 0.1°. The "66"
files are a further simplified copy. These files are not a substitute for
the source in analysis. A script that rebuilds them from the source will
come with the first versioned release.

## How to cite

> Marques Macedo, D. (2026). *Ilhoh: generalised Köppen-Geiger climate
> polygons, 1991–2020* [Data set]. https://github.com/Jirodimm/Ilhoh

Please cite Beck et al. (2023) as well. GitHub's "Cite this repository"
button gives the same reference in APA and BibTeX, from
[`CITATION.cff`](CITATION.cff). Versioned releases will be archived on
Zenodo with a DOI, which will then replace the link above.

Author: Diogo Marques Macedo,
[ORCID 0009-0008-6977-7180](https://orcid.org/0009-0008-6977-7180).

## Licence

The data is under the [Creative Commons Attribution 4.0 International
licence](LICENSE) (CC BY 4.0), the licence of its source.
