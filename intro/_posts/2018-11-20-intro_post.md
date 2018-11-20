---
title : Metric Learning from Probabilistic Labels
layout : post
author : Heesoo Park
tags : [Multi_Task_Learning]
---


<h3>Metric Learning from Probabilistic Labels (KDD 2018)</h3>


<p>

<b>Mengdi Huai</b><br/>
State University of New York at<br/>
Buffalo, NY, USA<br/>
<em>mengdihu@buffalo.edu</em><Br/><br/>
<b>Chenglin Miao</b><br/>
State University of New York at<br/>
Buffalo, NY, USA<Br/>
<em>cmiao@buffalo.edu</em><Br/><br/>
<b>Yaliang Li</b><br/>
Tencent Medical AI Lab<br/>
CA, USA<br/>
<em>yaliangli@tencent.com</em><br/><Br/>
<b>Qiuling Suo</b><Br/>
State University of New York at<br/>
Buffalo, NY, USA<br/>
<em>qiulings@buffalo.edu</em><br/><Br/>
<b>Lu Su</b>
State University of New York at<br/>
Buffalo, NY, USA<br/>
<em>lusu@buffalo.edu</em><Br/><Br/>
<b>Aidong Zhang</b><br/>
State University of New York at<br/>
Buffalo, NY, USA<br/>
<em>azhang@buffalo.edu</em>


</p>

<hr />
문단요약
<p>
1. ML technique에서 distance가 갖는 의미 : instance 간의 중요한 relationship을 찾을 수 있다.<br/>
2. 기존의 feature - label pair에서는 label이 deterministic 하게 결정되었지만 실제는 probabilistic하게 존재한다. <br/>
3. Instance-wise probabilistic label : 각각의 instance가 확률적 label을 갖는 경우. 예를 들어, crowdwourcing application, medical diagnosis application 등 <br/>
4. Group-wise probabilistic label : 각각의 group이 구성원들의 비율에 따라 label이 붙는 경우 (instance 각각의 label은 unknown) 예를 들어, political election 결과, epidemic analysis 등<br/>
5. instance-wise data의 label을 probabilistic-> deterministic 으로 바꿀 때 정보 손실이 일어나고, threshold 기반으로 labeling을 할 때, 정확한 threshold를 구하기 어렵다.<br/>
&nbsp;&nbsp;&nbsp;&nbsp; group-wise에서는 probabilistic-> deterministic 으로 변환하는게 불가능하다. <br/>
6. 이 논문에서는 label의 종류에 맞게 두가지 모델 제안 : <br/>
&nbsp;&nbsp;&nbsp; 1) InML(instance-level metric learning) :  확률 기반 label의 ranking을 통해 상대적 찾아내고, 거기에 기반하여 distance constraint를 구축한다. 그 후, optimization 문제로 접근하여 metric을 learning 한다. (large margin framework with hinge loss)<br/>
&nbsp;&nbsp;&nbsp; 2) GrML (group-level metric learning) : 각 그룹 안에서 유사한 instance의 pair 비율 계산한다. 그 후, latent similarity label을 구한다. (???)<br/>
7. 이 논문의 contribution : 1) InML 제안 2) GrML 제안 3) 이론적 분석 및 real-world dataset에서 확장 실험

</p>
