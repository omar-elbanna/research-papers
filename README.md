Research Papers

Published and accepted research papers from my work at Algoverse AI Research, mentored by researchers from Stanford University and UC Berkeley.


Papers

Prior Dominance in Audio-Visual LLMs: When Generative Models Memorize Over Reasoning Under Cross-modal Conflict

ICML 2026 — Foundations of Deep Generative Models Workshop (FoGen) & ML for Audio Workshop


We investigate where autoregressive AV-LLMs substitute memorized priors for reasoning under cross-modal conflict. Using logit lens and head shutoff ablations on VideoLLaMA 2-7B-AV across 1,281 conflict samples, we localize a consistent snap layer at 25.5 ± 1 across all model configurations — where the model commits to a learned prior before fully processing cross-modal evidence. We show that alignment-stage interventions shift answer bias without recovering grounded conflict resolution, and that InternVideo2 suffers a 32.3% accuracy drop and 17.3% instruction failure rate under contradiction.




Compositional Failure in Audio-Visual LLMs: Late-Layer Prior Dominance Under Cross-modal Conflict

ICML 2026 — Compositional Learning: Safety, Interpretability, and Agents Workshop (CompLearn)




We reframe audio-visual conflict as a compositional generalization test. Through mechanistic interpretability analysis, we identify 21 conflict-resolution heads clustered in layers 15-18, structurally upstream of the snap layer commitment point — meaning the model detects conflict early but overwrites it during generation. Three progressively stronger alignment methods (ACTC, TATI, AMD) all fail to improve compositional conflict resolution, staying near chance on a 6,300+ sample evaluation.




Key Findings


AV-LLMs commit to memorized priors at a consistent snap layer of 25.5 ± 1, regardless of alignment intervention
21 conflict-resolution heads cluster in layers 15-18, upstream of where learned priors override cross-modal computation
InternVideo2 drops 32.3% in accuracy under cross-modal conflict, with a 17.3% instruction failure rate
Alignment fine-tuning shifts answer bias without recovering grounded cross-modal reasoning
