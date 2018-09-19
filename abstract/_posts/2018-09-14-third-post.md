---
title : fri_20180914_3
layout : post
tags : [Text_Generation]
---

<h3>Deep Reinforceent Learning for Dialogue Generation (EMNLP 2016)</h3>


<p><b>Jiwei Li1 , Will Monroe1 , Alan Ritter<sup>2</sup> , Michel Galley<sup>3</sup> , Jianfeng Gao<sup>3</sup> and Dan Jurafsky<sup>1</sup>    </b> <br/>
<sup>1</sup>Stanford University, Stanford, CA, USA <br/>
<sup>2</sup>Ohio State University, OH, USA <br/>
<sup>3</sup>Microsoft Research, Redmond, WA, USA  <br/>
<em>{jiweil,wmonroe4,jurafsky}@stanford.edu, ritter.1492@osu.edu </em><br/>
<em>{mgalley,jfgao}@microsoft.com</em> <br/>

<hr />
<p>
Forward-looking function으로 future direction을 고려하여 dialogue를 생성한다. RL을 사용하여 2개의 가상 에이전트가 policy gradient를 통해 대화를 나누는 것을 simulation하며 학습한다. Reward는 3개의 대화 요소에 부여한다. : informativity, coherence, ease of answering
</p>