# The Win Ratio and Generalised Pairwise Comparisons: A Detailed Review

## Introduction
This document explores two key statistical methods—**the Win Ratio** and **Generalised Pairwise Comparisons (GPC)**—by synthesising insights from the following papers:

1. **Pocock et al. (2012)**: Introduction of the **Win Ratio** for analysing composite endpoints in clinical trials.
2. **Buyse (2010)**: Development of **Generalised Pairwise Comparisons (GPC)** as an extension of Wilcoxon-based statistical tests.
3. **Verbeeck et al. (2023)**: Application of **GPC in rare disease trials**, highlighting its advantages over the **Win Ratio**.

---

## What is the Win Ratio?

The **Win Ratio**, introduced by **Pocock et al. (2012)**, is a statistical method designed to analyse **composite endpoints** in clinical trials. It prioritises **clinically important events**, providing a more meaningful measure of treatment effect compared to conventional **time-to-first-event** analyses.

### Computation
The Win Ratio is calculated using **pairwise comparisons** between patients in the treatment and control groups:

1. **Pairwise Comparisons**: Each treatment patient is compared with each control patient.
2. **Prioritisation of Outcomes**: The highest-priority event (eg., **death**) is considered first. If a comparison can be made, the pair is counted.
3. **Secondary Outcomes**: If the highest-priority event does not distinguish the pair, the next-ranked event (eg., **hospitalisation**) is assessed.
4. **Classification**:
   - **Win**: If the treatment patient has a better outcome.
   - **Loss**: If the control patient has a better outcome.
   - **Tie**: If neither patient has a clearly better outcome.
5. **Win Ratio Calculation**:

   $$
   \text{Win Ratio} = \frac{\text{Number of Wins}}{\text{Number of Losses}}
   $$

### Worked Example
Consider a heart failure trial evaluating **cardiovascular (CV) death** and **hospitalisation**. Suppose:

- **100 wins** for treatment (later deaths in treatment vs. control).
- **80 losses** for treatment (earlier deaths in treatment vs. control).
- **50 hospitalisation-based wins**.
- **40 hospitalisation-based losses**.

The Win Ratio is computed as:

$$
\text{Win Ratio} = \frac{(100 + 50)}{(80 + 40)} = \frac{150}{120} = 1.25
$$

This suggests a **25% higher likelihood of better outcomes with treatment**.

---

## Generalised Pairwise Comparisons (GPC) and Comparison with the Win Ratio

### Overview of GPC
**Generalised Pairwise Comparisons (GPC)**, introduced by **Buyse (2010)**, extends the Wilcoxon-Mann-Whitney U-test to compare treatment groups across **multiple prioritised outcomes**. Unlike the **Win Ratio**, GPC provides a **net treatment benefit (NTB)**, a probability-based measure of treatment effect.

### Key Differences Between GPC and the Win Ratio

1. **Handling of Ties**  
   - **Win Ratio** ignores ties, potentially overestimating treatment effects.  
   - **GPC** explicitly accounts for ties, leading to **more reliable statistical inferences**.

2. **Outcome Types**  
   - **Win Ratio** is primarily designed for **time-to-event data**.  
   - **GPC** is **more flexible**, accommodating **continuous, binary, and time-to-event outcomes**.

3. **Statistical Interpretation**  
   - **Win Ratio** provides a **relative measure** (ie., a ratio of wins to losses).  
   - **GPC** provides an **absolute probability measure** (Net Treatment Benefit), which is **more intuitive for clinicians**.

4. **Regulatory Use**  
   - **Win Ratio** has **limited regulatory adoption**.  
   - **GPC** has been **accepted by the FDA and EMA** for drug approval in **rare disease trials** (Verbeeck et al., 2023).

### Application to Rare Diseases (Verbeeck et al., 2023)
Verbeeck et al. (2023) highlight **GPC’s advantages in small-sample trials**, particularly for **rare diseases**. Their findings show that GPC:
- **Improves statistical power** by integrating **patient-reported outcomes (PROs)**.
- Can be applied to **crossover designs**, unlike the **Win Ratio**.
- Outperforms traditional composite endpoint methods in capturing **treatment benefits**.

---

## Conclusion

The **Win Ratio** and **Generalised Pairwise Comparisons (GPC)** are both valuable tools for analysing composite endpoints. The **Win Ratio** provides a **simplified, clinically meaningful measure**, but **ignores ties** and is **limited to time-to-event outcomes**. **GPC is more flexible**, handling **multiple outcome types**, and is increasingly used in **regulatory settings**.

For clinical trials where **prioritisation of multiple outcomes** is needed, **GPC is often the superior choice**.

---

## References

Buyse, M. (2010). Generalised pairwise comparisons of prioritised outcomes in the two-sample problem. *Statistics in Medicine, 29*(30), 3245-3257. https://doi.org/10.1002/sim.3923  

Pocock, S. J., Ariti, C. A., Collier, T. J., & Wang, D. (2012). The Win Ratio: A new approach to the analysis of composite endpoints in clinical trials based on clinical priorities. *European Heart Journal, 33*(2), 176-182. https://doi.org/10.1093/eurheartj/ehr352  

Verbeeck, J., Dirani, M., Bauer, J. W., Hilgers, R. D., Molenberghs, G., & Nabbout, R. (2023). Composite endpoints, including patient-reported outcomes, in rare diseases. *Orphanet Journal of Rare Diseases, 18*, 262. https://doi.org/10.1186/s13023-023-02819-x  
