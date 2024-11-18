# APPLICATION OF HANDTRACKING IN IMAGE PROCESSING FOR NON-TOUCH DEVICE CONTROL
An Off-policy Reinforcement Learning Algorithm for Optimal Tracking Control Problem

Full report: [Link](https://drive.google.com/drive/folders/1c36tEH7o8h9nW9n_5ceyp_sqpw7lBP_1?usp=drive_link)
## 1. Introduction
The COVID-19 pandemic inflicted substantial losses on Vietnam, with nearly 1.7 million infections and over 31,000 deaths. The pandemic's devastation overwhelmed healthcare systems and left profound scars. Despite successful containment efforts, the risk of resurgence persists. Close contact between individuals and contaminated surfaces remains a primary driver of SARS-CoV-2 transmission. To address this, we have developed a touchless control system, a cutting-edge technology of the 4.0 era.

This system employs a trained Hand Tracking model to identify hand landmarks, enabling gesture-based control and interaction with hardware components, including LED lights and alarms. This application not only mitigates direct contact during pandemics but also holds significant potential for industrial device control, enhancing production efficiency and workplace safety.
## 2. Module HANDTRACKING

![image](https://github.com/user-attachments/assets/032bc792-3ef3-4a7f-b28e-5aea855e8343)

The HandTracking module is part of the MediaPipe library, developed by Google to provide real-time image and video processing solutions. The module uses pre-trained machine learning models to recognize and track 21 landmarks on the hand, allowing you to determine the location, orientation, and gestures of the hand.

Landmark coordinates: Each landmark on the hand is represented by a set of 3 coordinates (x, y, z), in which:

x, y: 2D coordinates of the landmark in the image, normalized to the interval [0, 1].

z: Relative depth of the landmark compared to the origin (usually the wrist), also normalized to the interval [0, 1].

The closer the landmark is to the camera, the smaller the z value.

Distance between two landmarks: To calculate the distance between two landmarks, we can use the Euclidean distance formula:

$$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2 + (z_2 - z_1)^2}$$

Where:
(x1, y1, z1) are the coordinates of the first landmark.
(x2, y2, z2) are the coordinates of the second landmark.

The angle between the three landmarks: To calculate the angle between the three landmarks A, B, C (with B as the vertex), we can use the formula:

$$\cos(ABC) = \frac{AB . BC}{|AB| * |BC|}$$

Where:
AB, BC are vectors calculated from the coordinates of the landmarks.
AB . BC is the dot product of the two vectors AB and BC.
|AB|, |BC| are the lengths of the two vectors AB and BC.

## 3. Hardware System
![image](https://github.com/user-attachments/assets/83f4a59c-6565-4e16-b02e-a08d622f3b55)

## 4. Result
![image](https://github.com/user-attachments/assets/a2c05999-b5f8-4a88-bdb3-df872712d464)

![image](https://github.com/user-attachments/assets/4171392c-7bc4-4e96-9bee-fc6c304af6ba)

![image](https://github.com/user-attachments/assets/f94c632b-e689-4192-ac0d-9e2d0f505ab5)

## 5. Conclusion
Touchless recognition and control systems are garnering significant attention from leading nations and tech companies worldwide. Currently, human-computer interaction in virtual reality relies heavily on intermediary devices like sensor gloves. This technology promises a breakthrough, potentially replacing older methods. Its versatility extends to diverse fields, from healthcare and industry to everyday life, a crucial goal for any research team. This report provides a comprehensive overview of the topic. Our team aims to further develop this technology, enhancing its capabilities and expanding its applications across various domains to benefit society.

# Links to the example headings above

Link to the sample section: [Link Text](#sample-section).

Link to the helpful section: [Link Text](#thisll--be-a-helpful-section-about-the-greek-letter-Θ).

Link to the first non-unique section: [Link Text](#this-heading-is-not-unique-in-the-file).

Link to the second non-unique section: [Link Text](#this-heading-is-not-unique-in-the-file-1).
