# COMP3850-PACE-Group-67
PACE computing industry project

Step 1:
For the first steps, We have tweaked the code so that instead of using the given embeddings(shadow_test and shadow_train),
we split the shadow.csv into train and test files for each shadow model. 
This is required to gain multiple shadow models instead of just one.

Step 2-3: 
The embedding generation now consists of a for loop to generate "k" shadow models.
k also decides the random seed to make each split different, resulting in different shadow models.
Each shadow model is saved as their own npy files.

Now I have create a variable named shadowData which is an array to hold
all data concerning each individual shadow model.
This makes it easy now to for loop all the sections of code by refering
to this one variable with all the shadow model data. 
This will be applied to all the additional steps. 
