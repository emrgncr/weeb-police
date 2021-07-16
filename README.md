# weeb-police
A tensorflow keras model that decides if a profile picture is anime or not. 

It also includes the training data.

I downloaded a bunch of random steam profile pictures from https://randomavatar.com/ (I think the website no longer works but there are similar websites) and then labeled the imges as "anime" and "non-anime" by hand. I also checked for duplicates and deleted them but I did not check for similarity and just detected the exact same images so I could not detect if there are slightly differently cropped images.

The training data has 3.035 anime labeled images and 18.650 non-anime labeled images. All the images are 92x92 pixels and most of them are RGB (some are BW).

Because these images are random steam profile pictures, some of them may be NSFW so be careful about that.

I also trained a tensorflow keras model with this data. The model is included in the repo.
The model is not perfect, while I was training it tensorflow said it had around 95% validition accuracy but after a bit of experimenting I would say it is closer to ~80%.
