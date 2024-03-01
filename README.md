<img src="https://github.com/HECTA-UoM/ClinicalNMT/blob/main/ClinicalNMT_logo.png" width="300">


# ClinicalNMT
Clinical Neural Machine Translation Projects: data, resources, and models for research sharing.


# Presentations
OpenNLP club 2024 https://youtu.be/RudrQQIMAS0 [PPT](https://docs.google.com/presentation/d/1RWGS5sUmJ6xX1asH3sik9w7Dk7J1Rmrt/edit?usp=sharing&ouid=112530642263849099949&rtpof=true&sd=true)| 
ClinicalNLP2023 https://clinical-nlp.github.io/2023/program.html @ ACL2023 https://virtual2023.aclweb.org/paper_ClinicalNLP_6.html | 
[PPT](https://github.com/HECTA-UoM/ClinicalNMT/blob/main/ClinicalNLP2023_ppt.pptx.pdf) |[paper](https://aclanthology.org/2023.clinicalnlp-1.5.pdf)

WMT2022 https://www.statmt.org/wmt22/papers.html @ EMNLP2022 https://2022.emnlp.org/program/workshops/ | [Poster](https://github.com/HECTA-UoM/ClinicalNMT/blob/main/WMT22_poster_Han_etal.pdf)

# New Pre-print on our [ClinicalNMT findings](https://arxiv.org/abs/2312.07250)- Accepted by [Frontiers in Digital Health](https://www.frontiersin.org/journals/digital-health/articles/10.3389/fdgth.2024.1211564/abstract)
Original Research Article in collections of Healthcare Text Analytics: Unlocking the Evidence from Free Text, Volume III

@misc{han2023neural,
      title={Neural Machine Translation of Clinical Text: An Empirical Investigation into Multilingual Pre-Trained Language Models and Transfer-Learning}, 
      author={Lifeng Han and Serge Gladkoff and Gleb Erofeev and Irina Sorokina and Betty Galiano and Goran Nenadic},
      year={2023},
      eprint={2312.07250},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}


# resources
The dataset used is available for research purposes, please contact: Serge Gladkoff, CEO, Logrus Global (https://logrusglobal.com/)

Models investigated: MarianNMT, NLLB, WMT21fb (model links in our [paper](https://doi.org/10.3389/fdgth.2024.1211564) )


#  References

@inproceedings{han-etal-2022-examining,
    title = "Examining Large Pre-Trained Language Models for Machine Translation: What You Don{'}t Know about It",
    author = "Han, Lifeng  and
      Erofeev, Gleb  and
      Sorokina, Irina  and
      Gladkoff, Serge  and
      Nenadic, Goran",
    booktitle = "Proceedings of the Seventh Conference on Machine Translation (WMT)",
    month = dec,
    year = "2022",
    address = "Abu Dhabi, United Arab Emirates (Hybrid)",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.wmt-1.84",
    pages = "908--919",
    abstract = "Pre-trained language models (PLMs) often take advantage of the monolingual and multilingual dataset that is freely available online to acquire general or mixed domain knowledge before deployment into specific tasks. Extra-large PLMs (xLPLMs) are proposed very recently to claim supreme performances over smaller-sized PLMs such as in machine translation (MT) tasks. These xLPLMs include Meta-AI{'}s wmt21-dense-24-wide-en-X (2021) and NLLB (2022). In this work, we examine if xLPLMs are absolutely superior to smaller-sized PLMs in fine-tuning toward domain-specific MTs. We use two different in-domain data of different sizes: commercial automotive in-house data and clinical shared task data from the ClinSpEn2022 challenge at WMT2022. We choose the popular Marian Helsinki as smaller sized PLM and two massive-sized Mega-Transformers from Meta-AI as xLPLMs.Our experimental investigation shows that 1) on smaller-sized in-domain commercial automotive data, xLPLM wmt21-dense-24-wide-en-X indeed shows much better evaluation scores using SacreBLEU and hLEPOR metrics than smaller-sized Marian, even though its score increase rate is lower than Marian after fine-tuning; 2) on relatively larger-size well prepared clinical data fine-tuning, the xLPLM NLLB tends to lose its advantage over smaller-sized Marian on two sub-tasks (clinical terms and ontology concepts) using ClinSpEn offered metrics METEOR, COMET, and ROUGE-L, and totally lost to Marian on Task-1 (clinical cases) on all official metrics including SacreBLEU and BLEU; 3) metrics do not always agree with each other on the same tasks using the same model outputs; 4) clinic-Marian ranked No.2 on Task- 1 (via SacreBLEU/BLEU) and Task-3 (via METEOR and ROUGE) among all submissions.",
}


@inproceedings{han-etal-2023-investigating,
    title = "Investigating Massive Multilingual Pre-Trained Machine Translation Models for Clinical Domain via Transfer Learning",
    author = "Han, Lifeng  and
      Erofeev, Gleb  and
      Sorokina, Irina  and
      Gladkoff, Serge  and
      Nenadic, Goran",
    editor = "Naumann, Tristan  and
      Ben Abacha, Asma  and
      Bethard, Steven  and
      Roberts, Kirk  and
      Rumshisky, Anna",
    booktitle = "Proceedings of the 5th Clinical Natural Language Processing Workshop",
    month = jul,
    year = "2023",
    address = "Toronto, Canada",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2023.clinicalnlp-1.5",
    doi = "10.18653/v1/2023.clinicalnlp-1.5",
    pages = "31--40",
    abstract = "Massively multilingual pre-trained language models (MMPLMs) are developed in recent years demonstrating superpowers and the pre-knowledge they acquire for downstream tasks. This work investigates whether MMPLMs can be applied to clinical domain machine translation (MT) towards entirely unseen languages via transfer learning. We carry out an experimental investigation using Meta-AI{'}s MMPLMs {``}wmt21-dense-24-wide-en-X and X-en (WMT21fb){''} which were pre-trained on 7 language pairs and 14 translation directions including English to Czech, German, Hausa, Icelandic, Japanese, Russian, and Chinese, and the opposite direction. We fine-tune these MMPLMs towards English-\textit{Spanish} language pair which \textit{did not exist at all} in their original pre-trained corpora both implicitly and explicitly.We prepare carefully aligned \textit{clinical} domain data for this fine-tuning, which is different from their original mixed domain knowledge.Our experimental result shows that the fine-tuning is very successful using just 250k well-aligned in-domain EN-ES segments for three sub-task translation testings: clinical cases, clinical terms, and ontology concepts. It achieves very close evaluation scores to another MMPLM NLLB from Meta-AI, which included Spanish as a high-resource setting in the pre-training.To the best of our knowledge, this is the first work on using MMPLMs towards \textit{clinical domain transfer-learning NMT} successfully for totally unseen languages during pre-training.",
}
