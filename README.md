# multiview-stitcher tutorial

This repo accompanies the **multiview-stitcher** tutorial during [Virtual I2K 2024](https://www.i2kconference.org/workshops).

## Links:
- multiview-stitcher [repo](https://github.com/multiview-stitcher/multiview-stitcher) and [docs](multiview-stitcher.github.io/multiview-stitcher/)
- napari-stitcher [repo](https://github.com/multiview-stitcher/napari-stitcher) and [docs](https://multiview-stitcher.github.io/napari-stitcher/)

## Workshop outline

- Intro slides (available [here](./20241030_intro_slides.pdf))

- Use with a GUI: napari-stitcher
	- 2D dataset (download [here](https://preibischlab.mdc-berlin.de/BigStitcher/Grid_2d.zip))
        - Prealign tiles using
            - napari built-in tools
            - napari-stitcher grid arrangement widget
	- 3D dataset (download [here](https://preibischlab.mdc-berlin.de/BigStitcher/Grid_3d.zip))
		- Prealign tiles using [napari-threedee](https://github.com/napari-threedee/napari-threedee)
	- Loading a tiled CZI file (download [here](https://github.com/multiview-stitcher/multiview-stitcher/raw/refs/heads/main/src/multiview_stitcher/test-datasets/mosaic_test.czi))

- Code example (notebook [in this repo](./example_stitching_workflow_3D.ipynb)):
    - Loading data into memory and lazily (dataset [here](https://preibischlab.mdc-berlin.de/BigStitcher/Grid_3d.zip))
    - Registration: translation and affine
    - Fusion: linear blending and max intensity projection
    - Visualizing results

## Installation

Preferably, create a new conda environment:

- `conda create -n multiview-stitcher python=3.10`
- `conda activate multiview-stitcher`

Then, you can use pip to install the following packages:

- `pip install napari-stitcher`
- `pip install napari-threedee` (optional)
- `pip install multiview-stitcher`


## Questions after the workshop?

Feel free to
- open an issue in the two repos above
- post with a `multiview-stitcher` tag on
  - forum.image.sc
  - imagesc.zulipchat.com
- contact me:
  - PM Marvin Albert on imagesc.zulipchat.com
  - marvin.albert@pasteur.fr


## Data acknowledgements

- Demo CZI mosaic dataset: thanks to Arthur Michaut @ Institut Pasteur
- BigStitcher 2D and 3D example datasets (License: GNU v2): thanks for making these available!
