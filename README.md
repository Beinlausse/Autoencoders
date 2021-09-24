# Autoencoders
## Vanilla autoencoder
### Datasets
We are working with two different datasets, first is Labeled faces in the wild(LFW), it consists of photos of people and dataframe with its atributes. Another dataset is MNIST - dataset of handwritten numbers. It is used here for VAE and CVAE.
### AE
Good articles about autoencoders https://habr.com/ru/post/331382 
https://towardsdatascience.com\intuitively-understanding-variational-autoencoders-1bfe67eb5daf
How autoencoder is designed "inside":
<img src="https://i.imgur.com/nVJAtMT.png" alt="Autoencoder">

Linear autoencoder result
![изображение](https://user-images.githubusercontent.com/79093859/134654548-14342e02-6b6a-4235-8985-2ff254263a2e.png)

Convolution autoencoder result
![изображение](https://user-images.githubusercontent.com/79093859/134654653-92728da6-f29e-4b5c-b4e2-b306372f8317.png)

I have made two slightly different architectures of AE to compare them, Linear showed better perfomance, that's why I used it in problems, connected with LFW

### Sampling
Sampling from Linear is not that awful, but that's not enough, obviously.
![изображение](https://user-images.githubusercontent.com/79093859/134654462-7bc75605-e621-4dd5-a2b7-c85ea60da699.png)

### Why are you so serious?
Here I found out "smile vector" and added it to latent code of serious people
![изображение](https://user-images.githubusercontent.com/79093859/134656550-890533c0-d5ad-4e97-8e5d-d7a21e6f5e15.png)
![изображение](https://user-images.githubusercontent.com/79093859/134656572-4c53090d-0198-460f-872c-124666068905.png)


## VAE
Article about Variational autoencoders https://towardsdatascience.com/intuitively-understanding-variational-autoencoders-1bfe67eb5daf
![изображение](https://user-images.githubusercontent.com/79093859/134656867-7c3d13f7-efc6-4dc1-bc01-d705cc4b3d63.png)
### Sampling
![изображение](https://user-images.githubusercontent.com/79093859/134656921-71e03cf7-3f09-49c7-b8f5-a55ad7751fe1.png)
Not enough yet
### Latent representation
![изображение](https://user-images.githubusercontent.com/79093859/134657070-7cdf7503-f6fc-4862-a015-a9a344344e77.png)
There is no obvious clastering, maybe because 2 dimensions is not enough.
## CVAE
![alt text](https://i.ibb.co/2tsWknB/Screen-Shot-2020-01-15-at-9-02-15-PM.png)
Conditional VAE is VAE, but input is concatenated with information about its class, so this information is used in latent code and we can easily sample pictures of different classes from one randon vector and we can sample one exact class.
![изображение](https://user-images.githubusercontent.com/79093859/134657227-0e817de8-e6c9-4f54-9b11-9ac262f8c924.png)
### Sampling
![изображение](https://user-images.githubusercontent.com/79093859/134657348-6c50316f-c0ad-4049-8f1b-d8344798d048.png)
### Latent representation
![изображение](https://user-images.githubusercontent.com/79093859/134657405-b7cc073c-95c3-4a94-910b-9aac9215d78e.png)
Here we can see some lines of distribution, but different classes can not be distinglished.

## Image Morphing
![изображение](https://user-images.githubusercontent.com/79093859/134657500-92142ece-1630-4b84-a8c1-1e4f2912e9bc.png)
That is spectacularly)

## Denoising
![изображение](https://user-images.githubusercontent.com/79093859/134657558-13a208cb-9c3b-4969-b438-6eb511042759.png)
Even simple AE works pretty well.
