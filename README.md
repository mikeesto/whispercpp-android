# whispercpp-android

An Android app using [whisper.cpp](https://github.com/ggerganov/whisper.cpp/) to do voice-to-text transcriptions.

## Usage

1. Download a model from [here](https://huggingface.co/ggerganov/whisper.cpp) and place it in the `app/src/main/assets/models` folder. Tiny and base models work best.

2. This project relies on the `whisper.cpp` library to be built for Android. Clone the [whisper.cpp repository](https://github.com/ggerganov/whisper.cpp/) and then set the `WHISPER_CPP_DIR` environment variable to the path of the repository. In Android Studio you can do this by going to Settings -> Build, Execution, Deployment -> Gradle-Android Compiler -> Command-line Options and adding the following line:

```
-DWHISPER_CPP_DIR=/path/to/whisper.cpp
```

3. Select the `release` active build variant, and use Android Studio to run and deploy to your device.
