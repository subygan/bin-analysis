Some datasets with vulnerable codes:


- [devign dataset](https://sites.google.com/view/devign)
- [Juliet dataset](https://samate.nist.gov/SARD/test-suites/112) for test cases in c/c++ 
- [Big vuln dataset](https://dl.acm.org/doi/10.1145/3379597.3387501)
  - Can be run again to scrape more examples of vlunerable code
- [ReVeal dataset](https://github.com/VulDetProject/ReVeal)
  - Contains part of Devign dataset + chrome and debian


  ### Steps:

- Collect data from CVEs and their associated commit histories.
- Isolate benchmarking data from the collected data.
- Test benchmark with ICL, n-shot, and other examples.
- Fine-tune the model on the collected data.
  - Gpt-3.5, [instructions](https://platform.openai.com/docs/guides/fine-tuning/preparing-your-dataset)
  - CodeLLama, [instructions](https://github.com/ragntune/code-llama-finetune/blob/main/fine-tune-code-llama.ipynb)