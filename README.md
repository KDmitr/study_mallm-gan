# study_mallm-gan
The effectivness of the algorithm for generating MALLM-GAN data was investigated.\
Original paper: Ling, Yaobin et al. “MALLM-GAN: Multi-Agent Large Language Model as Generative Adversarial Network for Synthesizing Tabular Data.” [ArXiv abs/2406.10521 (2024): n. pag.](https://arxiv.org/pdf/2406.10521)

### **Repeating the experiments described in the article**
<table class="tg"><thead>
  <tr>
    <th class="tg-c3ow"><span style="font-weight:bold">N</span></th>
    <th class="tg-0pky"></th>
    <th class="tg-fymr">Adult (<span style="font-weight:bold">F</span>1<span style="font-weight:bold">)</span></th>
    <th class="tg-fymr">Insurance (R2)</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0pky" rowspan="2">100</td>
    <td class="tg-0pky">Paper</td>
    <td class="tg-0pky">0.79&plusmn0.02</td>
    <td class="tg-0pky">0.72&plusmn0.00</td>
  </tr>
  <tr>
    <td class="tg-0pky">Our</td>
    <td class="tg-0pky">0.80</td>
    <td class="tg-0pky">0.73</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="2">200</td>
    <td class="tg-0pky">Paper</td>
    <td class="tg-0pky">0.77&plusmn0.03</td>
    <td class="tg-0pky">0.72&plusmn0.03</td>
  </tr>
  <tr>
    <td class="tg-0pky">Our</td>
    <td class="tg-0pky">0.74</td>
    <td class="tg-0pky">0.61</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="2">400</td>
    <td class="tg-0pky">Paper</td>
    <td class="tg-0pky">0.79&plusmn0.02</td>
    <td class="tg-0pky">0.71&plusmn0.03</td>
  </tr>
  <tr>
    <td class="tg-0pky">Our</td>
    <td class="tg-0pky">0.72</td>
    <td class="tg-0pky">0.11</td>
  </tr>
  <tr>
    <td class="tg-0pky" rowspan="2">800</td>
    <td class="tg-0pky">Paper</td>
    <td class="tg-0pky">0.80&plusmn0.02</td>
    <td class="tg-0pky">0.72&plusmn0.01</td>
  </tr>
  <tr>
    <td class="tg-0pky">Our</td>
    <td class="tg-0pky">0.75</td>
    <td class="tg-0pky">0.23</td>
  </tr>
</tbody></table>

### **GPT vs LLaMA (Comparison of two LLM)**
Comparison of two LLM:
* GPT: *GPT-3.5-turbo* (generator), *GPT-4* (optimizer)
* LLaMA: *LLaMa 3.1-70b-instruct* (generator and optimizer)

<img src="https://github.com/KDmitr/study_mallm-gan/blob/main/figure/ki_2.png" alt="{{ include.description }}" width="400"/>  <img src="https://github.com/KDmitr/study_mallm-gan/blob/main/figure/mi_2.png" width="400"/> 
### Experiments under different conditions
Comparison with the number of columns: 10, 5, 2; categorical/numerical features; traditional/few-shot generation.\
LLM: *LLaMa 3.1-70b-instruct*

Conclusions from the experiments:
* The fewer columns, the better the quality
* Few-shot generation typically produces inferior outcomes compared to the traditional method
* The model performs better with numerical features than with categorical features

<img src="https://github.com/KDmitr/study_mallm-gan/blob/main/figure/ki_3.png" alt="{{ include.description }}" width="400"/>  <img src="https://github.com/KDmitr/study_mallm-gan/blob/main/figure/mi_3.png" width="400"/>
