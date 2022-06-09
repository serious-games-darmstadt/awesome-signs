# Awesome Sign Recognition

This repository represents an overview of our research in sign language recognition. Some of the linked repositories are private, so please contact me if there is interest in this data. You can find more information about me and my work on [our institutes website](https://www.etit.tu-darmstadt.de/serious-games/willkommen_sg/team_sg/team_sg_details_106944.de.jsp).

## Databases

### Signs and Parametrizations

* [ASL-LEX with over 2,700 signs](https://asl-lex.org)
* [Prepared and extended version of ASL-LEX with focus on parameterization](https://sign-parametrization.netlify.app)
  - [Github Repository](https://github.com/serious-games-darmstadt/sign-parametrization)
  - [GrahpQL Endpoint](https://sign-parametrization.herokuapp.com/v1/graphql)
* [Video database with over 2,000 signs and over 21,000 videos](https://github.com/dxli94/WLASL)

### Data glove recordings
- [Rock-Paper-Scissors-Gestures with 5 and 25 gestures, recorded with a *Senso Glove: DK2* data glove](https://github.com/serious-games-darmstadt/dataglove_senso-glove-dk2_rps-gestures)
- [62 different static handshapes from ASL-LEX, recorded with *Manus Prime X* data glove](https://github.com/serious-games-darmstadt/dataglove_manus-prime-x_handshapes)

## Publications

* <details>
  <summary>Flex your muscles: EMG-based serious game controls, Joint International Conference on Serious Games, 2020</summary>
  
  **Abstract**: In recent years, non-traditional input devices for digital games and applications such as wearable sensors have become increasingly avail- able and affordable. Electromyography (EMG) promises some unique ad- vantages over traditional input devices such as keyboards or gamepads by collecting input data directly at a person’s muscle. As long as the corresponding muscle is intact, EMG can be used even when physical movement is not possible, for example when a person is injured or has an amputated limb. It also allows for unique wearable positioning on the body, potentially allowing for a larger freedom of movement.
In this paper, we examine whether an EMG-based input device is feasible to control an in-game character in a digital game. In order to do so, we first assess different EMG-related technologies and available EMG devices. Based on this assessment, we develop an EMG-based input device that can be connected to a computer. We develop a side scrolling game which can be connected to the EMG-based input device and allows for the player to switch between keyboard- and EMG-based controls. Lastly, we evaluate our developed system empirically and discuss the feasibility of EMG-based game controllers based on observed practical and theo- retical limitations of the technology.

  **Keywords**: human-computer-interaction, health games, electromyography

  **Comment**: Has shown us that EMG is not suitable for recognition of many handshapes (at least not as long as it is supposed to be easy to use)
</details>

* <details>
  <summary>Rock beats Scissor: SVM based gesture recognition with data gloves, WristSense/PerCOM, 2021</summary>
  
  **Abstract**: Hand gestures play an important role in human communication, particularly when auditory communication is limited. Akin to speech recognition, hand gesture recognition can therefore be a useful tool to facilitate communication and for more immersive computer interaction. In this paper, we examine the mobile recognition of hand gestures using data recorded with sensor gloves. We design a system based on Support Vector Ma- chines (SVM), capable of recognizing 5 different hand gestures. In an experiment with 11 participants, we determine applicable hyperparameters based on performance on the training set which translates into 100% classification accuracy on the test set. In an additional practical experiment with 9 participants, our system achieves up to 98% in a personalized and up to 87.5% in a generalized model setting.

  **Keywords**: gesture recognition, wearable, machine learning, data glove, support vector machine, rock-paper-scissor

  **Comment**: Feasibility study on gesture classification using data gloves with small number of gestures (= 5) and SVM.
</details>

* <details>
  <summary>Towards handshape identification for automatic gesture recognition using sign notation systems, European Conference on Social Media, 2021</summary>
  
  **Abstract**: Today, about 72 million people worldwide are speaking sign language. Since many deaf people are also dumb, they cannot communicate with hearing people through spoken language, even if they can lip-read. But sign language is difficult to learn, and more than 300 different sign languages in the world make things even more challenging. Therefore, to support the learning of sign language, we want to develop a gamified learning app for sign language that includes automatic sign recognition. The application should provide constructive feedback to the user about the quality of the executed sign. Each sign could be parameterised in terms of its characteristic handshape and its orientation and position: the more parameters are available, the more accurate and detailed feedback can be provided for the user. However, the parameters must also be distinguishable from a technical point of view.
  In linguistics, different notation systems exist to translate signs into written form. For this, the systems decompose signs into their characteristic properties. We want to utilise these notation systems to reduce signs to parameters that are easy to measure, e.g., the hand's shape, orientation, or position. Since the sign notation systems originate from different fields and have different backgrounds, they also differ in their objectives and thus in numbers and extents of parameters and respective features, further called symbols. Therefore, there are systems whose notations have just enough detail to identify the meant sign and those with so much detail that the reader can reproduce the sign. This higher number of details is reflected in a higher number of parameters and symbols.
  Hence, we present eleven sign notation systems, starting by examining the handshape as the most concise parameter of sign language. We compare it in the context of notation systems for its suitability for our gamified learning app for sign language. A clear differentiation of the handshapes needed for American Sign Language is essential for qualitative feedback for the user. At the same time, a small number of handshapes should reduce the technical effort required for reliable recognition.

  **Keywords**: handshape identification, gesture recognition, sign language, sign notation systems, sign learning app

  **Comment**: Good for learning about different sign language notation systems, however we now determine the parameters/handshapes needed via the ASL-LEX database.
</details>

* <details>
  <summary>Paper beats Rock: Elaborating the best machine learning classifier for hand gesture recognition, Joint International Conference on Serious Games, 2022</summary>
  
  **Abstract**: The research field of Human-Computer-Interaction (HCI) is constantly searching for innovative ways to control and interact with electronic devices. Gestures are a natural way of communication for humans. Therefore we investigated the suitability of the Senso Glove: DK2 data glove and a Support Vector Machine (SVM) for recognizing gestures of the popular game Rock-Paper-Scissors (RPS) in a previous work [1]. Building on this, we now want to increase the scope of training and testing data and evaluate different kinds of Machine-Learning (ML) classifiers in addition to the SVM. For this, we ingested two different datasets, optimized them using grid search, and evaluated all user data using the leave-one-out process. Our results show that for a small num- ber of gestures, Logistic Regression (LogReg) has the highest accuracy (97.6%) in predicting the results quickly. For a larger dataset, Random Forest (RF) achieves the highest accuracy (82.4%). Random Forest (RF) and LogReg give very good results on both datasets (average 89.7%, both), but LogReg is significantly faster overall. If the training and test data are not separated by user and are thus user-dependent, the results for both data sets improve to 99.2% and 99.5% with SVM, respectively, and again RF performs very well, with LogReg showing small weaknesses here.
In addition, we investigated how the accuracy of the classifiers performed when we gradually reduced the number of gestures from 25 to three in a dataset with 25 gestures.

  **Keywords**: gesturerecognition, machinelearning·Rock-Paper-Scissors, classification, data glove, Senso Glove: DK2, support vector machine, decision tree, random forest, k-nearest-neighbor, logistic regression, gaussian naive bayes, perceptron, feed-forward neural networks.

  **Comment**: Comparison of different classifiers for data from a simple data glove at 5 and 25 gestures.
</details>

## Theses
- Augmenting Finger Motion Data for Hand Gesture Recognition using Video-based Zero-Shot Domain Adaption
  - [Github Repository](https://github.com/serious-games-darmstadt/BA_augmented_finger_motion_data)
- [Recognition and classification of handshapes of American finger alphabet](https://www.etit.tu-darmstadt.de/serious-games/lehre_sg/abschlussarbeiten_sg/abschlussarbeiten_sg_details_14208.de.jsp)
  - [Github Repository](https://github.com/serious-games-darmstadt/BA_data_glove_asl)
- [Towards sign parametrization by using MediaPipe](https://www.etit.tu-darmstadt.de/serious-games/lehre_sg/abschlussarbeiten_sg/abschlussarbeiten_sg_details_17664.de.jsp)
  - [Github Repository](https://github.com/serious-games-darmstadt/BA_signs_video_parametrization)
- [Towards arm posture detection using sensor fusion and extended Kalman filter](https://www.etit.tu-darmstadt.de/serious-games/lehre_sg/abschlussarbeiten_sg/abschlussarbeiten_sg_details_14080.de.jsp)
  - [Github Repository](https://github.com/serious-games-darmstadt/MA_arm_posture_detection)
  - [Predecessor work](https://github.com/serious-games-darmstadt/imu-controller)
- [Augmenting Wearable Sensor Data For Sign Language Recognition](https://www.etit.tu-darmstadt.de/serious-games/lehre_sg/abschlussarbeiten_sg/abschlussarbeiten_sg_details_18880.de.jsp)
  - [Github Repository](https://github.com/serious-games-darmstadt/BA_data_enrichment)
- [Classification of signs according to Battison based on their articulatory complexity](https://www.etit.tu-darmstadt.de/serious-games/lehre_sg/abschlussarbeiten_sg/abschlussarbeiten_sg_details_18816.de.jsp)
  - [Github Repository](https://github.com/serious-games-darmstadt/MA_battison_classification)
- Towards metaclassification of complex handshape recognition
  - [Github Repository](https://github.com/serious-games-darmstadt/MA_handshape_metaclassifier)

## Others

* [Tool to classify handshapes and compare with 8 different classifiers](https://github.com/serious-games-darmstadt/gesture-classifier)
  - [Predecessor tool, here still with the possibility to classify data from Leap Motion in addition to data glove data](https://github.com/serious-games-darmstadt/leap_motion_and_data_glove_classifier)
* [Different graphics and visualizations of signs, handshapes, ...](https://github.com/serious-games-darmstadt/sign-visualizations)
* [Camera controlled browser games to learn sign language](https://sign-games.com)
  - [Github Repository](https://github.com/serious-games-darmstadt/sign-games)
