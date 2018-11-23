---
title : fri_20181123_3
layout : post
author : Heesoo Park
tags : [Analysis_Neural_Net]
---

<h3>BEYOND WORD IMPORTANCE: CONTEXTUAL DECOMPOSITION
TO EXTRACT INTERACTIONS FROM LSTMS (ICLR 2018)</h3>


<p>

<b>W. James Murdoch </b><Br/>
Department of Statistics<br/>
University of California, Berkeley<br/>
<em>jmurdoch@berkeley.edu</em><br/><br/>
<b>Peter J. Liu</b><br/>
Google Brain<br/>
Mountain View, CA<br/><br/>
<b>Bin Yu</b><br/>
Department of Statistics<br/>
Department of EECS<br/>
University of California, Berkeley<br/>


</p>

<hr />
문단요약
<p>
1. 기존의 language model은 joint probability의 factorization에 기반을 둠. <br/>
2. RNN 기반의 lauguage model을 설명. 이 때 dot product와 softmax의 조합이 과연 conditional probability를 표현하는데 적합한지에 대한 의문이 있음을 지적 <br/>
3. 이 논문에선, Softmax 기반 RNN이 정확히 matrix factorization 문제와 일치함을 보이고 특히 이때 high rank- matrix factorization과 일치함을 보인다. 그리고 이것은 softmax의 capacity가 충분치 않음을 보여준다. (Softmax-bottleneck)<br/>
4. 이 논문에서 softmax bottleneck을 유도하는 과정은 3단계이다. <br/>
&nbsp;&nbsp;&nbsp;&nbsp; 1) RNN에 discrete latent variable을 도입. <br/>
&nbsp;&nbsp;&nbsp;&nbsp; 2) Mixture of Softmax (MoS)로 다음 token의 확률을 나타냄 <br/>
&nbsp;&nbsp;&nbsp;&nbsp; 3) MoS가 larger normalized singular value와 일치하며 따라서 softmax보다 더 큰 capacity가 필요함을 보인다. <br/>
5. 이 논문에선 perplexity와 dialogue task를 통해 성능을 입증한다. <br/>
6. 이 논문의 contribution은 1) softmax bottleneck을 입증, 2) 이를 극복하는 새로운 방법 제안이다.

</p>
