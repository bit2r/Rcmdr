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


<table width="100%" summary="page for Moore {carData}"><tr><td>Moore {carData}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>Status, Authoritarianism, and Conformity</h2>

<h3>Description</h3>

<p>The <code>Moore</code> data frame has 45 rows and 4 columns.
The data are for subjects in a social-psychological experiment,
who were faced with manipulated disagreement from a partner of either
of low or high status. The subjects could either conform to the
partner's judgment or stick with their own judgment.
</p>


<h3>Usage</h3>

<pre>
Moore
</pre>


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


<table width="100%" summary="page for OBrienKaiser {carData}"><tr><td>OBrienKaiser {carData}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>O'Brien and Kaiser's Repeated-Measures Data</h2>

<h3>Description</h3>

<p>These contrived repeated-measures data are taken from 
O'Brien and Kaiser (1985). The data are from an imaginary study in which
16 female and male subjects, who are divided into three treatments, are measured
at a pretest, postest, and a follow-up session; during each session, they are
measured at five occasions at intervals of one hour. The design, therefore, has
two between-subject and two within-subject factors.
</p>
<p>The contrasts for the <code>treatment</code> factor are set to <i>-2, 1, 1</i> and
<i>0, -1, 1</i>. The contrasts for the <code>gender</code> factor are set to
<code>contr.sum</code>.
</p>


<h3>Usage</h3>

<pre>OBrienKaiser</pre>


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

<pre>
OBrienKaiser
contrasts(OBrienKaiser$treatment)
contrasts(OBrienKaiser$gender)
</pre>

<hr /><div style="text-align: center;">[Package <em>carData</em> version 3.0-5 <a href="00Index.html">Index</a>]</div>


## OBrienKaiserLong - `carData > OBrienKaiserLong`

`OBrienKaiserLong` 데이터셋은 `carData` 패키지에 포함되어 있다. 
`carData` 패키지는 `Rcmdr` 패키지가 호출될 때 자동으로 함께 호출되기 때문에, `OBrienKaiserLong` 데이터셋을 R Commander에서 메뉴기능을 통해서 활성데이터셋으로 불러올 수 있다.

통계> 요약 > 활성 데이터셋 메뉴를 통하여 OBrienKaiserLong  데이터셋의 요약정보를 확인할 수 있다.


![Windows 사례](fig/dataset-obrienlong-01.png)

`summary()` 함수를 이용한 것을 알 수 있다.

![Windows 사례](fig/dataset-obrienlong-02.png)



`str()` 함수를 활용하여 입력창에 직접 `str(OBrienKaiserLong)`을 입력하고 실행하여, 출력창에 다음과 같이 `OBrienKaiserLong` 데이터셋의 구조적 정보도 확인할 수 있다.


![Windows 사례](fig/dataset-obrienlong-03.png)

R Commander 화면에서 <데이터셋 보기> 버튼을 누르면 다음과 같은 내부 구성을 볼 수 있다:

![Linux 사례 (Ubuntu 18.04)](fig/dataset-obrienlong-04.png)


```r
head(OBrienKaiserLong, 1) # first subject
```



<table width="100%" summary="page for OBrienKaiserLong {carData}"><tr><td>OBrienKaiserLong {carData}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>O'Brien and Kaiser's Repeated-Measures Data in &quot;Long&quot; Format</h2>

<h3>Description</h3>

<p>Contrived repeated-measures data from O'Brien and Kaiser (1985). For details see <code><a href="../../carData/help/OBrienKaiser.html">OBrienKaiser</a></code>, which is for the &quot;wide&quot; form of the same data.</p>


<h3>Usage</h3>

<pre>OBrienKaiserLong</pre>


<h3>Format</h3>

<p>A data frame with 240 observations on the following 6 variables.
</p>

<dl>
<dt><code>treatment</code></dt><dd><p>a between-subjects factor with levels <code>control</code>, <code>A</code>, <code>B</code>.</p>
</dd>
<dt><code>gender</code></dt><dd><p>a between-subjects factor with levels <code>F</code>, <code>M.</code></p>
</dd>
<dt><code>score</code></dt><dd><p>the numeric response variable.</p>
</dd>
<dt><code>id</code></dt><dd><p>the subject id number.</p>
</dd>
<dt><code>phase</code></dt><dd><p>a within-subjects factor with levels <code>pre</code>, <code>post</code>, <code>fup</code>.</p>
</dd>
<dt><code>hour</code></dt><dd><p>a within-subjects factor with levels <code>1</code>, <code>2</code>, <code>3</code>, <code>4</code>, <code>5</code>.</p>
</dd>
</dl>



