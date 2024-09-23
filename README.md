<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Child Speech Emotion Recognition</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #f4f4f9;
            color: #333;
            padding: 20px;
        }
        h1 {
            color: #2c3e50;
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        h2, h3 {
            color: #34495e;
            margin-bottom: 15px;
        }
        p, li {
            font-size: 1.1rem;
            line-height: 1.6;
        }
        ul {
            padding-left: 20px;
        }
        .dataset {
            background-color: #ecf0f1;
            border-left: 5px solid #2980b9;
            padding: 10px;
            margin-bottom: 20px;
            list-style: none;
        }
        .dataset li {
            font-weight: bold;
        }
        .section {
            margin-bottom: 40px;
        }
        code {
            background-color: #e8e8e8;
            padding: 2px 5px;
            border-radius: 4px;
            font-family: monospace;
        }
    </style>
</head>
<body>

    <h1>Child Speech Emotion Recognition using Deep Learning</h1>

    <div class="section">
        <h2>Introduction</h2>
        <p>This project aims to predict emotions from child speech using machine learning and deep learning techniques. We trained the model on various datasets, including <b>TESS</b>, <b>SAVEE</b>, <b>RAVDESS</b>, and <b>CREMAD</b>, all of which are commonly used for emotion recognition tasks.</p>
    </div>

    <div class="section">
        <h2>Datasets Used</h2>
        <ul class="dataset">
            <li>Crowd-sourced Emotional Multimodal Actors Dataset (Crema-D)</li>
            <li>Ryerson Audio-Visual Database of Emotional Speech and Song (Ravdess)</li>
            <li>Surrey Audio-Visual Expressed Emotion (Savee)</li>
            <li>Toronto Emotional Speech Set (Tess)</li>
        </ul>
    </div>

    <div class="section">
        <h2>Project Workflow</h2>

        <h3>1. Importing Libraries</h3>
        <p>We used several Python libraries such as <code>librosa</code> for audio processing, <code>keras</code> for deep learning, and <code>scikit-learn</code> for preprocessing and evaluation metrics.</p>

        <h3>2. Data Preparation</h3>
        <p>The datasets consist of emotional speech samples, and a dataframe was created to store emotion labels and their corresponding file paths for feature extraction.</p>

        <h3>3. Data Visualization and Exploration</h3>
        <p>We visualized the dataset to explore the distribution of emotions using bar charts. <b>Waveplots</b> and <b>Spectrograms</b> were also used to understand the audio signals.</p>

        <h3>4. Data Augmentation</h3>
        <p>We used data augmentation techniques like noise injection, time shifting, pitch alteration, and speed changes to enhance model generalization.</p>

        <h3>5. Feature Extraction</h3>
        <p>The following features were extracted from the audio signals:</p>
        <ul>
            <li>Zero Crossing Rate</li>
            <li>Chroma_STFT</li>
            <li>MFCC (Mel-frequency cepstral coefficients)</li>
            <li>RMS (Root Mean Square)</li>
            <li>MelSpectrogram</li>
        </ul>

        <h3>6. Data Preparation</h3>
        <p>Once the features were extracted, we normalized the data and split it into training and testing sets.</p>

        <h3>7. Model Architecture</h3>
        <p>We designed a Convolutional Neural Network (CNN) model to classify emotions. The model consists of convolutional layers, max pooling layers, and dropout for regularization.</p>
    </div>

</body>
</html>
