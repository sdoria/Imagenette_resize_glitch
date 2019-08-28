# Imagenette: Resizing Images Twice Decreases Accuracy

Based on a discovery by Less Wright (https://github.com/lessw2020)


We compare validation accuracy for two resizing methods on Imagewoof[1]  (128px) :

(a) Resizing images to 128px from Imagewoof-160 (a 160px version of Imagewoof)

(b) Resizing images to 128px from Imagewoof-full_size (full size images)

| Epochs | Imagewoof-160 (a) | Imagewoof-full_size (b) | # of runs | p-value |
|---|---|---|---|---|
| 5 | 61.25% | 63.89% | 20 | 0.0001 |
| 20 | 80.87% | 82.40% | 3 | 0.043 |



[1] https://github.com/fastai/imagenette
