# FoG compared to full size BRO and SimBa
<p>
  <img src="https://github.com/nothingbutbut/ICML-full_size/blob/main/h1-run-performance.png" alt="h1-run" style="width:49%; float:left; margin-right:1%;">
  <img src="https://github.com/nothingbutbut/ICML-full_size/blob/main/h1-walk-performance.png" alt="h1-walk" style="width:49%; float:left; margin-left:1%;">
</p>
<p style="clear:both; font-size:18px; margin-top:20px;">
  This experiment was conducted to compare FoG with BRO, SimBa and TD-MPC2 that have larger model size. More detailedly, we use depth=10 for both BRO and SimBa, which gives them a total of ~42M parameters. That is almost twice as big as the largest FoG(fully expanded) model with ~21M parameters. This will ensure that BRO and SimBa will not be limited by the model size, and use more computation compared to FoG. For TD-MPC2, we use 19M parameters version given in their original paper. The results show that FoG is still able to outperform these methods in terms of sample efficiency and final performance. The results are shown in the figure above.

  It's worth noting that while these baselines claim to be scalable in parameter size, TD-MPC2 and BRO seem to achieve similar or even worse performance compared to their default model size. Only SimBa gets performance improvement in h1-walk(but not in h1-run). which means that comparing FoG to these methods with their default sizes is decent.
  All experiments are conducted with 5 seeds(3 seeds for TD-MPC2).
</p>
