# A/B Testing — Designing the Data-Generating Process

## Objective

I examined how random assignment, uncertainty analysis, and power planning affect causal conclusions from experiments.

## Methodology

- I analyzed the randomized LaLonde job-training experiment with 185 trainees and 260 controls.
- I compared the experimental estimate with an estimate using a simulated observational comparison group.
- I conducted a permutation test with 9,999 shuffled assignments.
- I calculated a bootstrap BCa confidence interval for the average treatment effect.
- I examined statistical power and required sample sizes for several earnings effects.
- I analyzed Day-1 retention for 90,189 players in the Cookie Cats A/B test.
- I calculated the retention difference, ran a permutation test, and constructed a bootstrap confidence interval.
- I wrote and checked a function that calculates the sample size required for 80% power.

## Key Findings

Trainees earned an average of $1,794.34 more than randomized controls. The permutation p-value was 0.0046, and the 95% confidence interval ranged from $575.18 to $3,262.37.

When the same trainees were compared with a simulated observational group, the estimated effect became −$14,784.45. The sign reversal demonstrated how selection bias can overwhelm the true treatment effect.

In Cookie Cats, Day-1 retention was 44.82% with the gate at level 30 and 44.23% with the gate at level 40. The difference was 0.59 percentage points, with a permutation p-value of 0.0752. The 95% confidence interval ranged from −0.07 to 1.23 percentage points.

A new test designed to detect the observed Cookie Cats difference with 80% power would require approximately 111,193 players per group. The results do not provide strong evidence that moving the gate to level 40 improves Day-1 retention.
