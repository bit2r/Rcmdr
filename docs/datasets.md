---
output: html_document
editor_options: 
  chunk_output_type: console
---
# 데이터셋 / `datasets`

## Prestige - `carData > Prestige`

![](fig/dataset-prestiage-01.png)

![](fig/dataset-prestiage-02.png)


```r
data(Prestige, package="carData")
```

![](fig/dataset-prestiage-03.png)

```r
help("Prestige")
```

carData 패키지에 있는 Prestige 데이터셋을 `.csv`로 저장하여 내보낼 수 있다.

[다운로드](data/Prestige.csv)

참조: [활성 데이터셋 내보내기...](https://rcmdr.tistory.com/52)


## Moore - `carData > Moore`

![](fig/dataset-moore-01.png)

![](fig/dataset-moore-02.png)

```r
data(Moore, package="carData")
```


![](fig/dataset-moore-03.png)


```r
help("Moore")
```

상기 명령 실행을 통해서 `Moore` 데이터셋에 대한 상세 정보를 얻을 수 있다.


<table width="100%"><tr><td>Moore {carData}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>Status, Authoritarianism, and Conformity</h2>

<h3>Description</h3>

<p>The <code>Moore</code> data frame has 45 rows and 4 columns.
The data are for subjects in a social-psychological experiment,
who were faced with manipulated disagreement from a partner of either
of low or high status. The subjects could either conform to the
partner's judgment or stick with their own judgment.
</p>


<h3>Usage</h3>

<pre><code class='language-R'>Moore
</code></pre>


<h3>Format</h3>

<p>This data frame contains the following columns:
</p>

<dl>
<dt>partner.status</dt><dd>
<p>Partner's status.  A factor with levels:
<code>high</code>,
<code>low</code>.
</p>
</dd>
<dt>conformity</dt><dd>
<p>Number of conforming responses in 40 critical trials.
</p>
</dd>
<dt>fcategory</dt><dd>
<p>F-Scale Categorized.
A factor with levels (note levels out of order):
<code>high</code>,
<code>low</code>,
<code>medium</code>.
</p>
</dd>
<dt>fscore</dt><dd>
<p>Authoritarianism: F-Scale score.
</p>
</dd>
</dl>



<h3>Source</h3>

<p>Moore, J. C., Jr. and Krupat, E. (1971) 
Relationship between source status, authoritarianism and conformity in a
social setting. <em>Sociometry</em> <b>34</b>, 122&ndash;134.  
</p>
<p>Personal communication
from J. Moore, Department of Sociology, York University.
</p>


<h3>References</h3>

<p>Fox, J. (2016)
<em>Applied Regression Analysis and Generalized Linear Models</em>,
Third Edition. Sage.  
</p>
<p>Fox, J. and Weisberg, S. (2019) 
<em>An R Companion to Applied Regression</em>, Third Edition, Sage.
</p>

<hr /><div style="text-align: center;">[Package <em>carData</em> version 3.0-5 <a href="00Index.html">Index</a>]</div>
</div>


## OBrienKaiser - `carData > OBrienKaiser`

`carData` 패키지에 있는  `OBrienKaiser` 데이터셋이다. `carData` 패키지는 `Rcmdr` 패키지가 호출될 때 자동으로 함께 호출되기 때문에 **R Commander**에서 `carData` 패키지에 포함된 데이터셋들을 자유롭게 호출할 수 있다. 

[Read data set from an attached package...](https://rcmdr.kr/37)

OBrienKaiser 데이터셋은 R Commander에서 활성 데이터셋으로 이용할 수 있다. 그러나 '통계 > 요약 > 활성데이터셋' 기능은 사용할 수 없다. 다음과 같은 오류문을 Rgui 창에서 보게된다.

 
> Error in sprintf(gettextRcmdr("There are %d variables in the data set %s.\nDo you want to proceed?"),  : 
>  '%d'는 유효하지 않은 포맷입니다; 문자형 객체들에는 포맷 %s를 사용해주세요


입력창에 str(OBrienKaiser) 함수를 입력하고 실행하여 OBrienKaiser 데이터셋의 구조를 살펴보자.

![](fig/dataset-obrien-01.png)

입력창에 `summary(OBrienKaiser)` 함수를 입력하고 실행하여 요약 정보를 살펴보자.

![](fig/dataset-obrien-02.png)


<table width="100%"><tr><td>OBrienKaiser {carData}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>O'Brien and Kaiser's Repeated-Measures Data</h2>

<h3>Description</h3>

<p>These contrived repeated-measures data are taken from 
O'Brien and Kaiser (1985). The data are from an imaginary study in which
16 female and male subjects, who are divided into three treatments, are measured
at a pretest, postest, and a follow-up session; during each session, they are
measured at five occasions at intervals of one hour. The design, therefore, has
two between-subject and two within-subject factors.
</p>
<p>The contrasts for the <code>treatment</code> factor are set to <code class="reqn">-2, 1, 1</code> and
<code class="reqn">0, -1, 1</code>. The contrasts for the <code>gender</code> factor are set to
<code>contr.sum</code>.
</p>


<h3>Usage</h3>

<pre><code class='language-R'>OBrienKaiser</code></pre>


<h3>Format</h3>

<p>A data frame with 16 observations on the following 17 variables.
</p>

<dl>
<dt><code>treatment</code></dt><dd><p>a factor with levels <code>control</code> <code>A</code> <code>B</code></p>
</dd>
<dt><code>gender</code></dt><dd><p>a factor with levels <code>F</code> <code>M</code></p>
</dd>
<dt><code>pre.1</code></dt><dd><p>pretest, hour 1</p>
</dd>
<dt><code>pre.2</code></dt><dd><p>pretest, hour 2</p>
</dd>
<dt><code>pre.3</code></dt><dd><p>pretest, hour 3</p>
</dd>
<dt><code>pre.4</code></dt><dd><p>pretest, hour 4</p>
</dd>
<dt><code>pre.5</code></dt><dd><p>pretest, hour 5</p>
</dd>
<dt><code>post.1</code></dt><dd><p>posttest, hour 1</p>
</dd>
<dt><code>post.2</code></dt><dd><p>posttest, hour 2</p>
</dd>
<dt><code>post.3</code></dt><dd><p>posttest, hour 3</p>
</dd>
<dt><code>post.4</code></dt><dd><p>posttest, hour 4</p>
</dd>
<dt><code>post.5</code></dt><dd><p>posttest, hour 5</p>
</dd>
<dt><code>fup.1</code></dt><dd><p>follow-up, hour 1</p>
</dd>
<dt><code>fup.2</code></dt><dd><p>follow-up, hour 2</p>
</dd>
<dt><code>fup.3</code></dt><dd><p>follow-up, hour 3</p>
</dd>
<dt><code>fup.4</code></dt><dd><p>follow-up, hour 4</p>
</dd>
<dt><code>fup.5</code></dt><dd><p>follow-up, hour 5</p>
</dd>
</dl>



<h3>Source</h3>

<p>O'Brien, R. G., and Kaiser, M. K. (1985)
MANOVA method for analyzing repeated measures designs: An extensive primer.
<em>Psychological Bulletin</em> <b>97</b>, 316&ndash;333, Table 7.
</p>


<h3>Examples</h3>

<pre><code class='language-R'>OBrienKaiser
contrasts(OBrienKaiser$treatment)
contrasts(OBrienKaiser$gender)
</code></pre>

<hr /><div style="text-align: center;">[Package <em>carData</em> version 3.0-5 <a href="00Index.html">Index</a>]</div>
</div>

