# CS-567-Assignment-4-solution

Download Here: [CS 567 Assignment #4 solution](https://jarviscodinghub.com/assignment/cs-567-assignment-4-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

(1) (5 points) For this problem you’ll be building off of the region growing problem we worked on in
class, based on Practical Lesson 6.8.3. Recall when we ran the algorithm in class we binarized the
image and initialized where the growing began and so only the one region was identified. Please do
work off the class code and not the author’s since I wrote a more efficient version of the script that
should grow the region much faster and I simplified the algorithm to work with binary images. The
goal here is to skip the initialization step (selecting a pixel in the segment of interest) and then use
this flexibility to allow us to find all connected segments in our binary image. Your result should
produce an image where each connected region of pixels is indicated by an integer and should look
like Figure 1, where each color represents a different segment for a total of 5 segments (your colors
may differ). To achieve this you will need to embed the while loop from class into a for loop that
will loop through the pixels and if a pixel in the image has an intensity of 1 and hasn’t yet be
assigned to a segment, that pixel serves as the initial pixel of a new segment. Tip: If you want
your loop to go really fast, have it skip rows of pixels where the original image is all 0s or where
the nonzero pixels have already been assigned to a segment. My version took fewer than 4s to run
and I’m sure that time could be beat!
Figure 1: The solution you are working toward for problem 1. Each color represents a different
segment (dark blue is background).
(2) (10 points) This goal of this problem is to check that you’re making progress on the final project
and that you’re able to write code that I (and the TA) can easily execute. Generate code that
extracts 1 feature from each of the distributed retina images. Recall, this is a single, numeric, value
1
that summarizes something about each image. Write this code so it will estimate these features from
the left out data set as well as the distributed data set. Please see the Final Project instructions
for more details. In short, I should be able to change 2 paths in your code to the 2 sets of data
(one I distributed and held out data). I will then run your code directly from the command line
(akin to using the run command). Some of you may have written extra functions, so it is fine if I
also need to change an addpath command. Just zip up all your MATLAB functions. This portion
of the homework will not use the mlx/pdf option. You will submit MATLAB script(s) only. You
will be graded on:
• Whether your code executes without errors.
• Whether your code is efficient. It should be able to compute the features on all images within
a minute or two, tops.
• I will not grade you on the quality of your features, but I will give you feedback if I think you
are not on the right track. The only output from the code should be any notes you include
to verify the code is running (I often like it to print out the image it is currently working on
so I can notice if it gets stuck) and a scatter plot of the feature magnitude on the y-axis and
the image number on the x-axis (one for the distributed data and the held out data). For
the distributed data I ordered all of the healthy retinas first, so this will be an easy check to
see if your feature has any potential. You should be able to see a noticeable difference in the
feature magnitude for the first 18 vs second 18 values.
