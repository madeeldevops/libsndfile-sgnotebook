# Libsndfile in Sagemaker Notebook.

The following steps are to get all the necessary files for ML Engineer working on fastaudio etc.

1. Install necessary libraries 
     ```
     !pip install fastaudio torch==1.8.1 torchvision==0.9.1 torchaudio==0.8.1 wwf timm
     ```
2. Go to shell and download and install libsndfile library
     ```bash
     wget https://github.com/libsndfile/libsndfile/releases/download/1.0.31/libsndfile-1.0.31.tar.bz2`
     tar -xf filename.tar
     ```
     Navigate to the extracted folder using cd command
     ```bash
     cd foldername
     ```
     Now run the following command to install the tarball*.*
     ```bash
     ./configure
     make
     sudo make install
     ```
3. It will install your libsndfile library and you can use it.

---

- If you want a notebook pre-configured with all library. Copy the content from "lifecycle-configs-smnotebook" and paste it in notebook lifecycle configuration on start.

- You can test your libraries by running the commands provided in "notebook.ipynb".
