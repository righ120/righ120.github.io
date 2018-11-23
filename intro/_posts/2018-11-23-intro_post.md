---
title : BEYOND WORD IMPORTANCE  CONTEXTUAL DECOMPOSITION TO EXTRACT INTERACTIONS FROM LSTMS
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
1. 최근 data 간의 non-linearty를 학습하는 모델들은 해석이 불가능하여 black box로 남아있다. (대표적으로 LSTMs) <br/>
2. 이 논문에선, LSTM 모델에서 어떤 변경도 없이, 각 step에서 어떤 부분이 최종 prediction에 기여하는지 contextual decomposition (CD)를 통해 분석한다. 이 때, 기여하는 부분이 어떤 단어들인지 찾아낼 뿐만 아니라, 이들 단어들이 어떻게 결합하여 기여하는지 또한 찾아낸다.<br/>
3. 이를 실험을 통해 입증하였으며, 같은 data에서 기존 방법들이 잘 동작하지 않는 것도 확인하였다.
</p>
