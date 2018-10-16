---
title : Topic Aware Neural Response Generation
layout : post
author : Heesoo Park
tags : [Seq2Seq]
---

<h3>Topic Aware Neural Response Generation (AAAI 2017)</h3>


<p>

<b>Chen Xing,<sup>1,2∗</sup> Wei Wu,<sup>4</sup> Yu Wu,<sup>3</sup> Jie Liu,<sup>1,2 †</sup><br/>
Yalou Huang,<sup>1,2</sup> Ming Zhou,<sup>4</sup> Wei-Ying Ma<sup>4</sup></b><br/>
<sup>1</sup>College of Computer and Control Engineering, Nankai University, Tianjin, China<br/>
<sup>2</sup>College of Software, Nankai University, Tianjin, China<br/>
<sup>3</sup>State Key Lab of Software Development Environment, Beihang University, Beijing, China<br/>
<sup>4</sup>Microsoft Research, Beijing, China<br/>
<em>{v-chxing, wuwei, v-wuyu, mingzhou, wyma}@microsoft.com {jliu,huangyl}@nankai.edu.cn</em><br/>




</p>

<hr />
문단요약
<p>
1. 현재 chatbot이 다양한 목적에 맞게 쓰이고 있다. <br/>
2. 기존 chatbot 모델은 MT 모델 위에서 response를 생성하는 학습을 했다. 최근에는 attention 기반의 seq2seq 모델이 response 생성 학습에 많이 이용되고 있다. 하지만 이 모델들은 자연스러운 답변은 하지만 informative 하고 interesting 한 답변을 생성하는데는 실패하고 있다.<br/>
3. 이 논문에선 informative하고 interesting 한 답변을 생성하는 것에 촞ㅁ을 맞춘다. 이전 논문에서 general한 답변에 penalty를 준 방법을 쓴 반면, 이 모델은 답변이 될만한 내용을 topic을 사용하여 가져온다. Input이 주어지면 이를 기반으로 가능한 topic을 구하고 이를 기반으로 답변을 생성한다.<br/>
4. Encoding에서는 message에 대한 hidden vector를 얻는다. 또한 message에서 topic word를 뽑아 embedding vector를 얻는데, 이 topic word는 미리 Twitter dataset으로 학습시킨 LDA를 통해서 구할 수 있다. Decoding에선 Encoding에서 구한 input message를 context vector 하나로 합치고, topic words embedding을 topic vector로 합성한다. 이 때 두 과정에서 모두
attention mechanism을 사용하는데, topic 에 적용할 때에는 mechanism에 약간의 변형을 거친다. 이 두개의 attention을 기반으로 문장을 생성하는데, 이 때 topic word 들에 대해서는 확률값에 bias를 더해주어 그 등장 확률을 높여준다.<br/>
5. 실험은 Baidu Teiba 데이터로 하였고, automatic 하게 평가하는 방법과 사람이 직접 평가하는 방법 두가지를 모두 거쳤다. 이 두개 평가 모두에서 해당 모델이 informative 한 답변을 생성하는 것으로 평가되었다. <br/>
6. 이 논문은 response generation에 topic을 반영하였고, seq2seq에 topic 정보를 자연스럽게 합성하였으며, 실험적으로 이 모델이 잘동작하는 것을 확인하였다.
</p>
