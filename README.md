### 1) Use a conditional VAE to make pretty clouds! 
### 2) ??
### 3) Classify! 

### Ideas for classification: 
  1)
    * Scan the input image like a convolution (left->right, up->down)
    * Try each label (there's only 4 luckily) to see how good the reconstruction is. 
    * Pick the label with the best performance.
    * "Learn" a mask by finding the highest confidence regions in the scanned image.
  
  2)
    * Integrate the class information into the loss somehow. 
    * Can add a discriminative network that's fed the reconstructed image.
    * This could work kind of like paired inverse - forward models in Jordan & Rumelhart
    
