# Strategy-Based Warm Starting
Python replication of "Strategy-Based Warm Starting for Regret Minimization in Games", Noam Brown &amp; Tuomas Sandholm 2016

paper: https://www.cs.cmu.edu/~noamb/papers/16-AAAI-Strategy-Based-TR.pdf

# Result

Figure 1 from the paper (random 100x100 matrix games, warm-starting cumulative regrets each iteration from the average policy):

![figure 1](fig1.png)

Also tried doing the same experiment as Figure 1, but with RM+. RM+ improves the results without warm-starting, but not with warm-starting? Maybe I did something wrong:

![figure 1, but with RM+](fig1_plus.png)

# Notes on the paper

I think there are some typos in the paper: 

In the section "Warm-starting Algorithm", in the middle of left column, page 4, I'm guessing

Define $\upsilon'^\sigma_i(z)$ for $z \in Z$ as $\pi^\sigma_{-i}u_i(z)$.

should be 

Define $\upsilon'^\sigma_i(z)$ for $z \in Z$ as $\pi^\sigma_{-i}(z)u_i(z).$

Similarly, near the end of the section "Choosing Substitute Counterfactual Values", I think 

In particular, $\pi^\sigma_{-i}(\Delta(I))^2$ in (16) acts as a bound on ...

should be

In particular, $\pi^\sigma_{-i}(I)(\Delta(I))^2$ in (16) acts as a bound on...

# Citation

```bibtex
@inproceedings{brown2016strategy,
  title={Strategy-based warm starting for regret minimization in games},
  author={Brown, Noam and Sandholm, Tuomas},
  booktitle={Proceedings of the AAAI Conference on Artificial Intelligence},
  volume={30},
  number={1},
  year={2016}
}
```
