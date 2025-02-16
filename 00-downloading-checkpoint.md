Here is the **complete** `docs/00-downloading-checkpoint.md` file with all necessary updates:  

---

### **📄 `docs/00-downloading-checkpoint.md`**  

```markdown
# How to Download Checkpoints  

This guide explains how to download and set up checkpoints for DiffAE.  

## 📌 Step 1: Clone the Repository & Navigate to the Directory  
Before downloading checkpoints, first, **clone the repo** and move into the project directory:  
```sh
git clone https://github.com/phizaz/diffae.git
cd diffae
```

## 📌 Step 2: Install `gdown` for Google Drive Downloads  
`gdown` is required to download the model checkpoints from Google Drive. Install it using:  
```sh
pip install gdown
```

## 📌 Step 3: Download Pretrained Checkpoints  
Run the following command to download all checkpoints:  
```sh
gdown --folder https://drive.google.com/drive/folders/1-fa46UPSgy9ximKngBflgSj3u87-DLrw
```

Alternatively, you can manually download from:  
- **Pretrained Model Checkpoints:** [Google Drive](https://drive.google.com/drive/folders/1abNP4QKGbNnymjn8607BF0cwxX2L23jh)

## 📌 Step 4: Move Checkpoints to Correct Directory  
After downloading, place the checkpoint files into a `checkpoints/` directory:  
```sh
mkdir -p checkpoints
mv *checkpoints* checkpoints/
```

Your directory structure should look like this:  
```
checkpoints/
├── bedroom128_autoenc
│   ├── last.ckpt
│   ├── latent.ckpt
├── bedroom128_autoenc_latent
│   ├── last.ckpt
├── bedroom128_ddpm
...
```

## 📌 Step 5: Verify Checkpoints Are Downloaded  
To confirm the checkpoints are in place, run:  
```sh
ls checkpoints/
```

To check the size of each checkpoint file:  
```sh
du -sh checkpoints/*
```

Now, your checkpoints are **set up properly**, and you can proceed with running the model. 🚀  
```

---

