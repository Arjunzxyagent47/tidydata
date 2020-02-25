This repo contains :
1.CodeBook.txt which describes the dataset.
2.README.txt (The file you are now reading)
3.run_analysis.R which was used to create tidydata.txt
4.tidydata.txt which is a modified dataset from UCI HAR


Analysis:
Steps taken to convert UCI HAR (Human Activity Recognition Dataset:

1.First, download and unzip "http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones" 
  into your R working directory.
2.Open the UCI HAR folder, read the README file and also observe the other files.Inference:The variables in the data X
  are sensor signals measured with waist-mounted smartphone from 30 subjects.The variable in the data Y indicates 
  activity type the subjects performed during recording.
3.Create the Rscript run_analysis.R. 
4.Combine training dataset and test dataset.Extract the measurements on the mean and standard deviation for each 
  measurement.(use rbind() ,grep() to get column indexes for variable name contains "mean()" or "std()")
5.Label the data.
6.From the data set , create a second, independent tidy data set with the average of each variable for each activity
  and each subject. 