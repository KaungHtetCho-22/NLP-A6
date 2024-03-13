# NLP-A6
NLP assignment from AIT

**Kaung Htet Cho (st124092)**

## Task1
### Student Layer Initialization

- implemented top_k_layers {1,2,3,4,5,6} from 12-layers teacher to 6-layers student.
- implemented bottom_k_layers {7,8,9,10,11,12} from 12-layers teacher to 6-layers student.
- implemented odd_layers {1,3,5,7,9,11} from 12-layers teacher to 6-layers student.
- implemented even_layers {2,4,6,8,10,12} from 12-layers teacher to 6-layers student.


## Task2
### Evaluation of distilled student BERT

| Student layer | Training loss | Validation loss | Validation accuracy |
|----------------|-------------|---------------|-------------------|
| Top-K layer     |      0.2623    |   0.7968  |    0.6910 |
| Bottom-K layer |    0.2569      |     0.7968     |  0.6910  |
| Odd layer |    0.2568      |    0.7968        | 0.6910    |
| Even layer |        0.2567  |     0.7968       |   0.6910  |

### Difficulty

Limited GPU Memory: Deep learning models, especially large ones like the 12-layer teacher model, require significant GPU memory for training. When the model and data exceed the available memory capacity, CUDA out of memory errors occur.

### Analysis

Task Dependency: The effectiveness of initial layer selection can vary depending on the task. Layers that are optimal for one task may not be as effective for another. Therefore, selecting layers based solely on their position in the model architecture may not always yield the best results.

Improvements: Task-specific analysis should be conducted to determine the most suitable layers for distillation. Techniques such as task-aware layer selection or dynamic layer selection based on task characteristics can be explored to improve performance across different tasks.
