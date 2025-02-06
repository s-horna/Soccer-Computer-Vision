
# Soccer Computer Vision

This project detects soccer (or football for all non-Americans) players, referees, and ball movements in clips taken from a TV broadcast angle. I used Roboflow to access the [Training Dataset](https://universe.roboflow.com/roboflow-jvuqo/football-players-detection-3zvbc) that I used to train my local YOLOv8 model using Ultralytics. I used the SentenceTransformers package to access their clip-ViT-B-32 model that I used to differentiate the teams each player was on. I used the Supervision library for video utilities and annotations.
## Demo

![til](https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExdXFkZHNwaDNrYTRudHQwamc3NmpidW4xMDJzemN3a3g3cjM3aWJxbCZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/WnjNyCrzfwLIk1j4u7/giphy.gif)
![til](https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExaHBmazl3ZTFhNDNnaGtoY2Y0N2RtcHoxOTVmaGtzcDNwbndiZ2FneSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/5pPGw6Aay99LWKqW7p/giphy.gif)


## Installation

Install the project with git clone

```bash
  git clone https://github.com/s-horna/Soccer-Computer-Vision.git
  cd my-project
```
    
## Usage

1) Train the YOLO model by running the `training\player_ref_ball_detection_training.ipynb` notebook on a GPU (I used T4 GPU on Google Colab and it took about an hour).
2) Copy the models into the `models` folder
3) Run the `SoccerCV.ipynb` notebook and specify the video path you want to analyze.
## Acknowledgements

 - [Football AI Tutorial](https://www.youtube.com/watch?v=aBVGKoNZQUw)
 - [Build an AI/ML Football Analysis system with YOLO, OpenCV, and Python](https://www.youtube.com/watch?v=neBZ6huolkg&t=2514s)
 - [CLIP model](https://huggingface.co/sentence-transformers/clip-ViT-B-32)
 - [Ultralytics](https://docs.ultralytics.com/)
 - [Supervision](https://supervision.roboflow.com/latest/)
 - [Roboflow](https://universe.roboflow.com/)


## License

[MIT](https://choosealicense.com/licenses/mit/)

