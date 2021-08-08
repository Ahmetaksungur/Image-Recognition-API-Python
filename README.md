# Image Recognition API - Python
#### Python image recognition libraries process the image sent with the api and look at the object, classification, intense colors of the image and whether the image is safe or not.
 
Files you need to upload to the home path after downloading the home folder

https://github.com/OlafenwaMoses/ImageAI/releases/download/essentials-v5/resnet50_imagenet_tf.2.0.h5
https://github.com/OlafenwaMoses/ImageAI/releases/download/1.0/yolo.h5
 
 
#### /api [POST]
```json
{
	"image": "https://github.com/OlafenwaMoses/ImageAI/blob/master/test-images/11.jpg?raw=true"
}
```
#### /api Return
 
```json
{
  "width": 800,
  "height": 534,
  "security": {
    "nsfw": "0.00035329186",
    "sfw": "0.99964666"
  },
  "color_palette": [
    {
      "color": "#ECECEB",
      "score": 0.56
    },
    {
      "color": "#7F7A7D",
      "score": 0.12
    },
    {
      "color": "#C3917D",
      "score": 0.11
    },
    {
      "color": "#312B29",
      "score": 0.09
    },
    {
      "color": "#CCB698",
      "score": 0.05
    },
    {
      "color": "#8E6345",
      "score": 0.03
    },
    {
      "color": "#704433",
      "score": 0.02
    },
    {
      "color": "#494D5D",
      "score": 0.01
    }
  ],
  "classification": [
    {
      "label": "jean",
      "score": 14.029912650585175
    },
    {
      "label": "notebook",
      "score": 11.251913011074066
    },
    {
      "label": "stretcher",
      "score": 8.27689915895462
    },
    {
      "label": "monitor",
      "score": 8.269056677818298
    },
    {
      "label": "lab_coat",
      "score": 6.923883408308029
    }
  ],
  "objectDetection": [
    {
      "label": "person",
      "score": 99.90594983100891
    },
    {
      "label": "person",
      "score": 99.98345375061035
    },
    {
      "label": "person",
      "score": 99.86221194267273
    },
    {
      "label": "person",
      "score": 99.63626861572266
    },
    {
      "label": "laptop",
      "score": 99.60939884185791
    },
    {
      "label": "dining table",
      "score": 41.51776731014252
    },
    {
      "label": "person",
      "score": 98.27415943145752
    },
    {
      "label": "cup",
      "score": 99.72758293151855
    },
    {
      "label": "cup",
      "score": 98.5138475894928
    },
    {
      "label": "cup",
      "score": 88.39868307113647
    },
    {
      "label": "cell phone",
      "score": 53.04287672042847
    },
    {
      "label": "keyboard",
      "score": 31.74397349357605
    },
    {
      "label": "cell phone",
      "score": 79.6405017375946
    },
    {
      "label": "cup",
      "score": 98.25559854507446
    }
  ]
}
```
