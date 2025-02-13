🎨 Air Canvas - Draw with Your Fingers!
This project uses Python OpenCV and Mediapipe to let you draw using your hand gestures. No mouse, no touch—just your fingers! 🤯

✨ Features:
✅ Draw using hand gestures ✋
✅ Change colors (Red, Blue, Green, Yellow) 🎨
✅ Clear the canvas 🗑️

📌 Tech Stack:
Python 🐍
OpenCV 👀
Mediapipe 🖐️
🚀 How to Run:
Install dependencies:
bash
Copy
Edit
pip install opencv-python mediapipe numpy
Run the script:
bash
Copy
Edit
python air_canvas.py
🎯 Have fun drawing in the air! Let me know if you build something cool. 😎

Algorithm Kya hai ??

1. Frames ko read karna aur HSV colour space me convert karna – Pehle hum webcam se frames read karenge aur unko HSV (Hue, Saturation, Value) format me convert karenge. HSV format use karne ka reason hai ki isme colour detection easy hota hai as compared to RGB.
2. Canvas frame prepare karna aur ink buttons add karna – Ek blank canvas frame banayenge jisme user draw kar sakega. Saath hi, different ink colours ke buttons add karenge taaki user apni pasand ka colour select kar sake.
3. Mediapipe initialization ko adjust karna (sirf ek haath detect ho) – Mediapipe library ka use karke hand tracking initialize karenge, lekin sirf ek haath detect karne ke liye settings adjust karenge.
4. RGB frame ko Mediapipe hand detector me pass karna aur landmarks detect karna – Frames ko RGB format me convert karke Mediapipe ke hand tracking model me bhejenge taaki haath ke landmarks detect ho sakein.
5. Forefinger (taarjhni ungli) ke coordinates detect karna aur store karna – Index finger ka position har frame pe detect karenge aur ek array me store karenge. Ye array basically drawing points ko track karega.
6. Stored points ko canvas aur frames pe draw karna – Jo points array me store hue hain unko use karke real-time drawing karenge. Matlab jahan ungli move karegi wahan canvas pe line ya dots draw honge.
7. 
***** Ye pura process ek AI-based virtual drawing board banayega jo haath ki movements ko detect karke screen pe draw karega! 🚀****----------------------







