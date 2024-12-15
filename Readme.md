# Webcam Image Classification

This repository contains code for a simple webcam image classification project using a pre-trained customized model and the p5.js library. The project allows real-time image classification using a webcam feed.

## Prerequisites

- A modern web browser that supports the MediaDevices API (e.g., Chrome, Firefox)
- An internet connection

## Usage

1. Clone or download this repository to your local machine.
2. Train an image classification model in [Google Teachable Machine](https://teachablemachine.withgoogle.com/train/image) and replace the link in sketch.js
   ```js
   let imageModelURL = 'https://teachablemachine.withgoogle.com/models/psEZTkqnk/';
   ```
4. Update the class that you wanted to detect in line 77 in sketch.js
  ```js
  // play sound
    if (label == 'Class 2') {
      counter++;
      // Play sound if "helmet" is continuously predicted for 5 times
      if (counter >= 2) {
        audio.play();
        counter = 0; // Reset the counter
      }
    } else {
      counter = 0; // Reset the counter if prediction is not "helmet"
    }
  ```

6. Open the `index.html` file in a web browser.

7. Allow the browser to access your webcam when prompted.

8. The webcam video feed will be displayed on the page, and the image classification will be performed in real-time.

## Model

The image classification model used in this project is hosted on Teachable Machine and you should use your own url.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Credits

- The ML5.js library: [ML5.js](https://ml5js.org/)
- p5.js library: [p5.js](https://p5js.org/)

## Acknowledgments

Special thanks to the contributors and maintainers of the ML5.js and p5.js libraries for providing the tools and resources necessary for this project.

## Author

[Rathees](https://github.com/ratheesk)
