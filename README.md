# 22zooniverse

This repository contains the data that we use for the analysis of chimpanzee annotation task.
Below explains the columns in these csv files.

- **crowd\_individual.csv**, the data collected in the crowdsourcing task (see the screenshot of the task)
  - _acc_acrossUser_: in the format of [x,y,z] where _x_ represents how many questions are correctly answered, _y_ represents how many questions are correct after merging "No" and "HardToSay" as "No", and _z_ represents the total number of answered questions
  - _difficult\_x_: the value indicating the perceived difficulty entered by each crowd worker for question _x_
  - _voteHard\_x_: whether the crowd worker selected "HardToSay" in question _x_

- **google-x.csv**, the pairwise similarity of the videos in the task by using _x_ as the metric, for which we considered FSIM, PSNR, RMSE, SRE, and SSIM
  - _n1, n2, n3_: 3 negative example videos (in the training materials)
  - _y1, y2, y3_: 3 positive example videos (in the training materials)
  - _t1, t2, t3, t4, t5, t6_: 6 test videos

&nbsp;&nbsp;&nbsp;&nbsp;> The name of the column indicates the pair of videos for which the similarity score is calculated. For example, _n1\_y2_ means the similarity between _n1_ and _y2_.

- **ground\_truth.csv**, the groundturth labels for the 6 test videos in each task.

