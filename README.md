# chatglm-fintune
基于chatglm3-6b微调的大模型应用

# 微调输出过程

![微调loss](https://github.com/zjs1994/chatglm-fintune/assets/41611224/0e67a541-54c4-4820-bc8a-a699721b2913)

# 修改basic_demo/web_demo_gradio_finetuned.py文件，使用推理后的模型启动
ModelType = Union[PreTrainedModel, PeftModelForCausalLM]
TokenizerType = Union[PreTrainedTokenizer, PreTrainedTokenizerFast]

MODEL_PATH = os.environ.get('MODEL_PATH', '/data1/jeason/ChatGLM3-main/finetune_demo/output/checkpoint-3000')
TOKENIZER_PATH = os.environ.get("TOKENIZER_PATH", MODEL_PATH)
<img width="1194" alt="image" src="https://github.com/zjs1994/chatglm-fintune/assets/41611224/c9fc8f6e-7bcc-4b07-b983-d798bcf70ff4">

# 使用微调后的模型进行推理
![image](https://github.com/zjs1994/chatglm-fintune/assets/41611224/7da029a3-2c36-4dec-8fbb-40d53557ffa8)


