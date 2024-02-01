# :artificial_satellite: Augmented Convolutional Neural Networks for Remote Sensing Change Detection 

## :card_index_dividers: Code Repository for CS ECE 5824 - Advanced Machine Learning 

## :black_nib: Authors: [Canvas Group: Remote Sensing Change Detection]
1. Sarvesh Patil (sarveshpatil@vt.edu) 
2. Pranjal Ranjan (pranjalranjan@vt.edu)
3. Ankit Parekh (ankitparekh@vt.edu)
4. Badhrinarayan Malolan (badhrinarayan@vt.edu) 

## :open_file_folder: Repository Index

| **File** | **Description** | **Model** | **Challenge** |
|:---------------------------------:|:------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| [AML_Initial_Model_Selection.ipynb](AML_Initial_Model_Selection.ipynb) | Notebook for initial baselining and model selection | Unaugmented: EF, Siam-Conc. & Siam-Diff | Original Dataset |
| [AML_Unaugmented.ipynb](AML_Unaugmented.ipynb) | Notebook for training unaugmented networks for few-shot learning | Unaugmented: EF | Few-shot learning |
| [AML_Data_Augmentation.ipynb](AML_Data_Augmentation.ipynb) | Notebook for training augmented network with edge maps and MRA | Augmented: EF (Edge & MRA) | Original Dataset & Few-shot learning |
| [AML_Pretrain.ipynb](AML_Pretrain.ipynb) | Notebook for training augmented network with pretrained imagenet encoder | Augmneted: EF (Pretrained Encoder) | Original Dataset & Few-shot learning |
| [AML_Evaluation.ipynb](AML_Evaluation.ipynb) | Notebook for evaluating results for all phases | Unaugmented: EF, Siam-Conc. & Siam-Diff & Augmented models: EF (Edge, MRA & Pretrained) | Original Dataset, Few-shot learning, Noise Robustification & Dataset Shift |
| [Project_Report.pdf](Project_Report.pdf) | Report containing details about the datasets, implementation, experiments and results | --- | --- |
| README.md | Description file for the repository | --- | --- | 

## :white_check_mark: Instructions to run the notebooks:

### 1.	**For Phase I**: 

>> Run the cells inside the **_AML_Initial_Model_Selection.ipynb_** notebook sequentially to train and test the three Unaugmented networks (EF, Siam-Conc. & Siam-Diff.).

>>> Use the default values in the ```Dataset Downloader``` & ```Dataset Characteristics``` cells.

### 2.	**For Phase II**: 

>> Run the cells inside the **_AML_Data_Augmentation.ipynb_** notebook sequentially to train and test Edge-Augmented & MRA-Augmented networks.

>> Run the cells inside the **_AML_Pretrain.ipynb_** notebook sequentially to train and test Feature-Augmented networks.
 
>>> Use the default values in the ```Dataset Downloader``` & ```Dataset Characteristics``` cells.
>>> Use the default values in the ```Subset Choice``` cell.
 
### 3.	**For Phase III**:

 * Dataset Shift & Noise Robustness:

>> Run the first cell inside the **_AML_Evaluation.ipynb_** notebook with both the dataset choices (“LEVIRCD_Plus” & “WHU”) to download the primary and alternate dataset. 

>> Run the second cell inside the **_AML_Evaluation.ipynb_** notebook to import requisite libraries.

>> Scroll to the Phase III Dataset Shift & Noise Robustness results section of the notebook, and run the cells sequentially to reproduce the results. 

 * Few-shot Learning:
 
>> Run the cells inside the **_AML_Unaugmented.ipynb_** notebook sequentially to train and test few-shot learning for Unaugmented EF network.
 
>> Run the cells inside the **_AML_Data_Augmentation.ipynb_** notebook sequentially to train and test few-shot learning for Edge-Augmented & MRA-Augmented EF network.
 
>> Run the cells inside the **_AML_Pretrain.ipynb_** notebook sequentially to train and test few-shot learning for Feature-Augmented EF network.
 
>>> Use the default values in the ```Dataset Downloader``` & ```Dataset Characteristics``` cells.

>>> Select respective subset percentage values (25 & 50) in the ```Subset choice``` cell for the respective experiment.

## :star2: Qualitative Results

### Qualitative Result I

![Alt text](qualitative_result_I_A.png?raw=true)

![Alt text](qualitative_result_I_B.png?raw=true)

### Qualitative Result II

![Alt text](qualitative_result_II_A.png?raw=true)

![Alt text](qualitative_result_II_B.png?raw=true)