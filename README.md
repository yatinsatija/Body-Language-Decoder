# Body-Language-Decoder

The proposed work aims to leverage state of the art body, facial and hand landmark extraction frameworks to come up with a custom machine learning model which is capable of recognizing the type of action being performed in the video source. The work is titled ‘Machine Learning based body language decoder’ that takes into account body, facial and hand landmark coordinates to arrive at the output.

## Objectives

- Use of state of the art frameworks to extract body joint coordinates from the input for effective computer vision based modelling of the human body.
- Creation of a machine learning model which would be trained on a custom dataset so created.
- Usage of this model in the real time on web cameras to capture and detect body language accordingly
- Comparison and analysis of various machine learning model architectures with respect to performance and limitations.

## Functional requirements

Functional requirements define the basic system behaviour. Essentially, they are what the system does or must not do, and can be thought of in terms of how the system responds to inputs. Functional requirements usually define if/then behaviours and include calculations, data input, and business processes.<br/>

1. Frame Extraction and Processing:<br/>
   The proposed system demands to have a mechanism where in each frame from video input has to be separated and introduced into a state of the art landmark extraction model. This phase has equal importance in both dataset creation and real time deployment phase as each frame gets processed.
2. Dataset Generator:<br/>
   To be able to create a custom dataset from the video stream and encapsulate the extracted landmark coordinates into a dataframe, there should be a system which automatically does the same to enhance the dataset creation process. Hence, a module it to be created which implements this functionality.

3. Action/Gesture Classification based on Machine Learning:<br/>
   Upon successful extraction of face and body landmarks through the input source, those landmarks are passed through machine learning/deep learning based classifiers to detect the type of action/gesture performed by the subject under consideration from the given frame.

4. GUI to display Action type in real time:<br/>
   To deploy the model in real time scenarios where the input is being taken from video sources like webcam, it is of paramount importance to have a GUI based interface which displays the action type along with the confidence metric to the user.

## Hardware requirements

Minimum requirements:

- 4GB RAM
- Quad core processor
- 2GB integrated GPU<br/>
  Recommended requirements:
- CPU: Model name: Intel(R) Xeon(R) CPU @ 2.30GHz
- Cache size: 46080 KB
- GPU: single 12GB NVIDIA Tesla K80 GPU
- 13 GB RAM

## Software requirements

- Python 3.5 or higher
- Open source human body modelling framework - MediaPipe
- Scikit learn preprocessing
- Scikit learn classifiers - LogisticRegression, RidgeClassifier, RandomForestClassifier, GradientBoostingClassifier
- Opencv- python
- Numpy
- Pandas
