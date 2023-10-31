# Html-Code-Corrector

## Dataset

The dataset contains incorrect codes and their correct codes in html. The dataset is generated synthetically and there are 7362 unique examples.

## Preprocessing

Dataset is first transformed from text to sequences then labelled as 0 for bad and 1 for good. The dataset is then split 20% is used for validation and 20% is used for testing.

## Model

Model has 64 LSTM cells in first layer and 32 cells in second layer. Model is trained for 20 epochs. 

## Testing

At present for testing purpose training dataset is used if the model predicts it as bad then the html code is 
rectified using rule based technique.

## Results
Intially the results are as follows:

- Training and Validation Accuracy is 86%
![Model Training Accuracy](training_acc.png)

<br>
- Test Accuracy is 85%
![Model Training Loss](training_loss.png)



Bad HTML code examples are given below:

- ```<p>This is bad```
- ```<center>Centered content```
- ```<div style='color: red'>```
- ```<table><tr><td>Layout</td></tr></table>```
- ```<img src='image.jpg'>```
- ```This is content```
- ```<div custom-attr='value'>```
- ```<div id='duplicateID'>```
- ```<img src='http://insecure.com/image.jpg'>```
- ```<div>This is div</div>```

Link to website for testing purpose is:
[HTML Code Corrector](https://html-code-corrector-app.streamlit.app/)