## Petals to the Metal: Flower Classification on TPU       
**Dataset Link** : https://www.kaggle.com/c/tpu-getting-started        
**Personal Notebook Link** : https://www.kaggle.com/stephenyang0215/petals-to-the-metals            
**Description**: In this Getting Started competition (what is a Getting Started competition?), we're classifying 104 types of flowers based on their images drawn from five different public datasets. Some classes are very narrow, containing only a particular sub-type of flower (e.g. pink primroses) while other classes contain many sub-types (e.g. wild roses).

The dataset contains imperfections - images of flowers in odd places, or as a backdrop to modern machinery - but that's part of the challenge! Build a classifier than can see past all that, to the flowers at the heart of the images.

**Files**: This competition provides its files in TFRecord format. The TFRecord format is a container format frequently used in Tensorflow to group and shard data data files for optimal training performace. Each file contains the id, label (the class of the sample, for training data) and img (the actual pixels in array form) information for many images. Please see our Getting Started notebook or our Learn exercise for notes on how to load and use them! Additional information is available in the TPU documentation.

train/*.tfrec - training samples, including labels.   
val/*.tfrec - pre-split training samples w/ labels intended to help with checking your model's performance on TPU. The split was stratified across labels.    
test/*.tfrec - samples without labels - you'll be predicting what classes of flowers these fall into.    
sample_submission.csv - a sample submission file in the correct format.  
   
- id
- label (in training data) the class of flower represented by the sample.    