<h3>Source</h3>

<p>O'Brien, R. G., and Kaiser, M. K. (1985)
MANOVA method for analyzing repeated measures designs: An extensive primer.
<em>Psychological Bulletin</em> <b>97</b>, 316&ndash;333, Table 7.
</p>


<h3>See Also</h3>

<p><code><a href="../../carData/help/OBrienKaiser.html">OBrienKaiser</a></code>.</p>


<h3>Examples</h3>

<pre>
head(OBrienKaiserLong, 15) # first subject
</pre>

<hr /><div style="text-align: center;">[Package <em>carData</em> version 3.0-5 <a href="00Index.html">Index</a>]</div>


## airquality - `datasets > airquality`

![Linux 사례 (MX 21)](fig/dataset-airquality-01.png)

R이 시작될 때, datasets 패키지가 자동으로 호출된다. 따라서 R Commander를 실행할 때, datasets 패키지는 첨부 패키지화되어 메뉴창을 통해서 내부 데이터셋을 찾고 불러올 수 있다.

메뉴창에서 순서대로 데이터 > 패키지에 있는 데이터 > 첨부된 패키지에서 데이터셋 읽기... 를 선택하면 다음과 같은 창이 등장한다.

![Windows 사례](fig/dataset-airquality-02.png)


출력창을 보면, airquality라는 데이터셋에는 6개의 변수가 있고, 각 변수는 수치형 정보를 담고 있다.

![Windows 사례](fig/dataset-airquality-03.png)

Month 변수는 최소 5에서 최대 9로 값이 있는데, 정확히는 5월부터 9월까지일 것이다. 한달 한달을 뜻하는 월(month)은 5월이 9월보다 크다고 할 수 없고, 5월, 6월, 7월, 8월, 9월 등으로 개체화되어 분리된다. 다시 말하면, 요인형 변수가 되어야 한다는 뜻이다.

그럼 왜, airqualty 데이터셋의 Month 변수는 수치형으로 되어 있을까. 원자료를 R의 데이터셋으로 불러오는 과정에서 해당 변수의 요인화과정이 생략되었을 것이다.


<table width="100%" summary="page for airquality {datasets}"><tr><td>airquality {datasets}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>New York Air Quality Measurements</h2>

<h3>Description</h3>

<p>Daily air quality measurements in New York, May to September 1973.
</p>


<h3>Usage</h3>

<pre>airquality</pre>


<h3>Format</h3>

<p>A data frame with 153 observations on 6 variables.
</p>

<table summary="Rd table">
<tr>
 <td style="text-align: right;">
    <code>[,1]</code> </td><td style="text-align: left;"> <code>Ozone</code>   </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> Ozone (ppb)</td>
</tr>
<tr>
 <td style="text-align: right;">
    <code>[,2]</code> </td><td style="text-align: left;"> <code>Solar.R</code> </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> Solar R (lang)</td>
</tr>
<tr>
 <td style="text-align: right;">
    <code>[,3]</code> </td><td style="text-align: left;"> <code>Wind</code>    </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> Wind (mph)</td>
</tr>
<tr>
 <td style="text-align: right;">
    <code>[,4]</code> </td><td style="text-align: left;"> <code>Temp</code>    </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> Temperature (degrees F)</td>
</tr>
<tr>
 <td style="text-align: right;">
    <code>[,5]</code> </td><td style="text-align: left;"> <code>Month</code>   </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> Month (1--12)</td>
</tr>
<tr>
 <td style="text-align: right;">
    <code>[,6]</code> </td><td style="text-align: left;"> <code>Day</code>     </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> Day of month (1--31)
  </td>
</tr>

</table>



<h3>Details</h3>

<p>Daily readings of the following air quality values for May 1, 1973 (a
Tuesday) to September 30, 1973.
</p>

