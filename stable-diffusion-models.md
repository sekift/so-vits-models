# stable-diffusion-models

 收集有关stable diffusion的各种模型、应用。



## 1 应用

|      | 名称                                                         | 功能                  | 论文                                                         | Github                                                       | 使用情况                                                     |
| ---- | ------------------------------------------------------------ | --------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1    | [SD-XL](https://huggingface.co/spaces/hysts/SD-XL)           | 文生图                | [2307.01952](https://arxiv.org/abs/2307.01952)               | [github](https://github.com/stability-ai/generative-models)  | +                                                            |
| 2    | [Llama 2 7B Chat](https://huggingface.co/spaces/huggingface-projects/llama-2-7b-chat) | chatbot, LLM, Llama 2 | [2307.09288](https://arxiv.org/abs/2307.09288)               | [github](https://github.com/facebookresearch/llama)          | +，中文效果差了点                                            |
| 3    | [ Zeroscope V2](https://huggingface.co/spaces/hysts/zeroscope-v2) | 文生视频              |                                                              |                                                              | +，只有3s，效果一般                                          |
| 4    | [ Shap-E](https://huggingface.co/spaces/hysts/Shap-E)        | 文转3D，图转3D        | [2305.02463](https://arxiv.org/abs/2305.02463)               | [github](https://github.com/openai/shap-e)                   | +，效果差                                                    |
| 5    | [ ControlNet V1.1](https://huggingface.co/spaces/hysts/ControlNet-v1-1) | 文生图、图生图        | [2302.05543](https://arxiv.org/abs/2302.05543)               | [github](https://github.com/lllyasviel/ControlNet) [github](https://github.com/lllyasviel/ControlNet-v1-1-nightly) | +，繁忙                                                      |
| 6    | [Rerender](https://huggingface.co/spaces/Anonymous-sub/Rerender) | 视频生视频            |                                                              |                                                              | ++，可用，目前只有封面+3s                                    |
| 7    | [ModelScope Text To Video Synthesis](https://huggingface.co/spaces/damo-vilab/modelscope-text-to-video-synthesis) | 文生视频              | [2303.08320](https://arxiv.org/abs/2303.08320)               | [github](https://github.com/modelscope/modelscope)           | 2-3s，效果一般                                               |
| 8    | [ELITE](https://huggingface.co/spaces/ELITE-library/ELITE)   | 文生图                | [2302.13848](https://arxiv.org/abs/2302.13848)               | [github](https://github.com/csyxwei/ELITE)                   | +，可以把选中的物和prompt提示的结合在一起，可用              |
| 9    | [DDNM-HQ](https://huggingface.co/spaces/hysts/DDNM-HQ)       | 照片修复、彩色        | [2303.00354](https://arxiv.org/abs/2303.00354) [2212.00490](https://arxiv.org/abs/2212.00490) | [github](https://github.com/wyhuai/DDNM/tree/main/hq_demo)   | demo不可用，但colab应该可以                                  |
| 10   | [ControlNet + Anything v4.0](https://huggingface.co/spaces/hysts/ControlNet-with-Anything-v4) | 文生图、图生图        | [2302.05543](https://arxiv.org/abs/2302.05543)               | [github](https://github.com/lllyasviel/ControlNet)           | demo不可用                                                   |
| 11   | [ODISE](https://huggingface.co/spaces/xvjiarui/ODISE)        | 多物体识别            | [2303.04803](https://arxiv.org/abs/2303.04803)               | [github](https://github.com/NVlabs/ODISE)                    | 可用，结果为英文，+++                                        |
| 12   | [ BLIP2 with transformers](https://huggingface.co/spaces/hysts/BLIP2-with-transformers) | 识物                  | [2301.12597](https://arxiv.org/abs/2301.12597)               | [github](https://github.com/salesforce/LAVIS/tree/main/projects/blip2) | demo不可用                                                   |
| 13   | [Tune-A-Video Inference](https://huggingface.co/spaces/Tune-A-Video-library/Tune-A-Video-inference) | 文生视频、视频生视频  | [2212.11565](https://arxiv.org/abs/2212.11565)               | [github](https://github.com/showlab/Tune-A-Video)            | demo不可用，colab也不可用，[issue](https://github.com/showlab/Tune-A-Video/issues/69) |
| 14   | [Tune-A-Video Training UI](https://huggingface.co/spaces/Tune-A-Video-library/Tune-A-Video-Training-UI) | 同上                  | [2212.11565](https://arxiv.org/abs/2212.11565)               | [github](https://github.com/showlab/Tune-A-Video)            | 同上                                                         |
| 15   | [CutLER](https://huggingface.co/spaces/facebook/CutLER)      | 物体捕捉，没有识别    | [2301.11320](https://arxiv.org/abs/2301.11320)               | [github](https://github.com/facebookresearch/CutLER)         | demo可用                                                     |
| 16   | [MaskCut](https://huggingface.co/spaces/facebook/MaskCut)    | 物体捕捉，没有识别    | [2301.11320](https://arxiv.org/abs/2301.11320)               | [github](https://github.com/facebookresearch/CutLER)         | 同上                                                         |
| 17   | [Multiresolution Textual Inversion](https://huggingface.co/spaces/hysts/multiresolution-textual-inversion) | 文生图                | [2211.17115](https://arxiv.org/abs/2211.17115)               | [github](https://github.com/giannisdaras/multires_textual_inversion) | 效果觉得一般                                                 |
| 18   | [CogVideo](https://huggingface.co/spaces/THUDM/CogVideo)     | 文生视频              | [2205.15868](https://arxiv.org/abs/2205.15868)               | [github](https://github.com/THUDM/CogVideo)                  | demo可用，排队太久                                           |
| 19   | [AnimeGANv3 PortraitSketch](https://huggingface.co/spaces/hysts/AnimeGANv3_PortraitSketch) | 图生图，仅素描        |                                                              | [github](https://github.com/TachibanaYoshino/AnimeGANv3)     | 仅素描，效果还可                                             |
| 20   | [MangaLineExtraction_PyTorch](https://huggingface.co/spaces/hysts/MangaLineExtraction_PyTorch) | 漫画线提取，去色      |                                                              | [github](https://github.com/ljsabc/MangaLineExtraction_PyTorch) | 效果还行，只提取边线，去掉颜色，功能单一                     |
| 21   | [ViTPose Video](https://huggingface.co/spaces/hysts/ViTPose_video) | 姿态估计              | [2204.12484](https://arxiv.org/abs/2204.12484)               | [github](https://github.com/ViTAE-Transformer/ViTPose)       | 可用，通用的姿态估计开源工具箱                               |
| 21   | [ViTPose](https://huggingface.co/spaces/Gradio-Blocks/ViTPose) | 同上                  | [2204.12484](https://arxiv.org/abs/2204.12484)               | [github](https://github.com/ViTAE-Transformer/ViTPose)       | 同上                                                         |
| 22   | [Text2Human](https://huggingface.co/spaces/hysts/Text2Human) | 图文生人物            | [2205.15996](https://arxiv.org/abs/2205.15996)               | [github](https://github.com/yumingj/Text2Human)              | 可用，慢了点                                                 |
| 23   | [MMDetection](https://huggingface.co/spaces/hysts/mmdetection) | 多物体识别            |                                                              | [github](https://github.com/open-mmlab/mmdetection)          | 可用                                                         |
| 24   | [ HairCLIP](https://huggingface.co/spaces/Gradio-Blocks/HairCLIP) | 换发型与颜色          | [2112.05142](https://arxiv.org/abs/2112.05142)               | [github](https://github.com/wty-ustc/HairCLIP)               | 可用，较快，++                                               |
| 25   | [Portrait Style Transfer](https://huggingface.co/spaces/Gradio-Blocks/DualStyleGAN) | 换衣服                | [2203.13248](https://arxiv.org/abs/2203.13248)               | [github](https://github.com/williamyang1991/DualStyleGAN)    | 不是很明朗                                                   |
| 26   | [StyleGAN-Human](https://huggingface.co/spaces/Gradio-Blocks/StyleGAN-Human) | 换衣服                | [2204.11823](https://arxiv.org/abs/2204.11823)               | [github](https://github.com/stylegan-human/StyleGAN-Human)   | 不是很明朗                                                   |
| 27   | [StyleGAN-Human Interpolation](https://huggingface.co/spaces/hysts/StyleGAN-Human-Interpolation) | 生成衣服              | [2204.11823](https://arxiv.org/abs/2204.11823)               | [github](https://github.com/stylegan-human/StyleGAN-Human)   | 功能固定，GAN                                                |
| 28   | [StyleGAN-Human](https://huggingface.co/spaces/hysts/StyleGAN-Human) | 生成衣服              | [2204.11823](https://arxiv.org/abs/2204.11823)               | [github](https://github.com/stylegan-human/StyleGAN-Human)   | 功能固定，GAN                                                |
| 29   | [GAN-Control](https://huggingface.co/spaces/hysts/gan-control) | 换年龄、发型、发色    | [2101.02477](https://arxiv.org/abs/2101.02477)               | [github](https://github.com/amazon-research/gan-control)     | 功能固定，GAN                                                |
| 30   | [Manga OCR](https://huggingface.co/spaces/hysts/Manga-OCR)   | 漫画配字识别          |                                                              | [github](https://github.com/kha-white/manga-ocr)             | 可用                                                         |
| 31   | [Mediapipe Pose Estimation](https://huggingface.co/spaces/hysts/mediapipe-pose-estimation) | 面部识别              | [2006.10204](https://arxiv.org/abs/2006.10204)               | [github](https://github.com/google/mediapipe)                | 可用                                                         |
| 32   | [Mediapipe Face Detection](https://huggingface.co/spaces/hysts/mediapipe-face-detection) | 面部识别              | [1907.05047](https://arxiv.org/abs/1907.05047)               | [github](https://github.com/google/mediapipe)                | 可用                                                         |
| 33   | [ Mediapipe Face Mesh](https://huggingface.co/spaces/hysts/mediapipe-face-mesh) | 面部识别              | [1907.06724](https://arxiv.org/abs/1907.06724)               | [github](https://github.com/google/mediapipe)                | 可用                                                         |
| 34   | [Anime2Sketch](https://huggingface.co/spaces/hysts/Anime2Sketch) | 漫画线提取，去色      | [2104.05703](https://arxiv.org/abs/2104.05703)               | [github](https://github.com/Mukosame/Anime2Sketch)           | 可用，简单                                                   |
| 35   | [TADNE Image Viewer](https://huggingface.co/spaces/hysts/TADNE-image-viewer) | 生成动漫图            |                                                              |                                                              | 可用                                                         |
| 36   | [ TADNE Interpolation](https://huggingface.co/spaces/hysts/TADNE-interpolation) | 生成动漫图            |                                                              |                                                              | 可用                                                         |
| 37   | [Insightface SCRFD](https://huggingface.co/spaces/hysts/insightface-SCRFD) | 人脸检测              | [2105.04714](https://arxiv.org/abs/2105.04714)               | [github](https://github.com/deepinsight/insightface/tree/master/detection/scrfd) | 可用                                                         |
| 38   | [Insightface Person Detection](https://huggingface.co/spaces/hysts/insightface-person-detection) | 人脸检测              | [2105.04714](https://arxiv.org/abs/2105.04714)               | [github](https://github.com/deepinsight/insightface/tree/master/examples/person_detection) | 可用                                                         |
| 39   | [ Self-Distilled StyleGAN](https://huggingface.co/spaces/hysts/Self-Distilled-StyleGAN) | 相似图片集            | [2202.12211](https://arxiv.org/abs/2202.12211)               | [github](https://github.com/self-distilled-stylegan/self-distilled-internet-photos) | GAN                                                          |
| 40   | [StyleGAN2](https://huggingface.co/spaces/hysts/StyleGAN2)   | 相似图片集            | [1912.04958](https://arxiv.org/abs/1912.04958)               | [github](https://github.com/NVlabs/stylegan3)                | GAN                                                          |
| 41   | [Projected GAN](https://huggingface.co/spaces/hysts/projected_gan) | 相似图片集            | [2111.01007](https://arxiv.org/abs/2111.01007)               | [github](https://github.com/autonomousvision/projected_gan)  | GAN                                                          |
| 42   | [StyleGAN3](https://huggingface.co/spaces/hysts/StyleGAN3)   | 相似图片集            | [2106.12423](https://arxiv.org/abs/2106.12423)               | [github](https://github.com/NVlabs/stylegan3)                | GAN                                                          |
| 43   | [StyleGAN-XL](https://huggingface.co/spaces/hysts/StyleGAN-XL) | 相似图片集            | [2202.00273](https://arxiv.org/abs/2202.00273)               | [github](https://github.com/autonomousvision/stylegan_xl)    | GAN                                                          |
| 44   | [1adrianb Face Alignment](https://huggingface.co/spaces/hysts/1adrianb-face-alignment) | 人脸检测              | [1703.07332](https://arxiv.org/abs/1703.07332)               | [github](https://github.com/1adrianb/face-alignment)         |                                                              |
| 45   | [ Portrait Style Transfer with DualStyleGAN](https://huggingface.co/spaces/hysts/DualStyleGAN) | 变脸                  | [2203.13248](https://arxiv.org/abs/2203.13248)               | [github](https://github.com/williamyang1991/DualStyleGAN)    | 转为各种风格的漫画脸，++                                     |
| 46   | [StyleSwin](https://huggingface.co/spaces/hysts/StyleSwin)   | 相似图片集            | [2112.10762](https://arxiv.org/abs/2112.10762)               | [github](https://github.com/microsoft/StyleSwin)             | GAN                                                          |
| 47   | [Age Estimation APPA REAL](https://huggingface.co/spaces/hysts/age-estimation-APPA-REAL) | 人脸检测              |                                                              | [github](https://github.com/yu4u/age-estimation-pytorch)     |                                                              |
| 48   | [Anime_face_landmark_detection](https://huggingface.co/spaces/hysts/anime_face_landmark_detection) | 卡通人脸检测          |                                                              | [github](https://github.com/kanosawa/anime_face_landmark_detection) |                                                              |
| 49   | [Lbpcascade_animeface](https://huggingface.co/spaces/hysts/lbpcascade_animeface) | 卡通人脸检测          |                                                              | [github](https://github.com/nagadomi/lbpcascade_animeface)   |                                                              |
| 50   | [Yolov5_anime](https://huggingface.co/spaces/hysts/yolov5_anime) | 卡通人脸检测          |                                                              | [github](https://github.com/zymk9/yolov5_anime)              |                                                              |
| 51   | [Bizarre Pose Estimator Segmenter](https://huggingface.co/spaces/hysts/bizarre-pose-estimator-segmenter) | 卡通轮廓识别          | [2108.01819](https://arxiv.org/abs/2108.01819)               | [github](https://github.com/ShuhongChen/bizarre-pose-estimator) |                                                              |
| 52   | [ Yet Another Anime Segmenter](https://huggingface.co/spaces/hysts/Yet-Another-Anime-Segmenter) | 卡通轮廓识别          |                                                              | [github](https://github.com/zymk9/Yet-Another-Anime-Segmenter) |                                                              |
| 53   | [Bizarre Pose Estimator Tagger](https://huggingface.co/spaces/hysts/bizarre-pose-estimator-tagger) | 人物动作识别          | [2108.01819](https://arxiv.org/abs/2108.01819)               | [github](https://github.com/ShuhongChen/bizarre-pose-estimator) | ++                                                           |
| 54   | [ DeepDanbooru](https://huggingface.co/spaces/hysts/DeepDanbooru) | 人物动作识别          |                                                              | [github](https://github.com/KichangKim/DeepDanbooru)         |                                                              |
| 55   | [Danbooru Pretrained](https://huggingface.co/spaces/hysts/danbooru-pretrained) | 人物动作识别          |                                                              | [github](https://github.com/RF5/danbooru-pretrained)         |                                                              |
| 56   | [ StyleGAN3 Anime Face Generation (exp002)](https://huggingface.co/spaces/hysts/stylegan3-anime-face-exp002) | 生成动漫              |                                                              |                                                              | GAN                                                          |
| 57   | [StyleGAN3 Food101](https://huggingface.co/spaces/hysts/stylegan3-food101) | 生成动漫              |                                                              |                                                              | GAN                                                          |
| 58   | [StyleGAN3 Anime Face Generation (exp001)](https://huggingface.co/spaces/hysts/stylegan3-anime-face-exp001) | 生成动漫              |                                                              |                                                              | GAN                                                          |
| 59   | [latent-upscaler](https://huggingface.co/stabilityai/sd-x2-latent-upscaler) | 无损放大              |                                                              |                                                              |                                                              |
| 60   |                                                              |                       |                                                              |                                                              |                                                              |
|      |                                                              |                       |                                                              |                                                              |                                                              |
|      |                                                              |                       |                                                              |                                                              |                                                              |
|      |                                                              |                       |                                                              |                                                              |                                                              |
