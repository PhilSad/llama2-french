# llama2-french

wip

https://huggingface.co/blog/llama2#fine-tuning-with-peft

https://huggingface.co/datasets/PhilSad/Instruct-fr-merged


```bash
!python trl/examples/scripts/sft_trainer.py \
    --model_name meta-llama/Llama-2-7b-chat-hf \
    --dataset_name PhilSad/Instruct-fr-merged-1k \
    --load_in_4bit \
    --use_peft \
    --batch_size 4 \
    --gradient_accumulation_steps 2 \
    --log_with wandb \
    --output_dir=llama2-7b-chat-french-1k
```
