---
title : wed_20180912_3
layout : post
tags : [Image_Generation]
---

<h3>Mode Regularized Generative Adversarial Networks (ICLR 2017)</h3>


<p>
<b><sup>†</sup>Tong Che , <sup>‡</sup>Yanran Li , <sup>†§</sup>Athul Paul Jacob, <sup>†</sup>Yoshua Bengio, <sup>‡</sup>Wenjie Li </b><br/>
†Montreal Institute for Learning Algorithms, Universite de Montr ´ eal, Montr ´ eal, QC H3T 1J4, Canada ´ <br/>
‡Department of Computing, The Hong Kong Polytechnic University, Hong Kong <br/>
§David R. Cheriton School of Computer Science, University Of Waterloo, Waterloo, ON N2L 3G1, Canada <br/>
<em>{tong.che,ap.jacob,yoshua.bengio}@umontreal.ca</em><br/>
<em>{csyli,cswjli}@comp.polyu.edu.hk</em></p>

<hr />
<p>
2018-09-11 주헌이 발표 논문. <br/>


기존 GAN의 약점은 크게 두 가지 이다. <br/>
1) discriminator가 너무 강할 때 학습이 어렵다. 2) Mode collapse 현상이 있다.  <br/>
1)의 경우에는 generator를 auto-encoder의 형태로 만들어 강화시키고, 2) 의 경우에는 real image data에서 sampling을 통해 generator와 discriminator 가 실제 모든 mode에 대해 학습할 수 있도록 한다. <br/>


실제 ABSTRACT 에서는 학습이 잘 되지 않는 이유가 학습된 discriminator의 아주 특별한 functional shape 때문이라고 써있다. 이 shape이 실제 데이터의 분포보다 한 곳에 너무 집중된 분포를 그리게 한다. 이를 정규화 시키는 것이 위의 두가지 방법인듯...
</p>