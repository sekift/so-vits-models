# visual-chatgpt

https://github.com/microsoft/TaskMatrix

在colab运行，使用Tesla T4 的GPU。

copy到colab之后，按步骤build，过程出现下面问题：

1、from visual_chatgpt import * 引入，缺少mediapipe，使用  !pip install 'mediapipe' 解决

搭建好之后，在gradio中，上传图片能够成功，但是使用文字对话，报错：

```
======>Auto Resize Image...
Resize image form 800x800 to 512x512
/usr/local/lib/python3.10/dist-packages/transformers/generation/utils.py:1369: UserWarning: Using `max_length`'s default (20) to control the generation length. This behaviour is deprecated and will be removed from the config in v5 of Transformers -- we recommend using `max_new_tokens` to control the maximum length of the generation.
  warnings.warn(
Processed ImageCaptioning, Input Image: image/ab0636dd.png, Output Text: a man with brown hair and a green jacket

Processed run_image, Input image: image/ab0636dd.png
Current state: [('![](file=image/ab0636dd.png)*image/ab0636dd.png*', '收到。  ')]
Current Memory: 
Human: 提供一张名为 image/ab0636dd.png的图片。它的描述是: a man with brown hair and a green jacket。 这些信息帮助你理解这个图像，但是你应该使用工具来完成下面的任务，而不是直接从我的描述中想象。 如果你明白了, 说 "收到". 
AI: 收到。  
history_memory:
Human: 提供一张名为 image/ab0636dd.png的图片。它的描述是: a man with brown hair and a green jacket。 这些信息帮助你理解这个图像，但是你应该使用工具来完成下面的任务，而不是直接从我的描述中想象。 如果你明白了, 说 "收到". 
AI: 收到。  , n_tokens: 18


> Entering new AgentExecutor chain...
Yes
Action: Replace Something From The Photo
Action Input: image/ab0636dd.png, brown hair, blue hairimage_path=image/ab0636dd.png, to_be_replaced_txt= brown hair
/usr/local/lib/python3.10/dist-packages/transformers/modeling_utils.py:881: FutureWarning: The `device` argument is deprecated and will be removed in v5 of Transformers.
  warnings.warn(
/usr/local/lib/python3.10/dist-packages/torch/utils/checkpoint.py:31: UserWarning: None of the inputs have requires_grad=True. Gradients will be None
  warnings.warn("None of the inputs have requires_grad=True. Gradients will be None")
```

100%

50/50 [00:09<00:00, 5.55it/s]

