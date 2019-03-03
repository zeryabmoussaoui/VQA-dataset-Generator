This repository aims to generate a VQA dataset in a specific domain.

There are 3 notebooks out there:
	-visual-genome : generate a domaine specific dataset from visual genome by filtering images that contain objects provided in the 		keyword text file and not provided the negative keyword text file
	-VQA : generate a domaine specific dataset from VQA v2 dataset by filtering questions that contain keyword provided in the keyword 		text file
	-raw_images_generator : generate a domain specific dataset from raw images. We apply an object detection algorithm (in this case yolo) 		and apply some question templates to the detected objects to generate questions. The questions of course are very limited compared to 		human generated questions in other datasets.

Each notebook contains a variables section. Any user of this code must fill the variable with his specific needs to see the notebooks work fine.
There are some sections that were specific to the generation of indoor scenes like the room template questions,the transformation from an image extention to JPG or the section "Special usecase applyed to NUY Depth V2 dataset" or the keywords files. If you don't need them, just remove them. (see inside notebooks there are commented sections)
I have used Google Colab when writing this code, so in each notebook, there is a code that mounts drive on colab, you can skip that one if you don't use Colab or drive on Colab.
Use the Yolo directory contained in this project because I modified him to get additional commands.

