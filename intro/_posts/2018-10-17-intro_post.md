---
title : BERT Pre-training of Deep Bidirectional Transformers for Language Understanding
layout : post
author : Heesoo Park
tags : [Seq2Seq]
---

<h3>BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding (arXiv 2018)</h3>


<p>

<b>Jacob Devlin Ming-Wei Chang Kenton Lee Kristina Toutanova</b><br/>
Google AI Language<br/>
<em>{jacobdevlin,mingweichang,kentonl,kristout}@google.com</em><br/>



</p>

<hr />
문단요약
<p>
1. pre-training은 다양한 NLP task의 성능 향상에 유용하게 쓰인다.<br/>
2. 기존에는 두가지 방법으로 pre-training을 시킨 representation을 적용시켜왔다. 하나는 feature-based로 모델 구조를 task-specific 하게 변형 후, pre-trained representation을 부가 정보로 이용하는 방법이다. 또다른 하나는 task-specific한 부분을 최소화하고, 
pre-trained 된 parameter를 fine-tuning 만 한다. 이때, 이 두가지 방법 모두 unidirection 으로만 pre-training을 시켜왔다.<br/>
3. Unidirection한 방법은 token 단위로 적용되는 NLP task에서는 치명적인 한계를 가진다.<br/>
4. 이 논문에선 "masked language model" 이라는 새 pre-training objective function을 제안한다. 이 function은 input의 token을 랜덤하게 masking 하고, 이 masked 된 단어들을 주변 단어에 기반하여 복원하도록 한다. 이때 양 옆 주변 단어를 모두 고려하기 때문에 bidirectional 하게 pre-training을 시킬 수 있다. 또한 sentence 단위의 pre-training 방법인 "next sentence prediction" 방법도 제안한다. <br/>
5. 이 논문의 3가지 컨트리뷰션이 있다. 첫번째는 bidirectional pre-training 방법을 제안한 것이고, 두번째는 fine-tuning 방법으로 pre-trained representation을 적용하여 task-specific 한 구조를 만드는데 필요한 노력을 단축할 수 있다는 것이고, 세번째는 이 모델을 통해 11개의 최신 nlp task 결과를 모두 앞질렀다는 것이다.
</p>
