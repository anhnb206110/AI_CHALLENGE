# AI_CHALLENGE

Sử dụng mô hình ngôn ngữ để trả lời các câu hỏi ở mức độ bài thi toán SAT.

Tinh chỉnh mô hình `flan-t5-base` để trả lời cho các câu hỏi trắc nghiệm và sử dụng `gpt-3.5-turbo-instruct` cho các câu hỏi trả lời đáp án.

## Fine-tune

- Model: `flan-t5`
- Evaluate trên tổng số 7287 câu hỏi trắc nghiệm

|  | Epochs |Accuracy |
|--|--|--|
|`flan-t5-small` | 0 |19.32|
|`flan-t5-base` | 0 |26.86|
|`flan-t5-large` | 0 |27.67|
|`flan-t5-base-mathqa_v1`|3 |30.57|
|`flan-t5-base-mathqa_v2`|5 |34.07|
|`flan-t5-base-mathqa_v3`|8 |39.60|