

---

### **📄 `docs/01-running-checkpoint.md`**  

```markdown
# How to Run DiffAE  

This guide explains how to set up and run DiffAE for training and inference.  

## 📌 Step 1: Clone the Repository & Navigate to the Directory  
Before running DiffAE, first, **clone the repository** and move into the project directory:  
```sh
git clone https://github.com/phizaz/diffae.git
cd diffae
```

## 📌 Step 2: Install Dependencies  
Install all required dependencies:  
```sh
pip install -r requirements.txt
```
For **Google Colab**, install additional dependencies:  
```sh
sh install_requirements_for_colab.sh
```

## 📌 Step 3: Run Training  
To train the model, use one of the following commands depending on the dataset:  

- **FFHQ128 (Faces)**  
  ```sh
  python run_ffhq128.py
  ```

- **CelebA64**  
  ```sh
  python run_celeba64.py
  ```

- **Horse128**  
  ```sh
  python run_horse128.py
  ```

- **Bedroom128**  
  ```sh
  python run_bedroom128.py
  ```

## 📌 Step 4: Run Pretrained Model for Sampling  
To **generate samples** using the pretrained model:  
```sh
python experiment.py --sample
```

## 📌 Step 5: Evaluate Model (FID Score)  
To compute the **Fréchet Inception Distance (FID) score** for evaluation:  
```sh
python run_ffhq128.py --eval_fid
```

Now, DiffAE is running successfully! 🚀  
```

---

