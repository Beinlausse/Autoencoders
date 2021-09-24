# Autoencoders
## Vanilla autoencoder
### Datasets
We are working with two different datasets, first is Labeled faces in the wild(LFITW), it consists of photos of people and dataframe with its atributes. Another dataset is MNIST - dataset of handwritten numbers. It is used here for VAE and CVAE.
### AE
Good articles about autoencoders https://habr.com/ru/post/331382 
https://towardsdatascience.com\intuitively-understanding-variational-autoencoders-1bfe67eb5daf
<img src="https://i.imgur.com/nVJAtMT.png" alt="Autoencoder">
How autoencoder is designed "inside".
### 
I have made two slightly different architectures of AE to compare them, Linear showed better perfomance, that's why I used it in problems, connected with LFITW
## VAE
Article about Variational autoencoders https://towardsdatascience.com/intuitively-understanding-variational-autoencoders-1bfe67eb5daf
## CVAE
![alt text](https://i.ibb.co/2tsWknB/Screen-Shot-2020-01-15-at-9-02-15-PM.png)
Conditional VAE is VAE, but input is concatenated with information about its class, so this information is used in latent code and we can easily sample pictures of different classes from one randon vector and we can sample one exact class.
## 