<ul>
<li> <p><code>Ozone</code>: Mean ozone in parts per
billion from 1300 to 1500 hours at Roosevelt Island
</p>
</li>
<li> <p><code>Solar.R</code>: Solar radiation
in Langleys in the frequency band 4000&ndash;7700 Angstroms from
0800 to 1200 hours at Central Park
</p>
</li>
<li> <p><code>Wind</code>: Average wind speed in miles
per hour at 0700 and 1000 hours at LaGuardia Airport
</p>
</li>
<li> <p><code>Temp</code>: Maximum daily
temperature in degrees Fahrenheit at La Guardia Airport.
</p>
</li></ul>



<h3>Source</h3>

<p>The data were obtained from the New York State Department of
Conservation (ozone data) and the National Weather Service
(meteorological data).
</p>


<h3>References</h3>

<p>Chambers, J. M., Cleveland, W. S., Kleiner, B. and Tukey, P. A. (1983)
<em>Graphical Methods for Data Analysis</em>.
Belmont, CA: Wadsworth.
</p>


<h3>Examples</h3>

<pre>
require(graphics)
pairs(airquality, panel = panel.smooth, main = "airquality data")
</pre>

<hr /><div style="text-align: center;">[Package <em>datasets</em> version 4.1.3 <a href="00Index.html">Index</a>]</div>


## Bfox - `carData > Bfox`

![Linux 사례 (MX 21)](fig/dataset-bfox-01.png)

![Linux 사례 (MX 21)](fig/dataset-bfox-02.png)


```r
data(Bfox, package="carData")
```


Bfox 데이터셋이 활성화되었다면, 도움말 기능을 통하여 데이터셋의 정보를 확인할 수 있다.

![Linux 사례 (MX 21)](fig/dataset-bfox-03.png)

<table width="100%" summary="page for Bfox {carData}"><tr><td>Bfox {carData}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>Canadian Women's Labour-Force Participation</h2>

<h3>Description</h3>

<p>The <code>Bfox</code> data frame has 30 rows and 7 columns.
Time-series data on Canadian women's labor-force participation,
1946&ndash;1975.
</p>


<h3>Usage</h3>

<pre>
Bfox
</pre>


<h3>Format</h3>

<p>This data frame contains the following columns:
</p>

<dl>
<dt>partic</dt><dd>
<p>Percent of adult women in the workforce.
</p>
</dd>
<dt>tfr</dt><dd>
<p>Total fertility rate: expected births to a cohort of 1000
women at current age-specific fertility rates.
</p>
</dd>
<dt>menwage</dt><dd>
<p>Men's average weekly wages, in constant 1935 dollars and
adjusted for current tax rates.
</p>
</dd>
<dt>womwage</dt><dd>
<p>Women's average weekly wages.
</p>
</dd>
<dt>debt</dt><dd>
<p>Per-capita consumer debt, in constant dollars.
</p>
</dd>
<dt>parttime</dt><dd>
<p>Percent of the active workforce working 34 hours per week or
less.
</p>
</dd>
</dl>



<h3>Warning</h3>

<p>The value of <code>tfr</code> for 1973 is misrecorded as 2931; it should be 1931.
</p>


<h3>Source</h3>

<p>Fox, B. (1980) 
<em>Women's Domestic Labour and their Involvement 
in Wage Work.</em> Unpublished doctoral dissertation, p. 449.
</p>


<h3>References</h3>

<p>Fox, J. (2016)
<em>Applied Regression Analysis and Generalized Linear Models</em>,
Third Edition. Sage.  
</p>

<hr /><div style="text-align: center;">[Package <em>carData</em> version 3.0-5 <a href="00Index.html">Index</a>]</div>

## sleep - `datasets > sleep`


![Linux 사례 (MX 21)](fig/dataset-sleep-01.png)

![Linux 사례 (MX 21)](fig/dataset-sleep-02.png)


```r
data(sleep, package="datasets")
summary(sleep)
str(sleep)
```

데이터셋의 내부는 다음과 같다:

![Linux 사례 (MX 21)](fig/dataset-sleep-03.png)


<table width="100%" summary="page for sleep {datasets}"><tr><td>sleep {datasets}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>Student's Sleep Data</h2>

<h3>Description</h3>

