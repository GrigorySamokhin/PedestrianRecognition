## Approach

- Find a training dataset
- Define model architechture 
- Train weights
- Compare to becnhmark

### Find a training dataset
A dataset was selected for this project: [www.vision.caltech.edu](http://www.vision.caltech.edu/Image_Datasets/CaltechPedestrians/)
or CityPersons [www.bitbucket.org](https://bitbucket.org/shanshanzhang/citypersons/src/default/)

The Caltech Pedestrian Dataset consists of approximately 10 hours of 640x480 30Hz video taken from a vehicle driving through regular traffic in an urban environment. About 250,000 frames (in 137 approximately minute long segments) with a total of 350,000 bounding boxes and 2300 unique pedestrians were annotated. 


### define model 

You need to analyze the set of approaches compared to benchmark models.

# Benchmarking 

### Benchmarking of pre-trained models on pedestrian detection datasets (autonomous driving)
|    Detector                | Dataset   | Backbone| Reasonable  | Heavy    | 
|--------------------|:--------:|:--------:|:--------:|:--------:|
| [Cascade Mask R-CNN](https://drive.google.com/open?id=1B487ljaU9FxTSFaLoirOSqadZ-39QEH8) | CityPersons        | HRNet | 7.5        |   28.0      | 
| [Cascade Mask R-CNN](https://drive.google.com/open?id=1ysWlzN92EInIjDD_QwIq3iQEZJDo8wtT) | CityPersons        | MobileNet | 10.2        |   37.3      | 
| [Faster R-CNN](https://drive.google.com/open?id=1aanqAEFBc_KGU8oCFCji-wqmLmqTd749) | CityPersons        | HRNet | 10.2        |   36.2      |
| [RetinaNet](https://drive.google.com/open?id=1MGxZitqLzQtd2EF8cVGYNzSKt73s9RYY) | CityPersons        | ResNeXt | 14.6        |   39.5      |
| [RetinaNet with Guided Anchoring](https://drive.google.com/open?id=1eBxkjhl12ELlv7VFyH9jS2O4I3SO_t8V) | CityPersons        | ResNeXt | 11.7        |   41.5      |
| [Hybrid Task Cascade (HTC)](https://drive.google.com/open?id=1qPEJ1r48Ggl2TdE1ohcDoprZomC2j3SX) | CityPersons        | ResNeXt | 9.5       |   35.8      | 
| [MGAN](https://drive.google.com/open?id=1c191nSSRUGd0LfkjYXKcyJEZCtjUeWr-) | CityPersons        | VGG | 11.2       |   52.5      | 
| [Cascade Mask R-CNN](https://drive.google.com/open?id=1HkoUPlONSF04AKsPkde4gmDLMBf_vrnv) | Caltech        | HRNet |   1.7      |    25.7     | 
| [Cascade Mask R-CNN](https://drive.google.com/open?id=1GzB3O1JxPN5EusJSyl7rl9h0sQAVKf15) | EuroCity Persons | HRNet |    4.4     |  21.3       |
| [Faster R-CNN](https://drive.google.com/open?id=19xBNw_wJPGNFIYsylcxPGIuoDygxHa2D) | EuroCity Persons        | HRNet | 6.1        |   27.0      |
 
 
### Benchmarking of pre-trained models on general human/person detection datasets
 
 |    Detector                | Dataset   | Backbone| AP  |
 |--------------------|:--------:|:--------:|:--------:|
 |    [Cascade Mask R-CNN](https://drive.google.com/open?id=1MqI1-Bbn0vl5Ft1RnhD70YWl7JHRyVMx) | CrowdHuman   | HRNet| 84.1  |

### Pre-Trained models
Cascade Mask R-CNN
1) [CityPersons](https://drive.google.com/open?id=1B487ljaU9FxTSFaLoirOSqadZ-39QEH8)
2) [Caltech](https://drive.google.com/open?id=1HkoUPlONSF04AKsPkde4gmDLMBf_vrnv)
3) [EuroCity Persons](https://drive.google.com/open?id=1GzB3O1JxPN5EusJSyl7rl9h0sQAVKf15)
4) [CrowdHuman 1](https://drive.google.com/open?id=1rXopG04Dv-HKge3ZyqNYAHdCi9gmLuNe)
5) [CrowdHuman 2](https://drive.google.com/open?id=1MqI1-Bbn0vl5Ft1RnhD70YWl7JHRyVMx) (higher AP)
6) [WIDER Pedestrian](https://drive.google.com/open?id=1Z1LTASbr-VTIfbk4Fu-d2VCBpKPqADH8)

Faster R-CNN
1) [CityPersons](https://drive.google.com/open?id=1aanqAEFBc_KGU8oCFCji-wqmLmqTd749)
2) [EuroCity Persons](https://drive.google.com/open?id=19xBNw_wJPGNFIYsylcxPGIuoDygxHa2D)

RetinaNet
1) [CityPersons](https://drive.google.com/open?id=1MGxZitqLzQtd2EF8cVGYNzSKt73s9RYY)

RetinaNet with Guided Anchoring
1) [CityPerson](https://drive.google.com/open?id=1eBxkjhl12ELlv7VFyH9jS2O4I3SO_t8V)


Hybrid Task Cascade (HTC)
1) [CityPersons](https://drive.google.com/open?id=1qPEJ1r48Ggl2TdE1ohcDoprZomC2j3SX)

MGAN
1) [CityPersons](https://drive.google.com/open?id=1c191nSSRUGd0LfkjYXKcyJEZCtjUeWr-)

# Getting Started
