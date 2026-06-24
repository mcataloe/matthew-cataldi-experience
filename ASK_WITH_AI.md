# Query This Repository With an AI Assistant

This repository is structured so an AI assistant can evaluate Matthew Cataldi's experience using explicit evidence rather than résumé keyword matching alone.

## Recommended procedure

Provide the repository URL to the AI assistant and instruct it to use only information contained in this repository for claims about Matthew's experience.

Ask the assistant to:

1. Cite the relevant file and section for every material conclusion.
2. Distinguish direct experience from adjacent or transferable experience.
3. Preserve contribution language such as led, designed, implemented, evaluated, supported, and participated.
4. State when a requirement is unsupported or uncertain.
5. Avoid inferring sole ownership, production scale, business impact, or technical depth that is not documented.
6. Treat repeated descriptions as one body of evidence rather than multiple independent proofs.
7. Note limitations recorded in `evidence/claims.yaml`.

## General evaluation prompt

```text
Use only the information in this repository to evaluate Matthew Cataldi's experience.

For every conclusion:
- cite the relevant file and section;
- classify the evidence as direct, adjacent, unsupported, or unknown;
- preserve the documented contribution level;
- identify any important limitation or missing evidence;
- do not infer experience, ownership, scale, or outcomes that are not explicitly supported.
```

## Job-description comparison prompt

```text
Compare Matthew Cataldi's documented experience in this repository with the job description below.

Return:
1. strongest areas of direct fit;
2. adjacent or transferable experience;
3. unsupported or unclear requirements;
4. likely hiring-manager objections;
5. the best evidence to discuss in an interview;
6. an overall fit assessment that separates evidence from inference.

Cite the repository file and section supporting each conclusion. Do not upgrade supporting participation into ownership.

[PASTE JOB DESCRIPTION]
```

## Technical-depth prompt

```text
What evidence in this repository supports Matthew Cataldi's experience with [TOPIC]?

Organize the answer by project. For each project, identify:
- the problem context;
- Matthew's documented contribution;
- technologies or patterns involved;
- whether the evidence is direct or adjacent;
- limitations or boundaries on the claim.
```

## Useful questions

- What evidence supports Matthew's Staff Platform Engineer positioning?
- What distributed-systems reliability patterns has he applied?
- Has he directly led GitLab or internal developer platform modernization?
- What evidence supports Kubernetes and EKS experience, and where are the limits?
- What cloud architecture work has he led across AWS, Azure, and GCP?
- What experience does he have with AI-assisted systems and data platforms?
- Which projects best demonstrate cross-functional technical leadership?
- Where would a hiring manager reasonably probe for more depth?

## Interpretation rule

A plausible connection is not the same as documented experience. When the repository does not support a claim, the correct answer is that the evidence is absent or incomplete.
