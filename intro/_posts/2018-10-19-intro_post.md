---
title : Convolutional Sequence to Sequence Learning
layout : post
author : Heesoo Park
tags : [MT]
---

<h3>Convolutional Sequence to Sequence Learning (arXiv 2017) </h3>


<p>

<b>Jonas Gehring<br/>
Michael Auli<br/>
David Grangier<br/>
Denis Yarats<br/>
Yann N. Dauphin<br/></b>
Facebook AI Research

</p>

<hr />
문단요약
<p>
1. 현재 seq2seq에서 attention을 이용한, bi-directional RNN이 다른 모든 모델을 앞선 상황이다. <br/>
2. sequence modeling 에서 CNN이 가지는 이점 1 : 병렬 처리가 가능하다. <br/>
3. sequence modeling 에서 CNN이 가지는 이점 2 : hierarchical structure는 더 빠른 시간 내에 sequence feature를 계산할 수 있다. <br/>
4. 완전한 CNN 기반의 seq2seq은 RNN의 결과를 뛰어넘지 못한다. <br/>
5. 이 논문에선 전체가 모두 CNN으로만 구성된 모델을 제안한다. 이 때, gated linear unit, residual conntection, attention이 쓰이며, 추가적으로 attention 이 아주 작은 overhead 만을 필요로 하는 것을 보여준다.<br/>
</p>
