# AI Model Economics Benchmark

### Evaluating AI Model Accuracy, Latency, and Cost for Enterprise Finance Workflows

**Eric Mersch | Technology CFO | AI Finance & Automation**

## Executive Summary

This project examines the economics of deploying artificial intelligence models in enterprise financial operations.

The objective is to evaluate three critical dimensions of AI model performance:

- **Accuracy:** How reliably does the model classify financial transactions?
- **Latency:** How quickly does the model complete a workflow?
- **Cost:** What is the inference cost per 1,000 transactions?

## Initial Benchmark: OpenAI vs. TypeSafe Jev

A controlled experiment evaluated 50 synthetic invoices using two AI models. Each invoice was classified into one of three categories: Approve, Review, or Hold.

| Metric | OpenAI GPT-5.6 | TypeSafe Jev |
|---|---:|---:|
| Classification accuracy | 100% | 94% |
| Correct classifications | 50/50 | 47/50 |
| Inference cost per 1,000 invoices | $0.162 | $0.023 |
| Total benchmark workflow latency | 104.6 seconds | 0.6 seconds |

## Key Observations

**1. Cost efficiency**

TypeSafe Jev demonstrated approximately 7.1 times lower inference cost per invoice.

**2. Processing speed**

The observed end-to-end benchmark latency was substantially lower for Jev. Results are specific to the tested configurations and should not be interpreted as a universal model speed comparison.

**3. Accuracy trade-offs**

OpenAI classified all 50 synthetic invoices correctly, while Jev classified 47 correctly. The smaller sample limits conclusions about production reliability.

## Financial Implications

AI model selection should be based on total workflow economics rather than inference cost alone.

Relevant considerations include:

- Cost per successfully processed transaction
- Human review and exception-handling costs
- Financial impact of incorrect classifications
- Processing capacity and operating latency
- Data security, auditability, and compliance

## Future Development

Planned extensions include:

- Larger evaluation datasets
- Human-in-the-loop exception economics
- Risk-adjusted cost comparisons
- Automated benchmark reporting
- Additional AI model comparisons

## Methodology and Limitations

The initial experiment used 50 synthetic invoices. The results are preliminary and should not be generalized to production financial workflows without further testing.

Detailed evaluation datasets, executable code, and reproducibility documentation may be added in subsequent releases.

---

*This repository explores how financial executives can evaluate AI infrastructure decisions using quantitative operating and economic metrics.*
