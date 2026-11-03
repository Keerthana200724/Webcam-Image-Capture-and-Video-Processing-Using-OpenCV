# Image Capture and Video Processing Using OpenCV

---

## Aim

To write a Python program using OpenCV to capture an image from the webcam and perform the following operations:

1. Write the frame as a JPG file  
2. Display the video  
3. Display the video by resizing the window  
4. Rotate and display the video  

---

## 🛠️ Software Used

- Anaconda – Python 3.7  
- Jupyter Notebook / VS Code  
- OpenCV (`cv2`)  

---

## ⚙️ Algorithm

### Step 1:
Import the required libraries and initialize the webcam using `cv2.VideoCapture()`.

### Step 2:
Capture frames continuously from the webcam.

### Step 3:
Save a frame as a JPG image using `cv2.imwrite()`.

### Step 4:
Display the live video stream using `cv2.imshow()`.

### Step 5:
Resize the frame and rotate it using OpenCV functions, then display the processed frames.

---

## 💻 Program

### Developed By:
**Name:** _DHARSHINI V______________________  

### Register No:212225100010
---
```

# Image Capture and Video Processing Using OpenCV

import cv2

# STEP 1: Initialize Webcam

cap = cv2.VideoCapture(0)

if not cap.isOpened():
    print("Webcam not detected!")
    exit()

# STEP 2: Capture Frames Continuously

while True:

    ret, frame = cap.read()

    if not ret:
        print("Unable to capture video")
        break

    # STEP 3: Save Frame as JPG Image

    cv2.imwrite("captured_image.jpg", frame)

    # STEP 4: Display Original Video

    cv2.imshow("Original Video", frame)

    # STEP 5: Resize Video to 640 x 480

    resized = cv2.resize(frame, (640, 480))

    cv2.imshow("Resized Video", resized)

    # STEP 6: Rotate Video 90 Degrees Clockwise

    rotated = cv2.rotate(
        frame, cv2.ROTATE_90_CLOCKWISE
    )

    cv2.imshow("Rotated Video", rotated)

    # Press 'q' to exit

    if cv2.waitKey(1) & 0xFF == ord('q'):
        break

# STEP 7: Release Webcam and Close Windows

cap.release()
cv2.destroyAllWindows()

print("Video processing completed successfully!")
```

## Output

### i) Write the frame as JPG image
Captured image is saved as `captured_image.jpg`


### ii) Display the video
Live webcam video is displayed
# Image Capture and Video Processing Using OpenCV

---

## Aim

To write a Python program using OpenCV to capture an image from the webcam and perform the following operations:

1. Write the frame as a JPG file  
2. Display the video  
3. Display the video by resizing the window  
4. Rotate and display the video  

---

## 🛠️ Software Used

- Anaconda – Python 3.7  
- Jupyter Notebook / VS Code  
- OpenCV (`cv2`)  

---

## ⚙️ Algorithm

### Step 1:
Import the required libraries and initialize the webcam using `cv2.VideoCapture()`.

### Step 2:
Capture frames continuously from the webcam.

### Step 3:
Save a frame as a JPG image using `cv2.imwrite()`.

### Step 4:
Display the live video stream using `cv2.imshow()`.

### Step 5:
Resize the frame and rotate it using OpenCV functions, then display the processed frames.

---

## 💻 Program

### Developed By:
**Name:** _DHARSHINI V______________________  

### Register No:212225100010
---
```

# Image Capture and Video Processing Using OpenCV

import cv2

# STEP 1: Initialize Webcam

cap = cv2.VideoCapture(0)

if not cap.isOpened():
    print("Webcam not detected!")
    exit()

# STEP 2: Capture Frames Continuously

while True:

    ret, frame = cap.read()

    if not ret:
        print("Unable to capture video")
        break

    # STEP 3: Save Frame as JPG Image

    cv2.imwrite("captured_image.jpg", frame)

    # STEP 4: Display Original Video

    cv2.imshow("Original Video", frame)

    # STEP 5: Resize Video to 640 x 480

    resized = cv2.resize(frame, (640, 480))

    cv2.imshow("Resized Video", resized)

    # STEP 6: Rotate Video 90 Degrees Clockwise

    rotated = cv2.rotate(
        frame, cv2.ROTATE_90_CLOCKWISE
    )

    cv2.imshow("Rotated Video", rotated)

    # Press 'q' to exit

    if cv2.waitKey(1) & 0xFF == ord('q'):
        break

# STEP 7: Release Webcam and Close Windows

cap.release()
cv2.destroyAllWindows()

print("Video processing completed successfully!")
```

## Output

### i) Write the frame as JPG image
Captured image is saved as `captured_image.jpg`


### ii) Display the video
Live webcam video is displayed
<img width="1600" height="962" alt="WhatsApp Image 2026-11-03 at 8 26 02 AM" src="https://github.com/user-attachments/assets/53fa95fe-7384-4c63-996d-0b322331289f" />

### iii) Display the video by resizing the window
Video is shown in resized resolution (640 × 480)
<img width="1460" height="977" alt="WhatsApp Image 2026-11-03 at 8 26 03 AM" src="https://github.com/user-attachments/assets/2364a2ae-544f-4049-8d62-df465046122b" />


### iv) Rotate and display the video
Video is displayed after rotation (90° clockwise)
<img width="1600" height="937" alt="WhatsApp Image 2026-11-03 at 8 26 03 AM (1)" src="https://github.com/user-attachments/assets/035f0c19-d7d2-44a9-9b2b-7d2d08083fa6" />


---

## Result

Thus, the image is successfully captured from the webcam and various video processing operations such as saving, displaying, resizing, and rotating are performed using OpenCV.



### iii) Display the video by resizing the window
Video is shown in resized resolution (640 × 480)
<img width="565" height="387" alt="Screenshot 2026-10-30 105415" src="https://github.com/user-attachments/assets/7424d836-fda5-437f-aff4-eabdb6881402" />


### iv) Rotate and display the video
Video is displayed after rotation (90° clockwise)
<img width="795" height="918" alt="Screenshot 2026-10-30 105351" src="https://github.com/user-attachments/assets/4361ae21-f6c8-49b1-ab3e-ea6e60236a39" />


---

## Result

Thus, the image is successfully captured from the webcam and various video processing operations such as saving, displaying, resizing, and rotating are performed using OpenCV.
