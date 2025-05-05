# LDM_pipeline


(mnist_prep.ipynb): creates dataset of mnist digits which can be used as a toy example
[models.py]: defines the models used for auto encoding
AETrainer.ipynb: given a tensor of images, script trains an autoencoder which outputs enc.pth & dec.pth 
diffusion_dataset_maker.ipynb: given encoder model and image tensor, script creates diffusion dataset which outputs z_set.pth, n_set.pth, l_set.pth, t_set.pth
[guided_unet.py]: define model used to predict noise of image given previous timestep, the current time, the cross attention vectors
ldm-training-xatt.ipynb: train latent diffusion model to predict noise in kaggle