<p>Data which show the effect of two soporific drugs (increase in hours
of sleep compared to control) on 10 patients.
</p>


<h3>Usage</h3>

<pre>sleep</pre>


<h3>Format</h3>

<p>A data frame with 20 observations on 3 variables.
</p>

<table summary="Rd table">
<tr>
 <td style="text-align: right;">
    [, 1] </td><td style="text-align: left;"> extra </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> increase in hours of sleep</td>
</tr>
<tr>
 <td style="text-align: right;">
    [, 2] </td><td style="text-align: left;"> group </td><td style="text-align: left;"> factor  </td><td style="text-align: left;"> drug given</td>
</tr>
<tr>
 <td style="text-align: right;">
    [, 3] </td><td style="text-align: left;"> ID    </td><td style="text-align: left;"> factor  </td><td style="text-align: left;"> patient ID
  </td>
</tr>

</table>



<h3>Details</h3>

<p>The <code>group</code> variable name may be misleading about the data:
They represent measurements on 10 persons, not in groups.

</p>


<h3>Source</h3>

<p>Cushny, A. R. and Peebles, A. R. (1905)
The action of optical isomers: II hyoscines.
<em>The Journal of Physiology</em> <b>32</b>, 501&ndash;510.
</p>
<p>Student (1908)
The probable error of the mean.
<em>Biometrika</em>, <b>6</b>, 20.
</p>


<h3>References</h3>

<p>Scheff챕, Henry (1959)
<em>The Analysis of Variance</em>.
New York, NY: Wiley.
</p>


<h3>Examples</h3>

<pre>
require(stats)
## Student's paired t-test
with(sleep,
     t.test(extra[group == 1],
            extra[group == 2], paired = TRUE))

## The sleep *prolongations*
sleep1 &lt;- with(sleep, extra[group == 2] - extra[group == 1])
summary(sleep1)
stripchart(sleep1, method = "stack", xlab = "hours",
           main = "Sleep prolongation (n = 10)")
boxplot(sleep1, horizontal = TRUE, add = TRUE,
        at = .6, pars = list(boxwex = 0.5, staplewex = 0.25))
</pre>

<hr /><div style="text-align: center;">[Package <em>datasets</em> version 4.1.3 <a href="00Index.html">Index</a>]</div>


## DavisThin - `carData > DavisThin`


![Linux 사례 (MX 21)](fig/dataset-davis-01.png)



![Linux 사례 (MX 21)](fig/dataset-davis-02.png)


![Linux 사례 (MX 21)](fig/dataset-davis-03.png)

```r
help("DavisThin")
```


<table width="100%" summary="page for DavisThin {carData}"><tr><td>DavisThin {carData}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>Davis's Data on Drive for Thinness</h2>

<h3>Description</h3>

<p>The <code>DavisThin</code> data frame has 191 rows and 7 columns.
This is part of a larger dataset for a study of eating disorders.
The seven variables in the data frame comprise a &quot;drive for thinness&quot;
scale, to be formed by summing the items.
</p>


<h3>Usage</h3>

<pre>DavisThin</pre>


<h3>Format</h3>

<p>This data frame contains the following columns:
</p>

<dl>
<dt>DT1</dt><dd><p>a numeric vector</p>
</dd>
<dt>DT2</dt><dd><p>a numeric vector</p>
</dd>
<dt>DT3</dt><dd><p>a numeric vector</p>
</dd>
<dt>DT4</dt><dd><p>a numeric vector</p>
</dd>
<dt>DT5</dt><dd><p>a numeric vector</p>
</dd>
<dt>DT6</dt><dd><p>a numeric vector</p>
</dd>
<dt>DT7</dt><dd><p>a numeric vector</p>
</dd>
</dl>



<h3>Source</h3>

<p>Davis, C., G. Claridge, and D. Cerullo (1997) 
Personality factors 
predisposing to weight preoccupation: A continuum approach to the 
association between eating disorders and personality disorders. 
<em>Journal of Psychiatric Research</em> <b>31</b>, 467&ndash;480. [personal communication from the authors.]
</p>


<h3>References</h3>

<p>Fox, J. and Weisberg, S. (2019) 
<em>An R Companion to Applied Regression</em>, Third Edition, Sage.
</p>

