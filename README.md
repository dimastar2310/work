# Image cutting 

Using 2 Detectron predictors 
first one for instance detection (object)
second one we dont have sky in the data set so we use 
panoptic dection to determine the sky 
sky category is 40 
it has data in json that determine the area 
Using for 1 image but the prenciple is the same 

splitting the image into 3 parts RGB
determining what category in instanse info pegmentation model data
the name of the category in MetadataCatalog.get(cfg.DATASETS.TRAIN[0]) in stuff category ,only for coco 
working with 3 r g b pictures in paralel (area times) painting pixels white ,wich determine pixels (third argument is chanel)
concatinating the picture and displaying it.

this models only understand coco format
![alt text](https://github.com/dimastar2310/work/blob/main/out(1).png)
