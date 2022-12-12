# AI Rock Paper Scissors
This is the development environment for the weights required for the AI Rock Paper Scissors game. This project consists on two parts the backend which heavily relies on the weights generated on this repository for making inferences; and the frontend which provides a user interface the allow the player to interact with this classifier in a game like environment.

There are three versions of this project each one more capable as we progress:

## V1 (Simplistic approach)
The main purpose of the version 1 of this project was to create a siple approach that we can test the feasibility of the desired backend-frontend architecture. The performance wasn't as goog as we initially expected achieving a mAP of 0.56 which is not good considering that we were only having 2 classes. We Modified the code to not only detect Fists to also detect other classes like Rock Paper and Scissors. The resulting mAP stayed relatively the same 0.56.

## V2 (Increased complexity approach)
The main purpose of the version 2 of this project aimed to increase the precision of our model. We stopped creating a model for fists and focused mainly on the important classifications of the Rock Paper Scissors hand gestures. After training we observed a significant accuracy increase resulting on 0.97 in precision. However in the practical setting with significant variation from the training set we observed that there were still miss classifications.

## V3 (Using existing robust models)
In our third version given that we wanted to reach our goal as precised as posable we decided to go with a state of the art model that's why we used the YOLOv6-L variant showcased in this repository https://github.com/meituan/YOLOv6 the main reason we chosen this approach on top of other YOLO variants its the particular mixture of tradeoffs between inference cost and accuracy. You can review this and other external work we used in the utility folder of this project.

## Datasets
We used different mixtures of datasets on different versions of this project review in the bellow section.

### V1
- [Kaggle | Rock Paper Scissors Dataset](https://www.kaggle.com/datasets/sanikamal/rock-paper-scissors-dataset)

### V2
- [Kaggle | Rock Paper Scissors Dataset](https://www.kaggle.com/datasets/sanikamal/rock-paper-scissors-dataset)
- [Kaggle | Rock-Paper-Scissors Images](https://www.kaggle.com/datasets/drgfreeman/rockpaperscissors)
- [Kaggle | Rock Paper Scissors YOLO Annotated (Created by us*)](https://www.kaggle.com/datasets/hectorandac/rock-paper-scissors-yolo-annotated)

### V3
- [Kaggle | Rock Paper Scissors YOLO Annotated (Created by us*)](https://www.kaggle.com/datasets/hectorandac/rock-paper-scissors-yolo-annotated)

We experience the best results after including our own dataset.
