# 02456-DeepLearning-Segmentality
Segmentation of Car Parts for Deloitte

The *main_pipeline.ipynb* notebook is showing the result from the last run.

If recreating the result is desired, the raw data has to be uploaded to Google Drive and the path has to be specified in the notebook.

The suggested folder structure would be the following, for the repsective classes of images:
```
└──test_data
    └──00.npy
    └──...
└──train_data
    └──cyclegan
    └──door
    └──opel
    └──primary
        └──31.npy
        └──...
```

## Network performance

Modify network, encoder in the *main_pipeline* for reproduction of results.

| Network    | Backbone   | DICE Score |
|------------|------------|------------|
| DeepLabV3+ | ResNet-34  | 65         |
| DeepLabV3+ | ResNet-101 | 70         |
| U-Net++    | ResNet-34  | 77.3       |
| U-Net++    | ResNet-101 | 71.3       |
