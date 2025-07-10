# Cat vs Dog Image Classification using SVM

This project implements a Support Vector Machine (SVM) to classify images of cats and dogs using the [Kaggle PetImages dataset](https://www.kaggle.com/c/dogs-vs-cats/data). The workflow includes image preprocessing, feature scaling, dimensionality reduction with PCA, and SVM classification.

## Project Structure

- `Classifiaction_Using_SVM.ipynb` — Main Jupyter notebook for the SVM pipeline.
- `PetImages/` — Folder containing `Cat/` and `Dog/` subfolders with images.
- `X.npy`, `y.npy` — Saved preprocessed data for faster loading.

## Requirements

- Python 3.x
- numpy
- scikit-learn
- pillow

Install dependencies with:
```sh
pip install numpy scikit-learn pillow
```

## Dataset Setup

1. **Download** the [PetImages dataset](https://www.kaggle.com/c/dogs-vs-cats/data) from Kaggle.
2. **Extract** the `PetImages` folder into the same directory as this notebook.  
   Your structure should look like:
   ```
   your_project/
   ├── Classifiaction_Using_SVM.ipynb
   └── PetImages/
       ├── Cat/
       └── Dog/
   ```

## How to Run

1. Open `Classifiaction_Using_SVM.ipynb` in Jupyter Notebook or VS Code.
2. Run all cells.  
   - The notebook will load and preprocess images (can take a few minutes).
   - It will save preprocessed data as `X.npy` and `y.npy` for faster future runs.
   - The SVM model will be trained and evaluated, and accuracy will be displayed.

## Customization

- **Change number of images:**  
  Edit the `max_images` parameter in the notebook to use more or fewer images per class.
- **Change image size:**  
  Edit the `img_size` parameter in the `load_images_from_folder` function.

## Notes

- The notebook uses relative paths, so it works on any system as long as the folder structure is correct.
- For best results, use a GPU and consider deep learning models (CNNs) for higher accuracy.

## License

This project is for educational purpose
