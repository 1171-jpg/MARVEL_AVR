# MARVEL_AVR
Github repo for [MARVEL: Multidimensional Abstraction and Reasoning through Visual Evaluation and Learning](https://arxiv.org/abs/2404.13591) <br> 
Website link: [MARVEL](https://marvel770.github.io/) <br>
Huggingface link: [MARVEL](https://huggingface.co/datasets/kianasun/MARVEL)

# TL;DR
A new comprehensive benchmark, MARVEL, evaluates multi-modal large language models' abstract reasoning abilities in six patterns across five different task configurations, revealing significant performance gaps between human and SOTA MLLMs.
![image](https://github.com/1171-jpg/MARVEL_AVR/blob/main/image/demo.drawio.png)

# Folder
Json_data folder: sub-folder for each puzzle image and corresponding label json file.

Panel_data folder: images of each panel in each puzzle.

Marvel folder: images of 770 puzzles composed of six core knowledge patterns, geometric and abstract shapes, and five different task configurations


# Marvel
marvel_label.json
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
- **c_perception_answer_tuple**:
```python
(
    context part panel number,
    choices part panel number,
    whole puzzle panel number,
)
```


### If you find MARVEL useful for your work please cite:
```
@article{jiang2024marvel,
  title={MARVEL: Multidimensional Abstraction and Reasoning through Visual Evaluation and Learning},
  author={Jiang, Yifan and Zhang, Jiarui and Sun, Kexuan and Sourati, Zhivar and Ahrabian, Kian and Ma, Kaixin and Ilievski, Filip and Pujara, Jay},
  journal={arXiv preprint arXiv:2404.13591},
  year={2024}
}
```
