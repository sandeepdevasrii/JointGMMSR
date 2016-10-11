This archive contains the MATLAB codes corresponding to the paper
[1] Palakkattillam Sandeep and Tony Jacob, "Single Image Super Resolution
    using a Joint GMM Method", IEEE Transactions on Image Processing,
    Issue 9, September 2016.

Directory x2 contains the source codes for super resolution by 
a factor 2 (q = 2), and, Directory x3 contains the source codes for
q = 3.

To reproduce the SR results reported in [1], change the directory to
x2 (for q=2) or x3 (for q=3) and run the script "SRWrapper.m".
In both the cases (x2 and x3), Ground truth HR and the corresponding LR
images are stored in a directory named "Data". If you wish to run
the SR experiments on your own images, either copy your images to this
directory, or use your own directories for HR and LR images, and,
accordingly change Line No. 6 and 7 of the script "SRWrapper.m"

GMM Parameters trained by using our training database are stored in
the directory "Params" as can be seen in both the directories x2 and x3.
Due to the large file size, our training database is not included in
this archive. If you want the training database, write a mail to
p.sandeep@iitg.ernet.in

To train your own GMM, prepare two directories containing the ground
truth HR and the corresponding LR images respectively, and, edit
Line No.14 and 15 of the script "TrainGMM.m" to point to these
directories.
