# CDV - Causal Discovery In Video

Objective: Identify (granger) causal relationships between objects/subjects in videos

## Phase 1: Select a object-detection video dataset in which multiple objects/subjects interact, preferably in ways which include object obstruction
- Example Dataset: SportsMOT dataset (https://paperswithcode.com/dataset/sportsmot). Other resources may be found at, for example, https://www.twine.net/blog/top-object-recognition-video-datasets/ .
- Note: Students will likely need to create an augmented version of this dataset in Phase 2 to ensure object obstruction is appropriately handled

## Phase 2: Implement 2 Video-based object detection algorithms that handle missing (esp. obstructed) data. 
These algorithms will need to create a bounding box for each object and assign a unique identifier to each box.

## Phase 3: Implement 1-2 Granger causal estimation algorithms for discovering Granger causal relationships using box-center time-series extracted from videos.
- Example algorithm: cMLP / cLSTM (see https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9376668 and code at
https://github.com/iancovert/Neural-GC )
- Students will need to adapt trained algorithms from Phase 2 to extract box-center time series from real data
- Example time series (toy) datasets for causal discovery: Synthetic (lorenz model), DREAM4 insilico network data (see
https://www.synapse.org/#!Synapse:syn3049712/wiki/74630 )

## Other Notes:
- Analysis Technique(s): MSE for both networks (video object detection and causal graphs)
