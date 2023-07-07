# Image-Similarity

This is a Python script that compares the similarity between two images using the Streamlit framework. It utilizes computer vision techniques such as feature detection and matching to determine the degree of similarity between the images.

## Dependencies

Before running the script, make sure you have the following dependencies installed:

- streamlit
- numpy
- opencv-python
- Pillow
- matplotlib

You can install them by running the following command:

```
pip install streamlit numpy opencv-python Pillow matplotlib
```


## Usage

1. Clone the repository or download the script file.

2. Open a terminal or command prompt and navigate to the directory where the script is located.

3. Run the script using the following command:

```
streamlit run app.py
```


4. The Streamlit web application will launch in your default web browser.

5. Click on the "Upload Image 1" button to select the first image file.

6. Click on the "Upload Image 2" button to select the second image file.

7. Once both images are uploaded, the script will display the selected images and compare their similarity.

8. The degree of similarity will be shown as a percentage, and a message will indicate whether a match is found or not.

9. The script will also display an output image showing the matches between the two images.

10. You can repeat the process with different image pairs by clicking on the "Clear Cache" button in the Streamlit web application.

Note: The images should be in JPG, JPEG, or PNG format.

## Algorithm

The script uses the SIFT (Scale-Invariant Feature Transform) algorithm for feature detection and matching. Here is an overview of the algorithm steps:

1. Load the input images and convert them to grayscale.

2. Extract keypoints and descriptors from the grayscale images using the SIFT algorithm.

3. Perform feature matching between the descriptors of the two images using the Brute-Force Matcher.

4. Apply a ratio test to filter out potentially false matches.

5. Calculate the percentage similarity based on the number of good matches.

6. Display the similarity percentage and a message indicating whether a match is found or not.

7. Draw the matches between the two images and display the output image.

## License

This project is licensed under the GNU General Public License v3.0. Feel free to modify and use it.

