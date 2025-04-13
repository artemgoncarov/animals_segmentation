# animals_segmentation

## Top 1 solution of AI Academy hackathon 2025

**Description of our solution**:
1) For animal detection, we trained YOLO 11l
2) For segmentation, the SAM large model was trained, and inference was done on YOLO bboxes

## More details:

**YOLO**:
We decided to train the YOLO 11l model, since 11x is quite a heavy architecture and overfitted, so we took a simpler model.
The model was trained on your training data, to which various augmentations were applied using the Roboflow service.
On inference, if the model did not find bboxes, then we apply augmentations until the model finds objects.

**SAM**:
We decided to retrain the SAM Large model on your augmented data. Then we infer the model on YOLO boxes.

**Link on YOLO dataset**:
https://www.kaggle.com/datasets/artemgoncarov/animals-augmentations-segmentation-data

**To download the SAM dataset, use the code in the notebook.**

## Instructions for launching:
1) launch all cells in YOLO.ipynb
2) launch all cells in SAM.ipynb

## Weights

https://drive.google.com/file/d/1f4jEd2xKRFDtHLyFCCjhDKnXgcef3vBV/view?usp=gmail
