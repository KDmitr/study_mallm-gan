# study_mallm-gan
The effectivness of the algorithm for generating MALLM-GAN data was investigated.\
Original paper: Ling, Yaobin et al. “MALLM-GAN: Multi-Agent Large Language Model as Generative Adversarial Network for Synthesizing Tabular Data.” [ArXiv abs/2406.10521 (2024): n. pag.](https://arxiv.org/pdf/2406.10521)\
\
**Repeating the experiments described in the article**
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

**GPT vs LLaMA (Comparison of two LLM)**
