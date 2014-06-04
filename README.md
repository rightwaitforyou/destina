Destina
=======

##Introduction##

A DeSTIN implementation.

This project is developed under Ubuntu 12.04.3 and Mac OS X.

##To-do List##

1. Information filter based sparse coding.
2. Fast inverse (optional)
3. Test on Gabor wavelet dictionary and natural image with sparse coding.
4. Clustering algorithm for upper layer.
5. Test on second layer learned representation.
6. Centroids/Dictionary visualisation.
7. Signal composition and decomposition [done, haven't tested].
8. General mapping between layers [done, haven't tested].
9. Performance evaluation.
10. Memory leaking.
11. Interface for CIFAR image.
12. Some visualisation tools for image dataset.
13. Experiment result saving functions (needed to rescale to `uchar` space).

##Updates##

1. Gabor wavelet dictionary design [2014-04-22]
2. Image whitening updated [2014-04-24]
3. Information filter based sparse coding and test updated [2014-04-25 (undone)]
4. Main components of DeSTIN network are sketched [2014-04-27]

##Setup##

1. Clone the whole project (Matlab codes also provide some insight of the project)

2. `cd` in `cpp` folder and configure with `cmake`

   ```
   $ cd cpp
   $ mkdir build
   $ cd build
   $ cmake ..
   $ make
   ```

3. Some demonstration programs can be found in `src`, and executable can be found in `build/bin`.

4. If you want to update the program (fork and clone from your own account), you can simply use `update-all.sh`, run following code in terminal:
   ```
   $ sh update-all.sh
   ```

##Notes##

1. Example of Gabor Wavelet dictionary

   ![Gabor Wavelet Dictionary](/cpp/resources/gabor_dictionary_32_32.png)

2. Example of Whitened Image

   ![Whitened Image](/cpp/resources/whitening.png)

3. In C++ implementation, can only learn some representations roughly. However the performance is not acceptable, still need to figure out it's dictionary's problem or implementation's problem. Furthermore, the speed is not acceptable for now.

4. Example of reconstruction image with sparse autoencoder

   ![Sparse Autoencoder Reconstruction](/cpp/resources/sparse_autoencoder_reconstruction.png)

##Contacts##

Hu Yuhuang

Advanced Robotics Lab

Department of Artificial Intelligence

Faculty of Computer Science & IT

University of Malaya

duguyue100@gmail.com