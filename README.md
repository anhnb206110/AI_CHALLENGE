# AI_CHALLENGE

Sử dụng mô hình ngôn ngữ để trả lời các câu hỏi ở mức độ bài thi toán SAT.

Tinh chỉnh mô hình `flan-t5-base` để trả lời cho các câu hỏi trắc nghiệm và sử dụng `gpt-3.5-turbo-instruct` cho các câu hỏi trả lời đáp án.

## Fine-tune

- Model: `flan-t5`
- Evaluate trên tổng số 7287 câu hỏi trắc nghiệm

|  |Paramaters | Epochs |Accuracy |
|--|--|--|--|
|`flan-t5-small`|77M| 0 |19.32|
|`flan-t5-base` |248M| 0 |26.86|
|`flan-t5-large`|783M| 0 |27.67|
|`flan-t5-base-mathqa_v1`|248M|3 |30.57|
|`flan-t5-base-mathqa_v2`|248M|5 |34.07|
|`flan-t5-base-mathqa_v3`|248M|8 |39.60|