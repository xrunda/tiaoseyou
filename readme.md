## 切换运行环境
```
source venv/bin/activate
```

## 准备autotrain环境
```
pip install autotrain_advanced
autotrain setup
```

## 运行微调命令
```
autotrain dreambooth \
    --model stabilityai/stable-diffusion-xl-base-1.0 \
    --image-path Andrea/ \
    --prompt "oil painting by Andrea style" \
    --resolution 1024 \
    --batch-size 1 \
    --num-steps 200 \
    --fp16 \
    --gradient-accumulation 4 \
    --lr 1e-4 \
    --project-name model_Andrea

```