 
# To run the model locally 
Due to file size restrictions, the keras and tflite models could not be uploaded to the repository. <br>

1. To download keras model and create the tflite model, run the command in a terminal: `python convert_keras_to_tflite.py`
2. To build the docker image, run the command in a terminal: `docker build -t dino-dragon-model .`
3. To run the built docker image, run the command: `docker run -it --rm -p 8080:8080 dino-dragon-model` <br>
   This will run lambda_function.py indefinitely in the container 
5. Then open a second terminal run the command: `python test-local.py` 
6. The output will be printed in the 2nd terminal below the command.
