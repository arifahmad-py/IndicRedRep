# Looks can be Deceptive: Distinguishing Repetition Disfluency from Reduplication

This repository provides all supporting materials (data, code, and instructions) for our COLING 2025 paper *"Looks can be Deceptive: Distinguishing Repetition Disfluency from Reduplication"*. In this work, we introduce the **IndicRedRep** dataset, consisting of Hindi, Telugu, and Marathi speech transcripts annotated at the word-level for reduplication and repetition. We propose a sequence labeling framework enhanced by the Reparandum-Interregnum-Repair (RiR) structure to accurately distinguish morphological reduplication from disfluent repetition.

**Paper Link:** [Looks can be Deceptive: Distinguishing Repetition Disfluency from Reduplication](https://arxiv.org/abs/2407.08147)]

## 1. Overview

**Reduplication** is a morphological phenomenon involving the repetition of a whole word or part of it to signal grammatical, semantic, or pragmatic nuances, such as plurality or emphasis.

**Repetition** is a speech disfluency where a speaker unintentionally repeats words or phrases, often due to cognitive hesitation or uncertainty.

**Key Contribution:**  
Our work is the first to provide a large-scale, publicly available dataset—**IndicRedRep**—labeled at the token-level for both reduplication and repetition. We also introduce a novel approach that leverages the RiR structure to substantially improve classification accuracy, even in challenging scenarios where both phenomena co-occur.

## 2. Dataset

**IndicRedRep** comprises three subsets:  
- **Hindi**: ~4.5K sentences (derived from the GramVaani Corpus)  
- **Telugu**: ~1.6K sentences (synthetically generated and manually validated)  
- **Marathi**: ~1.6K sentences (synthetically generated and manually validated)

Each sentence in IndicRedRep is annotated at the token-level with three possible labels:  
- `B/I-Red` for reduplication  
- `B/I-Rep` for repetition  
- `O` for non-reduplicative, non-disfluent words

The dataset is split into training, validation, and test sets using an 80:10:10 ratio. Further details on dataset statistics can be found in our paper and the accompanying data folder.

## 3. Acknowledgements & License

**License:**  
The IndicRedRep dataset: CC BY-NC 4.0  
Code Implementation: MIT License

**Acknowledgements:**  
We thank the authors of baseline models whose code we adapted. We also acknowledge the support of the Bhashini project, Ministry of Electronics and Information Technology (MeitY), Government of India, and our native language annotators for their invaluable assistance.

## 4. Citation

If you find IndicRedRep or our approach useful in your research, please cite our COLING 2025 paper:

```
@misc{ahmad2024looksdeceptivedistinguishingrepetition,
      title={Looks can be Deceptive: Distinguishing Repetition Disfluency from Reduplication}, 
      author={Arif Ahmad and Mothika Gayathri Khyathi and Pushpak Bhattacharyya},
      year={2024},
      eprint={2407.08147},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2407.08147}, 
}
```
