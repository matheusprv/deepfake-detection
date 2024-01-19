Subclipls Videos with Extracted Faces:

The preprocessing involves a series of steps. Initially, each video within a designated folder undergoes frame extraction. Subsequently, utilizing Retina Face, the software identifies and extracts faces from these frames, storing them separately. Finally, a compilation of these identified faces creates a new video file.


Decreasing Video Sizes:
Originally, the dataset specified fake videos to contain 25 frames and real ones to comprise 150 frames. However, some fake videos deviated, ending up with 24 frames. To rectify this discrepancy, a decision was made to standardize all fake videos to 24 frames and real videos to 144 frames, achieving dataset balance.

Challenges arose when attempting to train the model with varying video sizes. To overcome this obstacle, a solution emerged: breaking down real videos into 6 distinct clips, each containing 24 frames. This modification now enables seamless training processes.

Prepare dataset:
Before training, it is necessary to split de data into train, validation and test, and it was made using a proportion of 75/15/10, respectivly