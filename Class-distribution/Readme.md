<div align="center">
<h1>Dataset class distribution</h1>
Evgenii Iurin
</div>

<br>
<div align="center">
This code was created to represent class distribution, namely how many images are used by each class.
</div>
<br>

## Introduction
Data analytics - is a powerful tool that helps to evaluate datasets and adjust the direction of your application. The distribution shows in a clear way how many images are used by each class. That serves as quick dataset evaluation. There is a code description and two plots for representation.

As a baseline, I take the Dataset BDD100K. 
## Output
As an output data algorithm returns two ```png``` files with two variants of distribution graphs. For example, there are two plots for training and validation data.

<table>
<tr>
<th>Training dataset distribution</th>
<th>Validation dataset distribution</th>
</tr>
<tr>
<td>
<img src="img/distribution_of_the_train_dataset.png" alt="train_variant_1"/>  
</td>

<td>
<img src="img/Distribution_of_the_val_dataset.png" alt="val_variant_1"/>  
</td>

<tr>
<td>
<img src="img/Distribution_of_the_train_dataset_1.png" alt="train_variant_2"/>
</td>

<td>
<img src="img/Distribution_of_the_val_dataset_1.png" alt="val_variant_2"/>
</td>

</tr>
</table>


## Execution algorithm
1. Gets a folder with prepared files (.txt and .jpg) in YOLO format at the given folder path.
2. Opens each .txt file
3. In YOLO format each first humber on each line represents a class, which we gave earlier.
4. There can be several classes on one image . In order to keep the correct statistics we must calculate non-repeating classes. A sort function was written for this.
5. At the next stage, the sorted array goes to the function that calculates the number of images for each class.
6. The cycle repeats.
