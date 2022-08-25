# osn-solvent-model

The repository contains the models and the literature test data for the publication: **Explainable artificial intelligence for unraveling solvent effects in organic solvent nanofiltration** by *Gergo Ignacz, Nawader F. Algadhi and Gyorgy Szekely* submitted to Journal of Membrane Science in *August, 2022*. 

![alt text](https://github.com/ignaczgerg/osn-solvent-model/blob/main/ga.PNG)
image credit: Heno Hwang, scientific illustrator at KAUST
## Dependencies

The only dependency is [chemprop](https://github.com/chemprop/chemprop) with its own dependencies.


## How to use the model for prediction
To use the model for your own molecules, you must follow these instructions (tested on Windows 10):
<ol>
  <li>Create a .csv file (my_file.csv) into the ./data folder with at least one column in with the name: "smiles" (without quotation marks)</li>
  <li>Modify the basic_prediction.sh file and change the --test_path ./data/literature.csv to --test_path ./data/my_file.csv</li>
  <li>Run the basic_prediction.sh file: <code>bash basic_prediction.sh</code></li>
  <li>Wait until the model finishes (it might take a few minutes)</li>
  <li>A my_predictions.csv file will ba added to the parent folder which contains the predicted values</li>
</ol> 

If you run the bash script without modification, the model will run the literature.csv file (the same as in the manuscript).
