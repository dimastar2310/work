# Image cutting 
Note if you using GPU you can # in the model Iam using CPU for free version.
Using 2 Detectron predictors 
first one for instance detection (object)
second one we dont have sky in the data set so we use 
panoptic dection to determine the sky 
sky category is 40 
it has data in json that determine the area 
Note Using for 1 image but the prenciple is the same
you can put in !wget https://farm5.staticflickr.com/4147/5087832865_a8a388de44_z.jpg -q -O input.jpg ,
w/e picture you want from COCO data set replace url untill -q please, flicker one and it will work.

Splitting the image into 3 parts RGB
determining what category in instanse info pegmentation model data
the name of the category in MetadataCatalog.get(cfg.DATASETS.TRAIN[0]) in stuff category ,only for coco 
working with 3 r g b pictures in paralel (area times) painting pixels white ,wich determine pixels (third argument is chanel)
concatinating the picture and displaying it.

This models only understand coco format

Thanks the most to this articles

#https://kharshit.github.io/blog/2019/10/18/introduction-to-panoptic-segmentation-tutorial
#https://www.youtube.com/watch?v=eUSgtfK4ivk
#https://www.youtube.com/watch?v=h6s61a_pqfM&t=620s
#https://stackoverflow.com/questions/7589012/combining-two-images-with-opencv



![alt text](https://github.com/dimastar2310/work/blob/main/out(1).png)


