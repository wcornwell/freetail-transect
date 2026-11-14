# CLAUDE.md

## Where this repo sits — read before building anything new

**One library, two backbones.** `reallybig` is backbone-agnostic labeled audio living
outside every repo (OneDrive `call_library/`). Only the *embedding caches* and *venvs*
fork per backbone — the library itself never does. This repo touches none of that.

**This repo owns:** the published White-striped Free-tailed Bat map
(<https://willcornwell.org/freetail-transect/>) — one self-contained `index.html`.
**It does NOT own:** the page's content. `index.html` is **generated** by
`a2o-bats/figures/build_map.py`; the detector, the classifier and the analysis all live in
`a2o-bats`. Do not hand-edit `index.html` here — change the generator, re-export, and
commit the result.

Full ownership table, seams, venvs, shared data: **`~/Documents/ecoacoustics/ECOACOUSTICS.md`**. Check it
before writing a downloader, clip-mover, plot, or metric — it exists to stop double-builds.
