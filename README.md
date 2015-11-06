`docker build -t rectalogic/neural-style:latest .`

`docker run -i -v /tmp/images:/root/neural-style/images -v /tmp/outputs:/root/neural-style/outputs -t rectalogic/neural-style:latest -gpu -1 -proto_file models/VGG_ILSVRC_19_layers_deploy.prototxt -model_file models/VGG_ILSVRC_19_layers.caffemodel -style_image images/starry_night.jpg -content_image images/hoovertowernight.jpg -output_image outputs/hoover.jpg`
