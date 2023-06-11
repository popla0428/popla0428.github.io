---
layout: post
title: /[ABT/] ABT 기본용어 및 개념 - MEI (Minimum Effect of Interest) (vs. MDE)
tags: [ABT]
description: >
  Definition of Minimum Effect of Interest in the context of A/B testing
sitemap: false
categories:
  - study
  - 강의리뷰-및-실습 
 # 글이 소속되는 카테고리 
 # 하단 글 작성에서 샾 제목 쓰면 위의 title 보다 더 우선 적용노출됨 
---

# [ABT] ABT 기본용어 및 개념 - MEI (Minimum Effect of Interest) (vs. MDE)

**NOTE**  
`Analytics Toolkit`의 <a href="https://www.analytics-toolkit.com/glossary/minimum-effect-of-interest/" target = "_blank">Definition of Minimum Effect of Interest in the context of A/B testing</a> 요약.  

- Table of Contents
{:toc .large-only}

## 실험전 세팅되어야 하는 필수 파라미터  
> 실험계획 필수 인풋 파라미터  
- ① Significance level (유효수준), Power (파워;검정력)   
- ② MEI (Minimum Effect of Interest; 최소 관심 크기)
- ③ Sample size (표본크기; 샘플크기)  

---

① Significance level ($\alpha$) (비즈니스 10%정도 허용), and Power level (1-$\beta$)  
    - https://www.analytics-toolkit.com/glossary/risk-reward-analysis/     

② MEI (Minimum Effect of Interest)  
> 실험(ABT,RCT) 결과를 통계적으로 검정할 때 우리(실험자)가 희망하는 효과 크기(effect size).

- 적절한 크기의 MEI 정하는 것이 중요한 이유?  
    - 이 값이 잘 세팅되어야 실험에 필요한 샘플크기 계산 가능하고, 결과적으로 MEI에 충분한 통계 검정력을 얻을 수 있다.  

- ⭐️ 보통 MDE (Minimum Detectable Effect)라는 용어가 더 많이 사용되지만 저자는 권장하지 않는다 (용도에 맞게 다른 용어를 써야한다는 의미).  
- ⭐️ **이유는?**  
    * MDE는 통계적 검정의 기술적 특성을 내포하는 용어로 받아들여 진다. 하지만 MEI는 검정에 필요한 하나의 파라미터라는 게 잘 드러난다.  
    * 또한, MDE는 그 용어 때문에 이 수치보다 작은 참 효과들은 탐지할 수 없다는 착각을 하게 만든다. 이게 잘못된 이해라는 것은 (유의수준, 샘플크기 고정) 유효크기에 따른 실험의 검정력을 계산한 검정력 함수 (power function) 통해 확인할 수 있음.
    * 따라서, 특히 실험계획(디자인)의 인풋 파라미터를 논의할 때에는 `MEI`를 사용함으로써 이 값은 **'실험자가 탐지하고 싶은'** 최소 효과크기(effect size)임을 명확히 하는 것이 좋겠다!

③ Sample size ($\n$)