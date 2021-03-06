--- 
title: "설치형 오픈 통계 패키지 - `Rcmdr`"
author: "신종화, 이광춘, 유충현, 홍성학"
date: "2022-05-24"
site: bookdown::bookdown_site
output: bookdown::gitbook
documentclass: book
bibliography: [book.bib, packages.bib]
biblio-style: apalike
link-citations: yes
github-repo: bit2r/Rcmdr
description: "John Fox 교수님이 개발한 `Rcmdr` 오픈 통계 패키지를 통계 대중화를 위해 한글화해서 공유합니다."
---




# 들어가며

**한국 알(R) 사용자회**는 디지털 불평등 해소와 통계 대중화를 오픈 통계 패키지 개발을 2021년부터 추진하였습니다.
더불어 설치형 오픈 통계 패키지를 신종화 님께서 John Fox 교수님이 개발한 `Rcmdr`[@fox2016using] [@rcmdr2022manual] [@rcmdr2005paper] 기반으로 한글화 및 문서화에 10년 넘게 기여해주셨습니다. 이에 **한국 알(R) 사용자회**는 신종화님의 `Rcmdr` 거인의 어깨위에 디지털 불평등 해소와 통계 대중화를 위해 한 걸음 더 나아가게 되었습니다. 특히 신종화님께서 기여하신 한글화 및 문서를 근간으로 더 많은 분들이 오픈 통계 패키지를 사용할 수 있도록 `bookdown`으로 내용을 정리하여 통계 대중화가 한층 앞당겨질 것으로 기대됩니다.

신종화님께서 왜 오픈 통계 패키지로 `Rcmdr`를 근간으로 해야 하는지 이유를 명쾌하게 다음과 같이 정리해 주셨습니다.

R에는 여러 개의 GUI 작업도구들이 있습니다. 모두 목적이 분명하고, 좋은 도구이며, 일부는 현재도 향상작업이 진행되고 있습니다. 그럼에도 불구하고 R Commander를 위한 블로그 작업을 진행하는 이유는 크게 두가지 입니다.

첫째, R Commander는 직관적으로 기존의 기초통계학 도구와 유사합니다. Command Line 에서 작업하는 것에 익숙하지 않은, 또 어려움을 겪고 있는 사용자들에게 기초통계학분야를 학습하고 활용하는데 도움을 주기 위하여 R Commander가 개발되었습니다. 개발자인 John Fox 교수는 이 목적과 관리방향을 분명히하고 있습니다. 중급이상의 R 사용자/ 고급통계 연구자들에게는 R Commander가 불필요할 수 있습니다.

둘째, 지난 10년동안 R Commander의 메뉴 한글화작업을 진행해왔으며, 현재도 유지관리를 하고 있습니다. (이 정보는 R Commander 안의 Help > About Rcmdr 에 있습니다) [Translations:  Korean, Chel Hee Lee, Dae-Heung Jang, and Shin Jong-Hwa] 지난 10년 동안 개인적인 메모 차원에서 R Commander 사용 및 한글화 관련 블로그 포스트를 만들고 관리되어 왔고 [블로그](http://modernity.tistory.com)에 전체 과정이 고스란히 남아있고 계속적으로 유지관리될 것입니다.

- 신종화 [Rcmdr : R Commander](https://rcmdr.kr/)
- [CRAN Rcmdr 패키지 정보](https://cran.r-project.org/web/packages/Rcmdr/index.html)
- [개발자 John Fox 교수의 Rcmdr 소개](https://socialsciences.mcmaster.ca/jfox/Misc/Rcmdr/)
- [FOSSER_Ricoop](https://modernity.tistory.com/)


