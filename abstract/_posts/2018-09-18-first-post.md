---
title : tue_20180918_1
layout : post
tags : [Text_Generation]
---

<h3>Exemplar Encoder-Decoder for Neural Conversation Generation (ACL 2018)</h3>


<p><b>Gaurav Pandey, Danish Contractor, Vineet Kumar and Sachindra Joshi     </b> <br/>
IBM Research AI  <br/>
New Delhi, India  <br/>
<em>{gpandey1, dcontrac, vineeku6, jsachind}@in.ibm.com </em><br/>

<hr />
<p>
Training data 내에 silmilar example 을 통하여 conversation 에서 response 를 생성하는 모델(Exemplar Encoder-Decoder for Neural Conversation Generation). 이때 TF-IDF 를 기반으로 example 을 retrieve 하고 이를 이용해 exemplar vector 를 만든다. Decoder 는 이 벡터에 input context 와의 similarity 이용해 가중치를 준 후 이를 기반으로 response 를 생성한다. 
</p>