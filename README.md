# Hr_challenging_project

Files to download:

First Download "mask_rcnn_balloon.h5". Save it to the 'samples/balloon/' directory

Second Downlods "mask_rcnn.h5". Save it to the folder


## To detect the balloon in the image or videos using the provided weights
Apply splash effect on an image:

```bash
python3 balloon.py splash --weights=/path/to/mask_rcnn/mask_rcnn_balloon.h5 --image=<file name or URL>
```

Apply splash effect on a video. Requires OpenCV 3.2+:

```bash
python3 balloon.py splash --weights=/path/to/mask_rcnn/mask_rcnn_balloon.h5 --video=<file name or URL>
```

## Train the Balloon model

Train a new model starting from pre-trained COCO weights
```
python3 balloon.py train --dataset=/path/to/balloon/dataset --weights=coco
```

## Run Jupyter notebooks
Open the `inspect_balloon_data.ipynb` or `inspect_balloon_model.ipynb` Jupter notebooks. You can use these notebooks to explore the dataset and run through the detection pipelie step by step.
