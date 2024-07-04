# HaGRID
Hand Gesture Recognition

The code uses the MediaPipe library for detecting hand landmarks and OpenCV for processing images and video frames. It recognizes specific hand gestures (like 'V SIGN', 'SPIDERMAN SIGN', and 'HIGH-FIVE SIGN') and performs actions based on these gestures, such as applying a filter to the webcam feed or capturing an image. The code also integrates Pygame for playing a sound when an image is captured.

Detailed Analysis
Hand Landmark Detection and Finger Counting
Initialization:

Import necessary libraries.
Initialize the MediaPipe hands module and drawing utilities.
Detect Hands Landmarks Function:

Detects hand landmarks in a given image using MediaPipe.
Optionally displays the image with landmarks.
Count Fingers Function:

Determines which fingers are up based on hand landmarks.
Returns the status of each finger and the total count of fingers up.
Annotate Function:

Draws annotations on the image, indicating which fingers are up.
Optionally displays the annotated image.

Main Gesture Recognition and Webcam Feed Handling
Overlay Handprint Function:

Adds an image of a handprint to the main output image at a specified position.
Webcam Initialization and Frame Processing:

Captures frames from the webcam and processes each frame to detect hand landmarks and count fingers.
Visualizes the counted fingers in real-time.

Gesture Recognition and Actions
Recognize Gestures Function:

Recognizes specific hand gestures based on the status of fingers.
Updates the image with the recognized gesture and optionally displays it.
Sample Images Processing:

Processes sample images to demonstrate gesture recognition.
Webcam Gesture Recognition:

Captures frames from the webcam.
Recognizes gestures and performs actions based on the recognized gestures (e.g., applying a filter, capturing an image).

Applying Filters and Capturing Images
Filter Application:

Applies a filter image over the webcam feed when a specific gesture ('SPIDERMAN SIGN') is recognized for a certain number of consecutive frames.
Image Capture:

Captures an image when the 'V SIGN' gesture is recognized for a certain number of consecutive frames.
Plays a sound to indicate the image capture and displays the captured image.
Overlay Captured Image:

Overlays the captured image on the live webcam feed.
Webcam Feed Management:
Continuously captures frames from the webcam and processes them.
Handles keypress events to exit the loop and release the webcam.

Key Functionalities

Hand Landmark Detection: Uses MediaPipe to detect and draw hand landmarks on images and video frames.

Finger Counting: Determines which fingers are up and counts them.

Gesture Recognition: Identifies specific hand gestures based on finger statuses.

Filter Application: Applies a visual filter to the webcam feed based on gesture recognition.

Image Capture: Captures and saves an image when a specific gesture is recognized.

Real-time Webcam Processing: Continuously processes frames from the webcam to provide real-time gesture recognition and interaction.

Libraries and Tools Used

MediaPipe: For hand landmark detection.

OpenCV: For image and video processing.

Pygame: For playing audio when capturing images.

Matplotlib: For displaying images.

The code effectively combines these tools to create an interactive system that can recognize hand gestures and respond with specific actions, demonstrating a practical application of computer vision and gesture recognition.
