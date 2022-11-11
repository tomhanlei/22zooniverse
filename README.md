# 22zooniverse

This repository contains the data that we use for the analysis of chimpanzee annotation task.
Below explains the columns in these csv files.

- **crowd\_individual.csv**, the data collected in the crowdsourcing task (see the screenshot of the task)
  - _acc_acrossUser_: in the format of [x,y,z] where _x_ represents how many questions are correctly answered, _y_ represents how many questions are correct after merging "No" and "HardToSay" as "No", and _z_ represents the total number of answered questions
  - _difficult\_x_: the value indicating the perceived difficulty entered by each crowd worker for question _x_
  - _voteHard\_x_: whether the crowd worker selected "HardToSay" in question _x_

- **google-x.csv**, the pairwise similarity of the videos in the task by using _x_ as the metric, for which we considered FSIM, PSNR, RMSE, SRE, and SSIM