```
Traceback (most recent call last):
  File "/usr/local/lib/python3.10/dist-packages/gradio/routes.py", line 488, in run_predict
    output = await app.get_blocks().process_api(
  File "/usr/local/lib/python3.10/dist-packages/gradio/blocks.py", line 1431, in process_api
    result = await self.call_function(
  File "/usr/local/lib/python3.10/dist-packages/gradio/blocks.py", line 1109, in call_function
    prediction = await anyio.to_thread.run_sync(
  File "/usr/local/lib/python3.10/dist-packages/anyio/to_thread.py", line 33, in run_sync
    return await get_asynclib().run_sync_in_worker_thread(
  File "/usr/local/lib/python3.10/dist-packages/anyio/_backends/_asyncio.py", line 877, in run_sync_in_worker_thread
    return await future
  File "/usr/local/lib/python3.10/dist-packages/anyio/_backends/_asyncio.py", line 807, in run
    result = context.run(func, *args)
  File "/usr/local/lib/python3.10/dist-packages/gradio/utils.py", line 706, in wrapper
    response = f(*args, **kwargs)
  File "/content/TaskMatrix/visual_chatgpt.py", line 1520, in run_text
    res = self.agent({"input": text.strip()})
  File "/usr/local/lib/python3.10/dist-packages/langchain/chains/base.py", line 168, in __call__
    raise e
  File "/usr/local/lib/python3.10/dist-packages/langchain/chains/base.py", line 165, in __call__
    outputs = self._call(inputs)
  File "/usr/local/lib/python3.10/dist-packages/langchain/agents/agent.py", line 503, in _call
    next_step_output = self._take_next_step(
  File "/usr/local/lib/python3.10/dist-packages/langchain/agents/agent.py", line 420, in _take_next_step
    observation = tool.run(
  File "/usr/local/lib/python3.10/dist-packages/langchain/tools/base.py", line 71, in run
    raise e
  File "/usr/local/lib/python3.10/dist-packages/langchain/tools/base.py", line 68, in run
    observation = self._run(tool_input)
  File "/usr/local/lib/python3.10/dist-packages/langchain/agents/tools.py", line 17, in _run
    return self.func(tool_input)
  File "/content/TaskMatrix/visual_chatgpt.py", line 1408, in inference_replace_sam
    updated_image = self.inpaint(prompt=replace_with_txt, image=image_pil,
  File "/content/TaskMatrix/visual_chatgpt.py", line 1180, in __call__
    update_image = self.inpaint(prompt=prompt, image=image.resize((width, height)),
  File "/usr/local/lib/python3.10/dist-packages/torch/autograd/grad_mode.py", line 27, in decorate_context
    return func(*args, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py", line 983, in __call__
    image, has_nsfw_concept = self.run_safety_checker(image, device, prompt_embeds.dtype)
  File "/usr/local/lib/python3.10/dist-packages/diffusers/pipelines/stable_diffusion/pipeline_stable_diffusion_inpaint.py", line 479, in run_safety_checker
    image, has_nsfw_concept = self.safety_checker(
  File "/usr/local/lib/python3.10/dist-packages/torch/nn/modules/module.py", line 1194, in _call_impl
    return forward_call(*input, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/torch/autograd/grad_mode.py", line 27, in decorate_context
    return func(*args, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/diffusers/pipelines/stable_diffusion/safety_checker.py", line 51, in forward
    pooled_output = self.vision_model(clip_input)[1]  # pooled_output
  File "/usr/local/lib/python3.10/dist-packages/torch/nn/modules/module.py", line 1194, in _call_impl
    return forward_call(*input, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/transformers/models/clip/modeling_clip.py", line 941, in forward
    return self.vision_model(
  File "/usr/local/lib/python3.10/dist-packages/torch/nn/modules/module.py", line 1194, in _call_impl
    return forward_call(*input, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/transformers/models/clip/modeling_clip.py", line 866, in forward
    hidden_states = self.embeddings(pixel_values)
  File "/usr/local/lib/python3.10/dist-packages/torch/nn/modules/module.py", line 1194, in _call_impl
    return forward_call(*input, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/transformers/models/clip/modeling_clip.py", line 195, in forward
    patch_embeds = self.patch_embedding(pixel_values)  # shape = [*, width, grid, grid]
  File "/usr/local/lib/python3.10/dist-packages/torch/nn/modules/module.py", line 1194, in _call_impl
    return forward_call(*input, **kwargs)
  File "/usr/local/lib/python3.10/dist-packages/torch/nn/modules/conv.py", line 463, in forward
    return self._conv_forward(input, self.weight, self.bias)
  File "/usr/local/lib/python3.10/dist-packages/torch/nn/modules/conv.py", line 459, in _conv_forward
    return F.conv2d(input, weight, bias, self.stride,
RuntimeError: Input type (torch.cuda.HalfTensor) and weight type (torch.cuda.FloatTensor) should be the same
```



问题解决：

https://github.com/microsoft/TaskMatrix/issues/420

Setting
 self.torch_dtype = torch.float32  instead
 self.torch_dtype = torch.float16 if 'cuda' in device else torch.float32
 in all model class initialization @ visual_chatgpt.py worked on RTX 3090 CUDA 11.7!

结果：

把visual_chatgpt.py文件中近10个这样的语句都替换之后，运行使用成功。



已经复现，但是效果不如意，而且token消耗非常快，是文字的数十倍。而且效果貌似也不太好。