# **Abstractive Summarization of Indian Legal Text using BART**

This repository focuses on re-implementing the work on **Abstractive Summarization of Indian Legal Text** conducted by Law-AI (IIT Kharagpur). It uses the **BART model** (Bidirectional and Auto-Regressive Transformer) to generate concise summaries for Indian legal documents.

---

## **Objective**

- To replicate the methodology employed by Law-AI for abstractive summarization of Indian legal text.
- To fine-tune the **BART model** for Indian legal text datasets.
- To evaluate and compare performance with the results presented in the original work.(In progress..)

---

## **Features**

- Fine-tuning the BART model for legal text summarization.
- Handling complex and verbose Indian legal language.
- Generating concise abstractive summaries.
- Detailed comparison with Law-AI's implementation.(To be implemented)

---

## **Steps for Implementation**

1. **Data Collection**
   - Datasets of Indian legal documents, processed for training and testing.
   - Preprocessing includes tokenization, formatting, and handling legal jargon.

2. **Model Selection**
   - Fine-tuning the **BART** model using supervised learning for legal text summarization tasks.

3. **Training**
   - The model is trained using cross-entropy loss with GPU acceleration for better performance.

4. **Evaluation**
   - Performance evaluated using:
     - **ROUGE** (Recall-Oriented Understudy for Gisting Evaluation)
     - **BLEU** (BiLingual Evaluation Understudy) (To be implemented)

5. **Comparison with Law-AI Results**
   - Quantitative and qualitative comparisons of generated summaries against the original paper.(To be implemented)

---

## **Tools and Frameworks**

- **Language Models**: BART (via Hugging Face Transformers library)
- **Libraries**: Python (NLTK, SpaCy, PyTorch/TensorFlow)
- **Evaluation**: ROUGE metrics
- **Notebook Environments**: Google Colab for experimentation

---

## **Documentation**

The documentation is provided in the code itself.

#### **Refer to the links for the code:**
- [BART_fineTune-final.ipynb](https://colab.research.google.com/drive/17H_1VZZxeQQiWzCq7ycf-Tpm9SGsm2MF?usp=sharing)  
- [generate_summaries_chunking_BART.ipynb](https://colab.research.google.com/drive/1fxVaC7jWZJp3VDxcFABNLT4-xzHhtpEJ?usp=sharing)

To know more, refer to the file **'NFT_Project'** in the documentation folder.

---

## **References and Resources**

This work is inspired by the original implementation by IIT Kharagpur's **Law-AI**:  
[https://github.com/Law-AI/summarization/tree/aacl](https://github.com/Law-AI/summarization/tree/aacl)

This re-implementation is done for **educational purposes** to learn and understand the techniques of legal text summarization.

### Dataset and Resources
- **IN-Abs Dataset**:  
  Access the dataset, fine-tuned model, and generated summaries:  
  [Google Drive - IN-Abs Dataset](https://drive.google.com/drive/folders/1bu2u8f_1GicMVo1urBSIAeOMSuxct70T?usp=sharing)  
  - **Fine-tuned Model**: Located in the `model` folder.  
  - **Generated Summaries**: Located in the `output` folder.

---

## **Challenges**

- Handling the verbosity and complexity of Indian legal text.
- Overcoming the limited availability of annotated legal datasets.
- Maintaining domain relevance in abstractive summaries.

---

## **Future Work**

- Exploring other transformer models like Pegasus or T5.
- Extending the system to summarize legal documents from other legal systems.
- Investigating transfer learning with domain-specific pre-trained models.

---

### **License**

This project is for educational purposes only and is not intended for commercial use. All credit for the original methodology goes to the **Law-AI** team at IIT Kharagpur.


---

### References

- **Shukla, A. et al.** (2022). _Legal Case Document Summarization: Extractive and Abstractive Methods and their Evaluation_. In: The 2nd Conference of the Asia-Pacific Chapter of the Association for Computational Linguistics and the 12th International Joint Conference on Natural Language Processing.  
  `@inproceedings{shukla2022, title={Legal Case Document Summarization: Extractive and Abstractive Methods and their Evaluation}, author={Shukla, Abhay and Bhattacharya, Paheli and Poddar, Soham and Mukherjee, Rajdeep and Ghosh, Kripabandhu and Goyal, Pawan and Ghosh, Saptarshi}, booktitle={The 2nd Conference of the Asia-Pacific Chapter of the Association for Computational Linguistics and the 12th International Joint Conference on Natural Language Processing}, year={2022}}`

- **Bhattacharya, P. et al.** (2019). _A comparative study of summarization algorithms applied to legal case judgments_. In: European Conference on Information Retrieval, pages 413--428. Springer.  
  `@inproceedings{bhattacharya2019comparative, title={A comparative study of summarization algorithms applied to legal case judgments}, author={Bhattacharya, Paheli and Hiware, Kaustubh and Rajgaria, Subham and Pochhi, Nilay and Ghosh, Kripabandhu and Ghosh, Saptarshi}, booktitle={European Conference on Information Retrieval}, pages={413--428}, year={2019}, organization={Springer}}`
