<img src="https://github.com/HECTA-UoM/ClinicalNMT/blob/main/ClinicalNMT_logo.png" width="300">


# ClinicalNMT
Clinical NMT Projects and Related Resources

# Presentations
ClinicalNLP2023 https://clinical-nlp.github.io/2023/program.html @ ACL2023 https://virtual2023.aclweb.org/paper_ClinicalNLP_6.html
[PPT](https://github.com/HECTA-UoM/ClinicalNMT/blob/main/ClinicalNLP2023_ppt.pptx.pdf)

WMT2022 https://www.statmt.org/wmt22/papers.html @ EMNLP2022 https://2022.emnlp.org/program/workshops/


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

The following work is accepted to 5th ClinicalNLP WS@ACL2023
@misc{han2023investigating,
      title={Investigating Massive Multilingual Pre-Trained Machine Translation Models for Clinical Domain via Transfer Learning}, 
      author={Lifeng Han and Gleb Erofeev and Irina Sorokina and Serge Gladkoff and Goran Nenadic},
      year={2023},
      eprint={2210.06068},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
