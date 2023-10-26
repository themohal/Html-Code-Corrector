# Html-Code-Corrector

## Dataset

The dataset contains on very small list of incorrect codes and correct codes.

## Preprocessing

Dataset is first transformed from text to sequences then labelled as 0 bad and 1 good. 

## Model

Model is has 64 LSTM cells in first layer and 32 cells in second layer. Model is trained for 20 epochs. 

## Testing

At present for testing purpose training dataset is used if the model predicts it as bad then the html code is 
rectified using rule based technique.

## Results
Intially the results were good below is the provided list of bad practices that is used for training: 

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


