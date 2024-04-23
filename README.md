# MARVEL_AVR
Github repo for MARVEL: Multidimensional Abstraction and Reasoning through Visual Evaluation and Learning



# Marvel
final_label.json
- **id**: image id
- **pattern**: general concept pattern
- **task_configuration**: the task configuration of the puzzle
- **avr_question**: abstract visual reasoning question
- **answer**
- **explanation**: explanation of the pattern within the puzzle
- **f_perception_question**: fine-grained perception question annotated by human
- **f_perception_answer**
- **f_perception_distractor**
- **c_perception_question_tuple**: coarse-grained perception question based on panels of image
```python
(
    "coarse-grained perception question on the puzzle's context part",
    "coarse-grained perception question on the puzzle's choices part",
    "coarse-grained perception question on the whole puzzle"
)
```
- **l_perception_answer_tuple**:
```python
(
    context part panel number,
    choices part panel number,
    whole puzzle panel number,
)
```

