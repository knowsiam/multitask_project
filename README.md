# arch

multitask_project/
    classification/
    dataset/
        image/
            hydronephrosis_data_original/
                fold1/
                    abnormal/
                    normal/
                fold2/
                    abnormal/
                    normal/
                ...
                fold10/
                    abnormal/
                    normal/
            pericardium_data_resize/
                fold1/
                    mask/
                    process_img/
                fold2/
                    mask/
                    process_img/
                ...
                fold10/
                    mask/
                    process_img/
        radiomics_vector/
    radiomics/
    segmentation/
    README.md



# git
```bash

git add -A
git commit -m "chore: 更新所有檔案"
git pull --rebase origin <分支名稱>
git push origin <分支名稱>

```

# 用法
- 抽特徵
```python

python -m radkit.extract_features

```
- 訓練與驗證（10 折）
```python

python -m classification.train_classifier --model logreg --seed 42

```


