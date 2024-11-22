# **Sentence Reconstruction using Neural Networks**

## **Project Description**

This project was developed as part of the **Deep Learning** course at the **University of Bologna**. It reconstructs an original English sentence from a randomly permuted sequence of words. The reconstruction is performed using a transformer implemented in TensorFlow, and the notebook was developed in Google Colab.

### **Key Constraints**

- 🚫 **No pretrained models** were used.
- 🚫 **No postprocessing** (e.g., beam search) was applied.
- 📊 Model size is limited to **less than 20 million parameters**.
- 🎓 No additional training data was used.

---

## **Dataset**

- A synthetic dataset of permuted English sentences was used for training and evaluation.
- No additional external datasets were allowed per the project constraints.

---

## **Model Design**

### **Architecture**

- A **transformer** based on the structure explained in [official tensorflow website](https://www.tensorflow.org/text/tutorials/transformer#training_and_checkpointing)

- Experimented with:
  - **Single-shot** approach for direct sentence reconstruction.
  - **Iterative (autoregressive)** approach for token-by-token generation.

### **Parameter Constraints**

- The models were optimized to stay within the **20M parameter** limit.

---

## **Results**

- Validation Accuracy: Maximum validation accuracy of **85.78%**
- Test Accuracy: Average accuracy **55.5%** on the test set. _Note that the scoring function used for the test set differed from that of the validation set_.
- Model size: Approximately **17.5 million parameters**.

---

## **License**

[MIT License](LICENSE).
