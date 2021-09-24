# Autoencoders
## Vanilla autoencoder
### Datasets
We are working with two different datasets, first is Labeled faces in the wild(LFITW), it consists of photos of people and dataframe with its atributes. Another dataset is MNIST - dataset of handwritten numbers. It is used here for VAE and CVAE.
### AE
Good articles about autoencoders https://habr.com/ru/post/331382 
https://towardsdatascience.com\intuitively-understanding-variational-autoencoders-1bfe67eb5daf
<img src="https://i.imgur.com/nVJAtMT.png" alt="Autoencoder">
How autoencoder is designed "inside".
Linear autoencoder result
![изображение](https://user-images.githubusercontent.com/79093859/134654548-14342e02-6b6a-4235-8985-2ff254263a2e.png)

Convolution autoencoder result
![изображение](https://user-images.githubusercontent.com/79093859/134654653-92728da6-f29e-4b5c-b4e2-b306372f8317.png)

### Sampling
Sampling from Linear is not that awful, but that's not enough, obviously.
![изображение](https://user-images.githubusercontent.com/79093859/134654462-7bc75605-e621-4dd5-a2b7-c85ea60da699.png)

I have made two slightly different architectures of AE to compare them, Linear showed better perfomance, that's why I used it in problems, connected with LFITW
## VAE
Article about Variational autoencoders https://towardsdatascience.com/intuitively-understanding-variational-autoencoders-1bfe67eb5daf
## CVAE
![alt text](https://i.ibb.co/2tsWknB/Screen-Shot-2020-01-15-at-9-02-15-PM.png)
Conditional VAE is VAE, but input is concatenated with information about its class, so this information is used in latent code and we can easily sample pictures of different classes from one randon vector and we can sample one exact class.
