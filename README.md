# Data Splitter
A handy note-book to split data form samples and labels to test-train folders

<hr>
 Managing the way input data is stored can be tricky sometimes to easily load them into python intr for further processing, fo example if we consider famous Cats vs Dogs dataset for image processing, it is in images and labels format which requires some additional amount of work to load.
 
 Or suppose if you less RAM meomory and need to load part of a data set rather than complete dataset itself then, follow the above notebook to the same (may require slight tinkering to suit your needs) :)
 
 <hr>
 
<b>Initial dir structure</b> 

    \DATA
    ├───images
    └───labels
   
- images folder contains all samples
- labels contains mapping of images to labels (in our case it's in XML so ,we will parse it)

<b>To</b>

    \SAMPLES
    ├───1
    ├───2
    ├───3
    ├───4
    ├───5
    └───6
Now we will convert this into train,test and validation folder by using split-folders lib

<b> End Result </b>

        \SPLIT
        ├───train
        │   ├───1
        │   ├───2
        │   ├───3
        │   ├───4
        │   ├───5
        │   └───6
        └───val
            ├───1
            ├───2
            ├───3
            ├───4
            ├───5
            └───6
            
Now we can load this for ML stuff :)
