# Feature Learning-Based Knowledge Distillation for Teacher and Student Networks

This repository contains the implementation and results of our Bachelor’s Thesis Project (BTP) on **Feature Learning-Based Knowledge Distillation**, conducted at **The LNM Institute of Information Technology, Jaipur**, under the guidance of **Dr. Lal Upendra Pratap Singh**. You can also refer this [BTP Report](https://github.com/HetPatel12/Knowledge-Distillation/blob/main/BTP-Report.pdf) and [Presentation Slides](https://github.com/HetPatel12/Knowledge-Distillation/blob/main/Feature-Learning-based-Knowledge-Distillation-to-train-Teacher-and-Student-Networks.pdf).

## Project Overview

The project explores **knowledge distillation** techniques to train lightweight **student models** guided by more complex **teacher models** for remote sensing image classification. The methodology was validated across four prominent datasets:
- **UC Merced Land Use**
- **EuroSat**
- **AID**
- **NWPU-RESISC45**

Our approach employs **nuclear norm regularization** and optimized distillation loss functions, demonstrating significant reductions in model complexity while maintaining accuracy. This makes the models suitable for **resource-constrained environments** such as drones and edge devices.

---

## Objectives and Goals
- **Knowledge Transfer**: Evaluate the effectiveness of transferring information from teacher to student models.
- **Performance Optimization**: Achieve high accuracy with minimal computational demands.
- **Dataset Analysis**: Assess performance across diverse datasets.
- **Practical Applications**: Explore applications in disaster relief, environmental monitoring, and precision agriculture.

---

## Methodology

1. **Teacher-Student Framework**: 
   - **Teacher Model**: 4-layer CNN.
   - **Student Model**: 3-layer CNN trained with a combination of distillation and dataset-specific loss functions.

2. **Nuclear Norm Regularization**: 
   - Promotes simpler and more discriminative feature representations.
   - Enhances generalization to unseen data distributions.

3. **Hyperparameter Tuning**:
   - Experimented with varying distillation loss alpha values to balance soft-label contributions.

---

## Results

- The **student model** achieved accuracy comparable to or exceeding that of the teacher model across datasets.
- **Nuclear norm regularization** effectively improved model generalization and reduced computational overhead.

| Dataset              | Teacher Accuracy (%) | Student Accuracy (%) |
|----------------------|----------------------|-----------------------|
| UC Merced Land Use   | 83                  | 86                    |
| EuroSat              | 79                  | 82                    |
| AID                  | 76                  | 78                    |
| NWPU-RESISC45        | 59                  | 62                    |

---

## Future Work

- Expanding experiments to include more diverse datasets.
- Investigating alternative regularization methods (e.g., Frobenius norm, strategic dropout).
- Refining model architectures for improved efficiency.
- Applying the framework to other domains such as **natural language processing** and **recommendation systems**.

## License

© The LNM Institute of Information Technology, Jaipur, 2024. All rights reserved.
