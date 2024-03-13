# NLP-A6
NLP assignment from AIT

**Kaung Htet Cho (st124092)**

## Task1
### Student Layer Initialization

- implement top_k_layers {1,2,3,4,5,6} from 12-layers teacher to 6-layers student.
- implement bottom_k_layers {7,8,9,10,11,12} from 12-layers teacher to 6-layers student.
- implement odd_layers {1,3,5,7,9,11} from 12-layers teacher to 6-layers student.
- implement even_layers {2,4,6,8,10,12} from 12-layers teacher to 6-layers student.



## Task2
### Evaluation of distilled student BERT

| Student layer | Training loss | Validation loss | Validation accuracy |
|----------------|-------------|---------------|-------------------|
| Top-K layer     |      0.2623    |   0.7968  |    0.6910 |
| Bottom-K layer |    0.2569      |     0.7968     |  0.6910  |
| Odd layer |    0.2568      |    0.7968        | 0.6910    |
| Even layer |        0.2567  |     0.7968       |   0.6910  |

| Teacher model | Training loss | Validation loss | Validation accuracy |
|----------------|-------------|---------------|-------------------|
| Teacher model     |      0.2623    |   0.7968  |    0.6910 |