<hr /><div style="text-align: center;">[Package <em>carData</em> version 3.0-5 <a href="00Index.html">Index</a>]</div>


## USArrests - `datasets > USArrests`

![Linux 사례(MX 21)](fig/dataset-usarrest-01.png)

![Linux 사례(MX 21)](fig/dataset-usarrest-02.png)



```r
data(USArrests, package="datasets")
```


![Linux 사례(MX 21)](fig/dataset-usarrest-03.png)


R Commander 화면 상단에서 <데이터셋 보기> 버튼을 누르면 아래와 같은 내부 구성을 확인할 수 있다.



```r
help("USArrests")
```



<table width="100%" summary="page for USArrests {datasets}"><tr><td>USArrests {datasets}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>Violent Crime Rates by US State</h2>

<h3>Description</h3>

<p>This data set contains statistics, in arrests per 100,000 residents
for assault, murder, and rape in each of the 50 US states in 1973.
Also given is the percent of the population living in urban areas.
</p>


<h3>Usage</h3>

<pre>USArrests</pre>


<h3>Format</h3>

<p>A data frame with 50 observations on 4 variables.
</p>

<table summary="Rd table">
<tr>
 <td style="text-align: right;">
    [,1]  </td><td style="text-align: left;"> Murder    </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> Murder arrests (per 100,000)</td>
</tr>
<tr>
 <td style="text-align: right;">
    [,2]  </td><td style="text-align: left;"> Assault   </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> Assault arrests (per 100,000)</td>
</tr>
<tr>
 <td style="text-align: right;">
    [,3]  </td><td style="text-align: left;"> UrbanPop  </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> Percent urban population</td>
</tr>
<tr>
 <td style="text-align: right;">
    [,4]  </td><td style="text-align: left;"> Rape      </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> Rape arrests (per 100,000)
  </td>
</tr>

</table>



<h3>Note</h3>

<p><code>USArrests</code> contains the data as in McNeil's monograph.  For the
<code>UrbanPop</code> percentages, a review of the table (No. 21) in the
Statistical Abstracts 1975 reveals a transcription error for Maryland
(and that McNeil used the same &ldquo;round to even&rdquo; rule that <span style="font-family: Courier New, Courier; color: #666666;"><b>R</b></span>'s
<code><a href="../../base/html/Round.html">round</a>()</code> uses), as found by Daniel S Coven (Arizona).
</p>
<p>See the example below on how to correct the error and improve accuracy
for the &lsquo;&lt;n&gt;.5&rsquo; percentages.
</p>


<h3>Source</h3>

<p>World Almanac and Book of facts 1975.  (Crime rates).
</p>
<p>Statistical Abstracts of the United States 1975, p.20, (Urban rates),
possibly available as
<a href="https://books.google.ch/books?id=zl9qAAAAMAAJ&amp;pg=PA20">https://books.google.ch/books?id=zl9qAAAAMAAJ&amp;pg=PA20</a>.
</p>


<h3>References</h3>

<p>McNeil, D. R. (1977)
<em>Interactive Data Analysis</em>.
New York: Wiley.
</p>


<h3>See Also</h3>

<p>The <code><a href="../../datasets/help/state.html">state</a></code> data sets.</p>


<h3>Examples</h3>

<pre>
summary(USArrests)

require(graphics)
pairs(USArrests, panel = panel.smooth, main = "USArrests data")

## Difference between 'USArrests' and its correction
USArrests["Maryland", "UrbanPop"] # 67 -- the transcription error
UA.C &lt;- USArrests
UA.C["Maryland", "UrbanPop"] &lt;- 76.6

## also +/- 0.5 to restore the original  &lt;n&gt;.5  percentages
s5u &lt;- c("Colorado", "Florida", "Mississippi", "Wyoming")
s5d &lt;- c("Nebraska", "Pennsylvania")
UA.C[s5u, "UrbanPop"] &lt;- UA.C[s5u, "UrbanPop"] + 0.5
UA.C[s5d, "UrbanPop"] &lt;- UA.C[s5d, "UrbanPop"] - 0.5

## ==&gt; UA.C  is now a *C*orrected version of  USArrests
</pre>

