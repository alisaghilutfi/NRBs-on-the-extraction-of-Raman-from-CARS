# LUT CARS Data Analysis 
# Effect of Different NRB types
Paper's link: [Effect of non-resonant background on the extraction  of Raman signals from CARS spectra using deep neural networks](https://pubs.rsc.org/en/content/articlehtml/2022/ra/d2ra03983d)

By [Rajendhar junjuri](https://scholar.google.co.in/citations?user=BRu_wuAAAAAJ&hl=en)\, [Ali Saghi](https://scholar.google.co.in/citations?view_op=list_works&hl=en&hl=en&user=GcWhnFcAAAAJ),  [Lasse Lensu](https://scholar.google.co.in/citations?user=dk2Ezl0AAAAJ&hl=en&oi=ao), and [Erik M. Vartiainen](https://scholar.google.co.in/citations?user=zbxe2qYAAAAJ&hl=en&oi=ao) 

## About Synthetic test data
These are 300 synthetic test spectra evaluated in the manuscript.

1. First, 100 spectra correspond to ‘Product of two Sigmoid NRB’.

2. Spectra 101-200 account for ‘One sigmoid NRB’.

3. Spectra 201-300 correspond to ‘Polynomial NRB’.

"y_test_300_merge_spectra3.npy"---> referes to the true Raman signal

"x_test_300_merge_spectra3.npy"---> referes to the input CARS data

## About the experimental CARS test data
The experimental CARS test data set used in this investigation can only be provided upon request and can contact [Erik M. Vartiainen](https://research.lut.fi/converis/portal/detail/Person/56843?auxfun=&lang=en_GB) 

## About the CNN model code

The model architecture is directly adapted from the SpecNet paper (See https://github.com/Valensicv/SpecNet for the full code of the neural network model)
Here three different NRBs are evaluated. 

It can be accessed from the following program.
RSS_Advances_CNN_to_train_with_different_NRBs.py

Testing can be done by using the following program.
RSS_Advances_CNN_prediction_on_test_data.py

## About the trained model weights

"One_sigmoid_NRB_model_weights.h5" --->referes weights of the model trained with One sigmoid NRB.

"Polynomial_NRB_model_weights.h5" --->referes weights of the model trained with Polynomial_NRB.

"Specnet_weights.h5" --->referes weights of the model trained with the product of two sigmoids NRB

## Getting Started and Requirements 
You can use Python (TensorFlow 2.7.0) to test the pre-trained network. We have tested it in Spyder.

## Article can be found here 
https://scholar.google.co.in/citations?view_op=view_citation&hl=en&user=BRu_wuAAAAAJ&sortby=pubdate&citation_for_view=BRu_wuAAAAAJ:ULOm3_A8WrAC
