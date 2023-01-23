<!---
Copyright 2022 IBM Corp.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

<h3 align="center">
    <img width="350" alt="primeqa" src="docs/_static/img/PrimeQA.png">
    <p>The Prime Repository for State-of-the-Art Multilingual Question Answering Research and Development.</p>
</h3>

![Build Status](https://github.com/primeqa/primeqa/actions/workflows/primeqa-ci.yml/badge.svg)
[![LICENSE|Apache2.0](https://img.shields.io/github/license/saltstack/salt?color=blue)](https://www.apache.org/licenses/LICENSE-2.0.txt)
[![sphinx-doc-build](https://github.com/primeqa/primeqa/actions/workflows/sphinx-doc-build.yml/badge.svg)](https://github.com/primeqa/primeqa/actions/workflows/sphinx-doc-build.yml)   

PrimeQA is a public open source repository that enables researchers and developers to train state-of-the-art models for question answering (QA). By using PrimeQA, a researcher can replicate the experiments outlined in a paper published in the latest NLP conference while also enjoying the capability to download pre-trained models (from an online repository) and run them on their own custom data. PrimeQA is built on top of the [Transformers](https://github.com/huggingface/transformers) toolkit and uses [datasets](https://huggingface.co/datasets/viewer/) and [models](https://huggingface.co/PrimeQA) that are directly downloadable.


The models within PrimeQA supports End-to-end Question Answering. PrimeQA answers questions via 
- [Information Retrieval](https://github.com/primeqa/primeqa/tree/main/primeqa/ir): Retrieving documents and passages using both traditional (e.g. BM25) and neural (e.g. ColBERT) models
- [Multilingual Machine Reading Comprehension](https://huggingface.co/ibm/tydiqa-primary-task-xlm-roberta-large): Extract and/ or generate answers given the source document or passage.
- [Multilingual Question Generation](https://huggingface.co/PrimeQA/mt5-base-tydi-question-generator): Supports generation of questions for effective domain adaptation over [tables](https://huggingface.co/PrimeQA/t5-base-table-question-generator) and [multilingual text](https://huggingface.co/PrimeQA/mt5-base-tydi-question-generator).
