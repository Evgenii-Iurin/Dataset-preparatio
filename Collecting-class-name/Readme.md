<div align="center">
<h1>Collecting class name</h1>
Evgenii Iurin
</div><br>
<div>
This code was written to collect all possible categories that are used in the dataset.
</div> <br>

## Introduction
Sometimes developers do not indicate the exact names of categories in the documentation, for example, in the official BDD100K documentation, classes such as ```pedestrian``` and ```bicycle``` are indicated, however, to define these objects, the names ```person``` and ```bicycle``` are used, respectively.

## Output
The algorithm creates a txt file containing all the classes that are used in the dataset. For example, the classes below were collected from BDD100K database.

```txt
1: traffic light
2: traffic sign
3: car
4: drivable area
5: lane
6: person
7: bus
8: truck
9: rider
10: bike
11: motor
12: train
```

## Application

From unique array traversal, an algorithm was realized to find class names only for a given JSON structure (BDD100K) or similar. Below is an annotation proposed by BDD100K. For my workload I wrote this algorithm for this dataset.

<table>
<tr>
<th>JSON entry</th>
<th>JSON structure</th>
</tr>
<tr>
<td>
  
```json
  [{ 
        "name": "image_name",
        "attributes": {},
        "timestamp": number,
        "labels": [{"category": "class_name",
                    "attributes":{},
                    "manualShape": True,
                    "manualAttributes": True,
                    "box2d": {}, 
                    "id": number}] 
  }]
```
  
</td>
<td>

```py
  test

```

</td>
</tr>
</table>

