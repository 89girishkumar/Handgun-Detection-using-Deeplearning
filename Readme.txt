Project Name: Building a Gun Detection Model Using Deep Learning
Presentation Link:     https://youtu.be/iDIOwgEgF5Q


Name: Girish Kumar Ramachandra
California State University Fullerton



Project Methodology

•	Installation of Anaconda Python 3.7
•	install TensorFlow
•	install Tensorflow Environment	
•	TensorFlow models are already installed in (TensorFlow\models)
•	Install necessary packages in python (pillow, lxml, jupyter, matplotlib, opencv, cython,pathlib)
•	Installed google protobuf
•	Add necessary Environment Variables(PYTHONPATH)
•	install COCO API
•	Install Labelimg
•	i would suggest to paste the whole TensorFlow folder in C:/Users/
•	Now, to initiate a new training job, cd inside the training_demo folder and type the following in the anaconda prompt
	conda activate tensorflow_cpu
	python train.py --logtostderr --train_dir=training/ --pipeline_config_path=training/faster_rcnn_inception_v2_coco.config

•	to export a trained inference graph, 
	cd inside your training_demo folder, and run the following command: 
	python export_inference_graph.py --input_type image_tensor --pipeline_config_path training/faster_rcnn_inception_v2_coco.config --trained_checkpoint_prefix training/model.ckpt-20000 --output_directory trained-inference-graphs/output_inference_graph_v1.pb

•	to check the output go ahead 
	open anaconda prompt
	activate tensorlow environment
	cd into models and open jupyter notebook
	next manually navigate to research / object_detection / object_detection_tutorial
	run all cells to see the output at the bottom :) 