<hr /><div style="text-align: center;">[Package <em>datasets</em> version 4.1.3 <a href="00Index.html">Index</a>]</div>

## birthwt - `MASS > birthwt`

![Linux 사례 (MX 21)](fig/dataset-birthwt-01.png)


```r
data(birthwt, package="MASS")
```




birthwt 데이터셋이 활성화된 후, <데이터셋 보기> 버튼을 누르면 아래와 같이 내부 구성을 볼 수 있다:

![Linux 사례 (MX 21)](fig/dataset-birthwt-02.png)


```r
help("birthwt")
```

![Linux 사례 (MX 21)](fig/dataset-birthwt-03.png)


<table width="100%" summary="page for birthwt {MASS}"><tr><td>birthwt {MASS}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>
Risk Factors Associated with Low Infant Birth Weight
</h2>

<h3>Description</h3>

<p>The <code>birthwt</code> data frame has 189 rows and 10 columns.
The data were collected at Baystate Medical Center, Springfield, Mass
during 1986.
</p>


<h3>Usage</h3>

<pre>
birthwt
</pre>


<h3>Format</h3>

<p>This data frame contains the following columns:
</p>

<dl>
<dt><code>low</code></dt><dd><p>indicator of birth weight less than 2.5 kg.</p>
</dd>
<dt><code>age</code></dt><dd><p>mother's age in years.</p>
</dd>
<dt><code>lwt</code></dt><dd><p>mother's weight in pounds at last menstrual period.</p>
</dd>
<dt><code>race</code></dt><dd><p>mother's race (<code>1</code> = white, <code>2</code> = black,
<code>3</code> = other).</p>
</dd>
<dt><code>smoke</code></dt><dd><p>smoking status during pregnancy.</p>
</dd>
<dt><code>ptl</code></dt><dd><p>number of previous premature labours.</p>
</dd>
<dt><code>ht</code></dt><dd><p>history of hypertension.</p>
</dd>
<dt><code>ui</code></dt><dd><p>presence of uterine irritability.</p>
</dd>
<dt><code>ftv</code></dt><dd><p>number of physician visits during the first trimester.</p>
</dd>
<dt><code>bwt</code></dt><dd><p>birth weight in grams.</p>
</dd>
</dl>



<h3>Source</h3>

<p>Hosmer, D.W. and Lemeshow, S. (1989)
<em>Applied Logistic Regression.</em> New York: Wiley
</p>


<h3>References</h3>

<p>Venables, W. N. and Ripley, B. D. (2002)
<em>Modern Applied Statistics with S.</em> Fourth edition.  Springer.
</p>


<h3>Examples</h3>

<pre>
bwt &lt;- with(birthwt, {
race &lt;- factor(race, labels = c("white", "black", "other"))
ptd &lt;- factor(ptl &gt; 0)
ftv &lt;- factor(ftv)
levels(ftv)[-(1:2)] &lt;- "2+"
data.frame(low = factor(low), age, lwt, race, smoke = (smoke &gt; 0),
           ptd, ht = (ht &gt; 0), ui = (ui &gt; 0), ftv)
})
options(contrasts = c("contr.treatment", "contr.poly"))
glm(low ~ ., binomial, bwt)
</pre>

<hr /><div style="text-align: center;">[Package <em>MASS</em> version 7.3-55 <a href="00Index.html">Index</a>]</div>


## Friendly - `carData > Friendly`

![Linux 사례 (MX 21)](fig/dataset-friendly-01.png)


```r
data(Friendly, package="carData")
```



![Linux 사례 (MX 21)](fig/dataset-friendly-02.png)


```r
help("Friendly")
```


<table width="100%" summary="page for Friendly {carData}"><tr><td>Friendly {carData}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>Format Effects on Recall</h2>

<h3>Description</h3>

<p>The <code>Friendly</code> data frame has 30 rows and 2 columns.
The data are from an experiment on subjects' ability to remember words
based on the presentation format.
</p>


<h3>Usage</h3>

<pre>
Friendly
</pre>


<h3>Format</h3>

<p>This data frame contains the following columns:
</p>

