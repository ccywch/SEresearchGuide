# Guide to academic paper writing in software engineering domain

This is a brief guide in writing research papers in software engineering, especially useful for novices to propose a novel approach for solving a novel task.  
Note that it is only based on my own experience, which may be of some bias.
And it may not apply to some particular type of paper writing (e.g., empirical study, experience report), but some suggestions in this guide may still benefit your writing even in other areas (e.g., HCI).
Following commonly-used paper structure, I share some of my suggestions about different sections ranging from abstract to conclusion as follows:


## Abstract
Different from the conclusion, we focus more on the background and motivation in writing abstract.
So please use the 60%-70% space in this section to include the background, motivation, question formulation, limitation of existing works.
Briefly tell the approach and evaluation (give some numbers) in the rest.

## Introduction
By default, write one short paragraph for each item of the list:
* Background
* Task formulation
* Motivation and benefit of this task
* Existing studies and corresponding limitations
* Our approach (1-2 paragraphs)
* Evaluation
* A list of contributions (e.g., a novel approach for a novel question, an empirical study, an open-source tool, comprehensive evaluation)

## Approach
* A flow chart for the overall approach (It always takes me one afternoon to draw)
* Give some examples or draw some figures to demonstrate some steps in the approach 
* For some complicated logic, either write some mathematic formula (represent the problem formally) or a pseudo-code algorithm

## Evaluation
Compared with other areas (e.g., AI, HCI), SE strongly emphasises the evaluation.
For automated accuracy evaluation, please tell:
- Evaluation of each component within the approach and performance of the whole approach
- Evaluation dataset
- Metrics
- Baselines 
- Evaluation results
  - Comparison with baselines and summarize several reasons why our model outperforms
  - Error analysis: reasons why our model fails in some cases
  - Always give detailed examples to help illustrate the strength and shortcomings of our approach

In addition to the quantitative analysis, we also adopt the qualitative, especially the user study to demonstrate the usefulness of our tool.
*TODO*: I will write more about user study later.

## Discussion
This section is optional for a technical paper, but indispensable for empirical study.
* Generality
* Potential application
* Implications

## Related works
You may separate related works into several subsections.
But please note:
* Explicitly tell relations among different works, not just saying "AAA et al. \[??\] do this, BBB et al. \[??\] do that".
* At the end of each subsection, please explicitly tell the difference between our work and related works mentioned above.
* We usually put this section at the end of the paper in SE, but after introduction in HCI.

## Conclusion
Different from the abstract, this section focuses more on summerization without mentioning background or motivation.
Please include:
* Summarization of task, approach and evaluation in this study
* Future works 

## Other general suggestions
* Use short sentences with active voice in the paper, and keep the length of each paragraph consistent.
* Use formal words in academic writing, rather than oral words in daily speaking (e.g., pretty small)
* For some terms, do not use them arbitrarily. Please refer to other papers or online articles/blogs/tutorials written by native speakers. Once determined, please use it consistently across the whole paper.
* Before writing the paper, you are highly suggested to come up with the overall structure and discuss it with your supervisor. Then add figures, tables, algorithms while finally fill in detailed text.
* If this is your first time writing research papers, you are highly recommended to find one of your favorite papers (in the same type of yours) as the template for writing your own one.
* Be very serious about drawing **pictures/figures/tables**, which significantly influence readers' first expression, since a picture is worth a thousand words. 
* Before the paper submission, please ask non-authors to proofread it. If you are using Overleaf, please consider the [Grammerly extension](https://chrome.google.com/webstore/detail/overleaf-textarea/iejmieihafhhmjpoblelhbpdgchbckil?hl=en) on Chrome for grammar checking.

## Other Useful links:
1. [Draft Guidelines for My Students on Writing Software Engineering Research Papers](https://cragkhit.github.io/files/harman-writing-advice.pdf) by Mark Harman
2. https://www.163.com/dy/article/G4I3L5CH05366EUH.html
3. [The guide of paper writing in Latex] (https://github.com/ccywch/SEresearchGuide/blob/master/LatexWriting.md)
