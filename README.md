### This isn't so much an attempt to do well at the challenge as a way to mess around with autoencoders to make pretty clouds.

### If we were to classify using a conditional autoencoder though: 
  1)
    * Scan the input image like a convolution (left->right, up->down)
    * Try each label (there's only 4 luckily) to see how good the reconstruction is. 
    * Pick the label with the best performance.
    * "Learn" a mask by finding the highest confidence regions in the scanned image.
  
  2)
    * Integrate the class information into the loss (use a discriminator network). 
    * Can add a discriminative network that's fed the reconstructed image too.
    
Obviously we can use samples from the cVAE for data augmentation too..
