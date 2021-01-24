To train StarGAN on your own dataset, create a folder structure in the same format as RaFD and run the command:

# Train StarGAN on custom datasets
python main.py --mode train --dataset RaFD --rafd_crop_size 256 --image_size 256 --c_dim 1 --rafd_image_dir data/Manga/train --sample_dir manga/samples --log_dir manga/logs --model_save_dir manga/models --result_dir manga/results

# Test StarGAN on custom datasets
python main.py --mode test --dataset RaFD --rafd_crop_size 256 --image_size 256 --c_dim 1 --rafd_image_dir data/Manga/test --sample_dir manga/samples --log_dir manga/logs --model_save_dir manga/models --result_dir manga/results

# How to add dataset 
1. add forder to data/manga/Anime/{name}
2. reshape images
3. add c_dim
4. adjust parametarts in main.py

# datasets
[anime faces](https://www.kaggle.com/soumikrakshit/anime-faces)