<dl>
<dt>condition</dt><dd>
<p>A factor with levels:
<code>Before</code>, Recalled words presented before others;
<code>Meshed</code>, Recalled words meshed with others; 
<code>SFR</code>, Standard free recall.
</p>
</dd>
<dt>correct</dt><dd>
<p>Number of words correctly recalled, out of 40 on final trial of the experiment.
</p>
</dd>
</dl>



<h3>Source</h3>

<p>Friendly, M. and Franklin, P. (1980) 
Interactive presentation in multitrial free recall. 
<em>Memory and Cognition</em>
<b>8</b> 265&ndash;270 [Personal communication from M. Friendly].
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

## Cowles - `carData > Cowles`

![Linux 사례 (MX 21)](fig/dataset-cowles-01.png)


```r
data(Cowles, package="carData")
```

![Linux 사례 (MX 21)](fig/dataset-cowles-02.png)



```r
help("Cowles")
```


<table width="100%" summary="page for Cowles {carData}"><tr><td>Cowles {carData}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>Cowles and Davis's Data on Volunteering</h2>

<h3>Description</h3>

<p>The <code>Cowles</code> data frame has 1421 rows and 4 columns.
These data come from a study of the personality determinants
of volunteering for psychological research.
</p>


<h3>Usage</h3>

<pre>Cowles</pre>


<h3>Format</h3>

<p>This data frame contains the following columns:
</p>

<dl>
<dt>neuroticism</dt><dd><p>scale from Eysenck personality inventory</p>
</dd>
<dt>extraversion</dt><dd><p>scale from Eysenck personality inventory</p>
</dd>
<dt>sex</dt><dd><p>a factor with levels: <code>female</code>; <code>male</code></p>
</dd>
<dt>volunteer</dt><dd><p>volunteeing, a factor with levels: <code>no</code>; <code>yes</code></p>
</dd>
</dl>



<h3>Source</h3>

<p>Cowles, M. and C. Davis (1987)
The subject matter of psychology: Volunteers.
<em>British Journal of Social Psychology</em> <b>26</b>, 97&ndash;102.
</p>

<hr /><div style="text-align: center;">[Package <em>carData</em> version 3.0-5 <a href="00Index.html">Index</a>]</div>

## Adler - `carData > Adler`

![Linux 사례 (MX 21)](fig/dataset-adler-01.png)

데이터 > 패키지에 있는 데이터 > 첨부된 패키지에서 데이터셋 읽기... 기능을 선택하면, 위와 같은 메뉴 창을 보게된다.

carData를 선택하여 두번 클릭하면, 오른쪽에 carData 패키지에 내장된 데이터셋 목록이 등장한다. Adler 데이터셋을 선택한다.

![Linux 사례 (MX 21)](fig/dataset-adler-02.png)



```r
data(Adler, package="carData")  # Adler 데이터셋 활성화시키기
help("Adler", package="carData")# 도움말파일 열기
```



<table width="100%" summary="page for Adler {carData}"><tr><td>Adler {carData}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>Experimenter Expectations</h2>

<h3>Description</h3>

<p>The <code>Adler</code> data frame has 108 rows and 3 columns.  
</p>
<p>The &ldquo;experimenters&rdquo; were the actual subjects of the study. 
They collected ratings of the apparent success of
people in pictures who were pre-selected for their
average appearance of success. The experimenters were told prior to collecting 
data that particular subjects were either high or low in their tendency to rate 
appearance of success, and were instructed to get good data, 
scientific data, or were given no such instruction. Each 
experimenter collected ratings from 18 randomly assigned
subjects. This version of the Adler data is taken from Erickson and Nosanchuk (1977).
The data described in the original source, Adler (1973), have a more complex structure.
</p>


<h3>Usage</h3>

<pre>
Adler
</pre>


<h3>Format</h3>

<p>This data frame contains the following columns:
</p>

<dl>
<dt>instruction</dt><dd>
<p>a factor with levels:
<code>good</code>, good data;
<code>none</code>, no stress;
<code>scientific</code>, scientific data.
</p>
</dd>
<dt>expectation</dt><dd>
<p>a factor with levels:
<code>high</code>, expect high ratings;
<code>low</code>, expect low ratings.
</p>
</dd>
<dt>rating</dt><dd>
<p>The average rating obtained.  
</p>
</dd>
</dl>



<h3>Source</h3>

