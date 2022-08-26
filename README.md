# Sign-Language-Datection
Children with the disability of hearing loss are held at a disadvantage due to the reason that they have a hard time hearing the lectures that are present on the screen. Other factors would be a mute child who would not be able to speak in according to the response of the lecturer. In order for these children to cope with education the American Sign Language was created not only to help them with education but to provide ease for their daily lives. To help these children with their education we proposed a model that will help the student make ASL gestures to the camera and have it read and provide feedback on what language was read. For this we used OpenCV with Mediapipe Holistic to identify the key markers of the poser with all the values to be collected and then be trained on the Long Short Term Memory Architecture.

## MediaPipe Holistic 
The initial step of the program is to identify the Keypoints of the user. MP Holistic is an API created by Mediapipe which identifies the keypoints on a body by identifying the holistic key points

>mp_holistic = mp.solutions.holistic mp_drawing = mp.solutions.drawing_utils

These two api calls, are calls the Holistic API uses to identify the keypoints holistic keypoints and draw it

The function >draw_landmarks(image, results)

Draws landmarks of the identified keypoints on the user

https://user-images.githubusercontent.com/77060236/186928820-d3066a85-0756-4f1d-a51e-398eb5674473.mp4


However wth a few extra lines of code > **draw_styled_landmarks(image,results)**
The keypoints can be color coded for the viewer to identify the different parts of the human

https://user-images.githubusercontent.com/77060236/186929031-bd81b42c-4324-4b85-bfec-ec1b1c1fe1bb.mp4


