# Data Analysis Tools for *Hydra* Videos

- [Data Analysis Tools for *Hydra* Videos](#data-analysis-tools-for-hydra-videos)
  - [Find Midline](#find-midline)
  - [Trace Fluorescence](#trace-fluorescence)

## Find Midline

Track the midline of *hydra* based on the contours data from [ICY](http://icy.bioimageanalysis.org/) and coordinates of some tracked points from [DeepLabCut](https://github.com/AlexEMG/DeepLabCut). Measure the length of the midline for each frame and save it as a csv file. 

- Clone this repo
- Enter the directory find_midline/
- Run `python midline.py path/of/icy/file path/of/deeplabcut/file max_of_depth`

where the file from ICY should be .xml file, the file from DeepLabCut should be .csv file. 

**Note:** The tracked parts of Hydra must be in the order of *hypostome, armpit1, armpit2 and peduncle*

## Trace Fluorescence

Integrate the fluorescence in each frame of a video and plot the trace. 

- Clone the repo
- Enter the directory trace_fluorescence
- Run `python trace_fluo.py path/of/video/file`