# face_model_server
Models server for face recognition pipeline

### Running the service
- Download all of the necessary files and folders
- You can get the docker run command from docker_run file or:
> docker run -d --rm --name="face_ovms" -v $(pwd)/ovms_models:/models -p 30023:30023 -p 30024:30024 openvino/model_server:latest --config_path /models/config.json --port 30023
- After starting this service you have to restart face_api because this docker runs a new CPU model serving service to which face_api has to connect

### TO-DO
- [ ] Add docker-compose.yml
- [ ] Test with person detection
