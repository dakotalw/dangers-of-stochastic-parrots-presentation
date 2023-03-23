# Dangers Of Stochastic Parrots Presentation

Presentation of "On the Dangers of Stochastic Parrots: Can Language Models Be Too Big?" for DS-5899-01 at Vanderbilt University

## Introduction

Over the past 5 years, we have been experiencing huge advances in language models, and this trend seems to only be continuing. with brand new technologies such as GPT-4 coming out just this past week. The capabilities of these new models are impressive and with the rapid improvements in capabilities of these models, it is easy to see why experts are so eager to develop and improve these models so quickly. One of the driving factors in this rapid innovation is the increased avaliability and decreased cost of computational resources that allow models to grow larger than ever and be trained on more and more data. This is represented in the following figure, showing the growth in both parameter count and training dataset size from 2019-2021.

<img src="figure1.png" alt="Figure 1" width="500">

The purpose of this paper is to highlight some of the concerns that come along with these large-scale language models, ranging from environmental concerns to the social and ethical isues that arise with LMs like these.

## Overview / Problem

Overall, I would break down the main arguments of the authors into three main concerns with large language models: environmental concerns, social bias and lack of interpretability.

#### Environmental Concerns

With the ongoing climate crisis, there has been a big push for companies to be more responsible with their emissions, particularly carbon dioxide emissions. It is estimated that a human will use 5 tons of carbon dioxide emissions (CO<sub>2</sub>e) per year in 2017. According to 'Energy and Policy Considerations for Deep Learning in NLP' by Strubell et al., a single training of a large transformer can take upwards of 280 tons CO<sub>2</sub>e. It is noted that hardly any of the energy sources that cloud computing services utilize are renewable. Listed below are a series of models that were examined for environemental costs in Strubell et al.'s paper:

<img src="figures/figure2.png" alt="alt text" width="800">

The authors note how this high cost is not necessairly a bad thing as long as there is an improvement in accuracy. This was tested with the task of machine translation, a field where large language models had previously shown performance gains. It was estimated that in an English-to-German translation task, it costed 150,000 dollars and an unreported CO<sub>2</sub>e increase to raise the BLEU score (similarity between machine and human translation) by 0.1.

To bridge our discussion between environmental and social concerns, I want to bright to light another point that the author makes on how those communities who are generally most affected by climate change are generally those who will benefit from a large language model the least. As an example, people who live in the Maldives are estimated to have their home country completely submerged by 2100, however only around 60 percent of the residents have access to the internet. For those that do have internet access, it is unlikely that large language models are being developed for Dhivehi speakers, further reducing the percentage of individuals who would benefit from these technologies.

#### Social Concerns

When looking at social concerns, a lot of the discussion tends to revolve around bias involved in the training data. It has been shown in many studies in the past that problematic training sets can result in LMs that parrot derogatory sentiments along the lines of race, gender, ethnicity or disability status. There have been ongoing efforts such as Common Crawl, described as "petabytes of data collected over 8 years of web crawling", to create massive datasets that will accurately reflect the large and diverse online space. A filtered version of Common Crawl is part of the GPT-3 training set, but even with this, there is still a white-dominated viewpoint expressed in much of the data that is in US or UK English. Data from the Common Crawl that was used was selected for its similarity to GPT-2 training data, which is largely based on avaliable internet text data, such as Wikipedia articles or Reddit discussions, further pushing this issue since these are sites that are generally visited and maintaned by white males between the ages of 18-29. This was not the only diversity concern in their filtering methods however; all documents were checked and thrown out if they contained a word on a giant corpus of foul language, including slurs, swears, pornographic terms and other hate speech. Authors note how certain included terms such as 'twink' or 'queer' may have been seen as a pornographic or derogatory in the past, but have been adopted by the LGBTQ+ community as non-derogatory terms. This results in a model that is less likely to have been exposed to material from online spaces designed for and occupied by LGBTQ+ people.



## Authors' Suggestions

report training time and
sensitivity to hyperparameters when the released model is meant
to be re-trained for downstream use. 

There should be more of an emphasis on publishing and understanding LMs; we want to manage hype around these models so that we are not promoting training of larger models for lofty tasks

carbon efficiency/energy consumption as evaluation metric

## Let's Talk GPT-4

The rollout of GPT-4 has only exacerbated this issue for several reasons: of course the increased size of this model, but also there has been a serious lack of transparency from OpenAI regarding GPT-4. There has been no official figure for the number of parameters or the size of the training dataset, only that we know the training data now contains images.

There is no denying that technologies like this are already making life easier for those with access; ChatGPT has only been avaliable to the public for around 5 months and is already  and the purpose of this paper is not to stop people from training large language models. Th


## Critical Analysis

text

## Discussion Questions

- How should these companies handle the balance of protecting industry secrets and fairly reporting their resources used? Should the government step in?

## Related Articles

**Energy and Policy Considerations for Deep Learning in NLP** - https://arxiv.org/pdf/1906.02243.pdf

**OpenAI co-founder on company’s past approach to openly sharing research: ‘We were wrong’** - https://www.theverge.com/2023/3/15/23640180/openai-gpt-4-launch-closed-research-ilya-sutskever-interview


In the sense of this paper, language models are defined by systems that are trained for string prediction tasks

Computational needs has gone down compared to some past methods such as n-gram models which use connected substrings, with technologies such as embedding being developed that significantly decrease the size of the data used


