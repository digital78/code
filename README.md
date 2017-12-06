# code
-helper_functions.py: contains a set of common functions that are imported other python programs.

#-----------------------------------------#
-n-gen-bcf.py: generates negative binary cubic forms. This is not a parrallelized implementation and requires significant memory. For example, Y=100B takes about 80% of 256G RAM and about 200 minutes on a 64 CPU machine (m4.16xlarge).
Usage: ./n-gen-bcf.py <Y>


#-----------------------------------------#
-p-gen-bcf.py: generates positive binary cubic forms. This is a parallelized implementation that can use multiple cores. Multiple files are generated and then concatenated for the final result.
Usage: ./p-gen-bcf <Y> <processors> <TEMP_FOLDER>