<p>Erickson, B. H., and Nosanchuk, T. A. (1977)
<em>Understanding Data.</em> McGraw-Hill Ryerson.
</p>


<h3>References</h3>

<p>Adler, N. E. (1973)
Impact of prior sets given experimenters and subjects on the experimenter
expectancy effect.
<em>Sociometry</em> <b>36</b>, 113&ndash;126.
</p>

<hr /><div style="text-align: center;">[Package <em>carData</em> version 3.0-5 <a href="00Index.html">Index</a>]</div>

## warpbreaks - `datasets > warpbreaks`

![Linux 사례 (MX 21)](fig/dataset-warpbreaks-01.png)


```r
data(warpbreaks, package="datasets") # 데이터셋 불러오기	
help("warpbreaks")                   # 데이터셋 도움말 보기
summary(warpbreaks)                  # 데이터셋 통계 요약 보기
```



![Linux 사례 (MX 21)](fig/dataset-warpbreaks-02.png)

R Commander 화면 상단 우측에 있는 <데이터셋 보기> 버튼을 누른다. 아래와 같이 warpbreaks 데이터셋의 내부 구성을 볼 수 있다.

![Linux 사례 (MX 21)](fig/dataset-warpbreaks-03.png)



<table width="100%" summary="page for warpbreaks {datasets}"><tr><td>warpbreaks {datasets}</td><td style="text-align: right;">R Documentation</td></tr></table>

<h2>The Number of Breaks in Yarn during Weaving</h2>

<h3>Description</h3>

<p>This data set gives the number of warp breaks per loom, where a loom
corresponds to a fixed length of yarn.
</p>


<h3>Usage</h3>

<pre>warpbreaks</pre>


<h3>Format</h3>

<p>A data frame with 54 observations on 3 variables.
</p>

<table summary="Rd table">
<tr>
 <td style="text-align: right;">
    <code>[,1]</code> </td><td style="text-align: left;"> <code>breaks</code>  </td><td style="text-align: left;"> numeric </td><td style="text-align: left;"> The number of breaks</td>
</tr>
<tr>
 <td style="text-align: right;">
    <code>[,2]</code> </td><td style="text-align: left;"> <code>wool</code>    </td><td style="text-align: left;"> factor  </td><td style="text-align: left;"> The type of wool (A or B)</td>
</tr>
<tr>
 <td style="text-align: right;">
    <code>[,3]</code> </td><td style="text-align: left;"> <code>tension</code> </td><td style="text-align: left;"> factor  </td><td style="text-align: left;"> The level of tension (L, M, H)
  </td>
</tr>

</table>

<p>There are measurements on 9 looms for each of the six types of warp
(<code>AL</code>, <code>AM</code>, <code>AH</code>, <code>BL</code>, <code>BM</code>, <code>BH</code>).
</p>


<h3>Source</h3>

<p>Tippett, L. H. C. (1950)
<em>Technological Applications of Statistics</em>.
Wiley.  Page 106.
</p>


<h3>References</h3>

<p>Tukey, J. W. (1977)
<em>Exploratory Data Analysis</em>.
Addison-Wesley.
</p>
<p>McNeil, D. R. (1977)
<em>Interactive Data Analysis</em>.
Wiley.
</p>


<h3>See Also</h3>

<p><code><a href="../../stats/html/xtabs.html">xtabs</a></code> for ways to display these data as a table.
</p>


<h3>Examples</h3>

<pre>
require(stats); require(graphics)
summary(warpbreaks)
opar &lt;- par(mfrow = c(1, 2), oma = c(0, 0, 1.1, 0))
plot(breaks ~ tension, data = warpbreaks, col = "lightgray",
     varwidth = TRUE, subset = wool == "A", main = "Wool A")
plot(breaks ~ tension, data = warpbreaks, col = "lightgray",
     varwidth = TRUE, subset = wool == "B", main = "Wool B")
mtext("warpbreaks data", side = 3, outer = TRUE)
par(opar)
summary(fm1 &lt;- lm(breaks ~ wool*tension, data = warpbreaks))
anova(fm1)
</pre>

<hr /><div style="text-align: center;">[Package <em>datasets</em> version 4.1.3 <a href="00Index.html">Index</a>]</div>

