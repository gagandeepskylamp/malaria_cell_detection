# malaria_cell_detection
The folder cell-images-for-detecting-malaria contain two separate folders,parasitized and uninfected, containing the respective images of the cell that in mentioned in the folder.

The image_to_csv.ipynb file contains the python code to convert the cell images in the above filed to a readable format(csv).
The predictor.ipynb file contains the code to build the k-means and random forest models and compare them with certain metrics.

#how ,the image is converted to a readable formate
the image is converted to gray scale , gauscian blur is applied , 5 countours are detected and area of 5 coutours are calculated. and stored in a csv file.

#how the models are built
using sklearn libraries the models for kmeans and random forest are imported and train with the data we got from the previous step.
metrics library is used to calculate confusion_matrix,accuracy_score,recall_score,precision_score and f1_score.
metrics of both the models are compared and random forest gave the better prediction results.
