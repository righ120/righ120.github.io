---
title : UNSUPERVISED NEURAL MACHINE TRANSLATION
layout : post
author : Heesoo Park
tags : [MT]
---

<h3>UNSUPERVISED NEURAL MACHINE TRANSLATION (ICLR 2018)</h3>


<p>

<b>Mikel Artetxe, Gorka Labaka & Eneko Agirre</b><br/>
IXA NLP Group<br/>
University of the Basque Country (UPV/EHU)<br/>
<em>{mikel.artetxe,gorka.labaka,e.agirre}@ehu.eus</em><br/>
<b>Kyunghyun Cho</b><br/>
New York University<br/>
CIFAR Azrieli Global Scholar<br/>
<em>kyunghyun.cho@nyu.edu</em><br/>

</p>

<hr />
문단요약
<p>
1. NMT가 SMT에 비해 큰 성능 향상을 가져옴 <br/>
2. NMT에선 parallel corpora가 필수적인데, 이 dataset은 아주 부족하다. 이를 해결학 위한 기존 방법들은 cross-lingual signal을 필요로 한다.<br/>
3. 이 논문에선 cross-lingual info가 필요가 없는, 오직 mono-lingual dataset에서만 학습이 가능한 모델을 제안한다. 이때, cross-lingual embedding을 기반으로 학습을 시켜, encoder가 양방향으로 학습을 할 수 있게 된다. 여기에, token swap 형태의 noise를 추가하고, 또한 backtranslation을 이용해 성능을 향상시킨다.<br/>
4. 실험을 통해, 최신 모델들보다 성능이 좋게 나오는 것을 확인하였다. <br/>
5. 각 섹션에 대해 설명한다.<br/>
</p>
