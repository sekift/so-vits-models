# so-vits-models
 收集有关so-vits-svc、TTS的各种模型、应用以及录音有关的软件。



## 1 模型

|      | 人物                | 地址                                                         | 训练步数 | 版本    | 有无kmeans |
| ---- | ------------------- | ------------------------------------------------------------ | -------- | ------- | ---------- |
| 1    | 周杰伦              | https://huggingface.co/kevinwang676/jay                      | 10k      | <=4.0   | +          |
| 1    | 周杰伦              | https://huggingface.co/kevinwang676/guesswho                 | 3.25k    | <=4.0   | -          |
| 2    | 孙燕姿              | https://huggingface.co/kevinwang676/syz_ai                   | 6.125    | <=4.0   | -          |
| 3    | 许嵩                | https://huggingface.co/kevinwang676/vae                      | 10k      | <=4.0   | +          |
| 3    | 许嵩                | https://huggingface.co/kevinwang676/sovits-vae               | 10k      | <=4.0   | -          |
| 4    | 在玹                | https://huggingface.co/baebad/jay                            | 未知     | <=4.0   | -          |
| 5    | 星野爱              | https://huggingface.co/LynMeow/HoshinoAI_So-vits-svc-4.0     | 40k      | 4.0     | +          |
| 6    | Billie Joe          | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/BillieJoe | 24k      | 4.0     | -          |
| 7    | Chris Cornell       | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/ChrisCornell | 7.4k     | 4.0     | -          |
| 8    | Dave Mustaine       | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/DaveMustaine | 71.8k    | 4.0     | -          |
| 9    | David Bowie         | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/DavidBowie | 7.2k     | 4.0     | -          |
| 10   | Eddie Vedder        | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/EddieVedder | 48.8k    | 4.0     | -          |
| 11   | Eric Cartman        | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/EricCartman | 10.2k    | 4.0     | -          |
| 12   | James Hetfield      | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/JamesHetfield | 49.6k    | 4.0     | -          |
| 13   | Lady Gaga           | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/LadyGaga | 14.4k    | 4.0     | -          |
| 14   | Liam Gallagher      | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/LiamGallagher | 18.4k    | 4.0     | -          |
| 15   | Marina Sena         | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/MarinaSena | 8.8k     | 4.0     | -          |
| 16   | Noel Gallagher      | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/NoelGallagher | 15.2k    | 4.0     | -          |
| 17   | Parapper TheRapper  | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/ParapperTheRapper | 15.4k    | 4.0     | -          |
| 18   | Phil Anselmo        | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/PhilAnselmo | 25k      | 4.0     | -          |
| 19   | Stevie Ray Vaughan  | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/StevieRayVaughan | 6.2k     | 4.0     | -          |
| 20   | Tim Maia            | https://huggingface.co/marcoc2/so-vits-svc-4.0-models/tree/main/TimMaia | 319.2k   | 4.0     | -          |
| 21   | 动物/动画(10+)      | https://huggingface.co/RAYTRAC3R/so-vits-svc-4.0             | -        | 4.0     | -          |
| 22   | Tim Cook            | https://huggingface.co/Sucial/so-vits-svc4.1-Tim_Cook        | -        | 4.1     | +          |
| 23   | 小马宝莉动画(20+)   | https://huggingface.co/therealvul/so-vits-svc-4.0            | -        | 4.0     | +          |
| 24   | 小马宝莉动画(20+)   | https://huggingface.co/therealvul/so-vits-svc-3.0            | -        | 3.0     | -          |
| 25   | 原神角色(5)         | https://huggingface.co/kaze-mio/so-vits-genshin              | 10k+     | 4.1     | +          |
| 26   | 崩坏角色(3)         | https://huggingface.co/kaze-mio/so-vits-star-rail            | 20k+     | 4.0     | +          |
| 27   | Tokai Teio          | https://huggingface.co/Kree/so-vits-svc4.0-Tokai-Teio/tree/main/Tokai-Teio | 531.2k   | 4.0     | +          |
| 28   | 二次元()            | https://huggingface.co/TachibanaKimika/so-vits-svc-4.0-models | 1k+      | 4.0     | -          |
| 29   | Biden               | https://huggingface.co/Nardicality/so-vits-svc-4.0-models/tree/main/Biden20k | 20k      | 4.0     | -          |
| 30   | Obama               | https://huggingface.co/Nardicality/so-vits-svc-4.0-models/tree/main/Obama50k | 50k      | 4.0     | -          |
| 31   | Trump               | https://huggingface.co/Nardicality/so-vits-svc-4.0-models/tree/main/Trump18.5k | 18.5k    | 4.0     | -          |
| 32   | 安倍晋三            | https://huggingface.co/LynMeow/AbeShinzo_So-vits-svc-4.1_v2.3.6 | 25k      | 4.1     | +          |
| 33   | Shirayuki Noa       | https://huggingface.co/LynMeow/ShirayukiNoa_So-vits-svc-4.0/ | 49.6k    | 4.0     | +          |
| 34   | Takahashi Rie       | https://huggingface.co/hanachirusato/TakahashiRie_so-vits-svc | 291      | 4.0     | -          |
| 35   | 电影人物            | https://huggingface.co/Amo/so-vits-svc-4.0_GA                | 45k+     | 4.0     | +          |
| 36   | Shigure Tokina      | https://huggingface.co/yasyune/Shigure_Tokina_so-vits-svc-4.0v1 | 59.2k    | 4.0     | -          |
| 37   | Kurage Kikoto       | https://huggingface.co/yasyune/Kurage_Kikoto__Mahiro_Kikoto_so-vits-svc-4.0v1/tree/main/Kurage_Kikoto | 19.2k    | 4.0     | -          |
| 38   | Mahiro Kikoto       | https://huggingface.co/yasyune/Kurage_Kikoto__Mahiro_Kikoto_so-vits-svc-4.0v1/tree/main/Mahiro_Kikoto | 23.2k    | 4.0     | -          |
| 39   | 未知                | https://huggingface.co/ciferecavivon/so-vits-svc3.0_big      | 180k     | 4.0     | -          |
| 40   | Suga Yoshihide      | https://huggingface.co/AbeShinzo0708/so_vits_svc4_SugaYoshihide | 10.4k    | 4.0     | -          |
| 41   | Love Live(10+)      | https://huggingface.co/YazawaSunrise/LoveLive-so-vits-svc    | 280k     | 4.0     | -          |
| 41   | Love Live           | https://huggingface.co/Habuki/kanata-konoe-so-vits-svc-model | 7.2k     | 4.0     | -          |
| 42   | 未知(3)             | https://huggingface.co/kuuhaku1314/so-vits-svc-4.0           | 10k+     | 4.0     | -          |
| 43   | niel                | https://huggingface.co/mikefizzy/so-vits-svc                 | 183k     | 4.0     | -          |
| 44   | azusa               | https://huggingface.co/Rafxeed/so-vits-svc-models            | 30k      | 4.0     | -          |
| 45   | ru-saya             | https://huggingface.co/fnx/so-vits-svc-4.0-ru-saya           | 10k      | 4.0     | -          |
| 46   | 生田绘梨花          | https://huggingface.co/jed351/so-vits                        | 127.2k   | 4.0     | -          |
| 47   | 池田瑛纱            | https://huggingface.co/jed351/so-vits                        | 31.2k    | 4.0     | -          |
| 48   | 声优(15+1)          | https://huggingface.co/Itoifi/so-vits-svc-acg-models         | 60k+     | 3.0/4.0 | -          |
| 49   | LAIN?               | https://huggingface.co/SuCicada/Lain-so-vits-svc-4.0         | 256.8k   | 4.0     | +          |
| 50   | 佐仓杏子            | https://huggingface.co/SuCicada/SuTTS/tree/main/sakurakyouko | 100k     | 4.0     | -          |
| 51   | mikisayaka          | https://huggingface.co/SuCicada/SuTTS/tree/main/mikisayaka   | 50k      | 4.0     | -          |
| 52   | caster/morgen/saber | https://huggingface.co/xgdhdh/so-vits-svc-4.0                | 60k+     | 4.0     | -          |
| 53   | Larry_Koopa         | https://huggingface.co/JosueCr4ft/Larry_Koopa_so-vits-4-0    | 1.28k    | 4.0     | -          |
| 54   | jokowi              | https://huggingface.co/zhen182/jokowi-so-vits-svc-modelv1    | 2.08k    | 4.0     | -          |
| 55   | 崩坏                | https://huggingface.co/HaHaiko/SOVITS-SVC-Hi3-Characters     | 1.92k    | 4.0     | -          |
| 56   | ATRI                | https://huggingface.co/2DIPW/ATRI_SoVITS                     | 39.2k    | 4.0     | +          |
| 56   | ATRI                | https://huggingface.co/gb16001/sovits4.1_ATRI                | 40k      | 4.1     | +          |
| 57   | Madobe Family(5)    | https://huggingface.co/FinalIroha/Madobe_Family_SoVITS4.0_Model | 101.4k   | 4.0     | +          |
| 58   | 龙王的工作(8)       | https://huggingface.co/FinalIroha/Ryuuou_no_Oshigoto_SoVITS4.1_Model | 9.6k     | 4.1     | +          |
| 59   | 韩国明星(11)        | https://huggingface.co/Shashashasha                          | 6k+      | 4.0     | -          |
| 60   | Praat脚本           | http://www.globalaccentchinese.com/soft.php                  | -        | -       | 有用       |
| 61   | paimon              | https://huggingface.co/gb16001/soVits4.1_paimon              | 41.6k    | 4.1     | +          |
| 62   | 周杰伦、48系        | https://huggingface.co/sekift/so-vits-svc                    | >10k     | 4.1     | +，可用    |
| 63   | ATRI                | https://huggingface.co/gb16001/sovits4.1_ATRI/tree/main      | 40k      | 4.1     | +，        |
| 64   | 李志                | [NanjingLiZhi](https://huggingface.co/souljoy/so-vits-svc-NanjingLiZhi/tree/main) | 10k      | 4.0     |            |
| 64   | mayday              | https://huggingface.co/souljoy/so-vits-svc-mayday/tree/main  | 10k      | 4.0     |            |
| 65   | Tokoyami Towa       | https://huggingface.co/Zuiho/sovits_tokoyami_towa            | 139k     | 4.0     |            |
| 66   |                     |                                                              |          |         |            |



## 2 应用

|      | 人物          | 地址                                                         | 项目                   | 是否可用 | 限制                                                         |
| ---- | ------------- | ------------------------------------------------------------ | ---------------------- | -------- | ------------------------------------------------------------ |
| 1    | 周杰伦        | https://huggingface.co/spaces/wangxiuliang01/Voice-Cloning-for-Bilibili | so-vits等              | +        |                                                              |
| 2    | B站、孙燕姿等 | https://kevinwang676-test-1.hf.space/                        | so-vits                | +        |                                                              |
| 3    | 清/bilibili   | https://kevinwang676-voice-cloning-for-bilibili.hf.space/    | so-vits                | +        |                                                              |
| 3    | 音乐生成      | https://huggingface.co/spaces/facebook/MusicGen              | music-gen              | +        |                                                              |
| 3    | 音乐生成      | https://huggingface.co/spaces/Surn/UnlimitedMusicGen         | UnlimitedMusicGen      | +        | 经常错误                                                     |
| 4    | 文/音         | https://huggingface.co/spaces/SuCicada/Lain-vits             | TTS/vits               | +        |                                                              |
| 5    | 碧蓝档案(141) | https://huggingface.co/spaces/FrankZxShen/so-vits-svc-models-ba | so-vits                | +        |                                                              |
| 6    | 公主连结(161) | https://huggingface.co/spaces/FrankZxShen/so-vits-svc-models-pcr | so-vits                | +        |                                                              |
| 7    | datealive(4)  | https://huggingface.co/spaces/Wanlau/sovits-4.0_datealive    | so-vits                | +        | 限制45s                                                      |
| 8    | 文转音        | https://kevinwang676-personal-tts.hf.space/                  | so-vits                | +        | 无                                                           |
| 9    | 变声器        | https://huggingface.co/spaces/Ricecake123/RVC-demo           | rvc                    | +        | 限制90s，只有一个zundamon                                    |
| 10   | 图生视频      | https://huggingface.co/spaces/vinthony/SadTalker             | SadTalker              | +        | 等得久                                                       |
| 11   | 图/视频生视频 | https://huggingface.co/spaces/CVPR/Image-Animation-using-Thin-Plate-Spline-Motion-Model | SadTalker              | -        | 不可用                                                       |
| 12   | 歌词转歌曲    | https://huggingface.co/spaces/zlc99/M4Singer                 | SVS                    | +        | 可用                                                         |
| 13   | 人声转木吉他  | https://huggingface.co/spaces/lj1995/vocal2guitar            | RVC                    | +        |                                                              |
| 14   | 低配SVC       | https://github.com/yxlllc/DDSP-SVC                           | SVC                    | +        | 可用，在CPU上使用SVC                                         |
| 15   | 声音转换套件  | [sing例子](https://huggingface.co/spaces/amphion/singing_voice_conversion) , [Github](https://github.com/open-mmlab/Amphion) ,[论文](https://arxiv.org/abs/2312.09911) , [首页](https://openmmlab.com/) | TTS、SVC、SVS、so-vits | ++       | amphion家族，例子使用有时候慢并卡死，可多次操作。有和声的部分仍然未解决，训练时间过段，效果不明显。 |
| 16   |               |                                                              |                        |          |                                                              |



## 3 工具

|      | 名字         | 链接                                                         | 说明             |
| ---- | ------------ | ------------------------------------------------------------ | ---------------- |
| 1    | GoldWave     | https://www.newasp.com/soft/17851.html<br>https://www.goldwavechina.cn/ | 数字音频编辑软件 |
| 2    | 在线分离     | https://vocalremover.org/zh/                                 | 在线分离5声道    |
| 3    | 即时调音软件 | https://resource.dreamtonics.com.cn/download/                | PRO要钱          |
| 4    | Praat        | https://www.fon.hum.uva.nl/praat/download_win.html           | 语言软件         |
| 5    | 格式转换     | https://cloudconvert.com/mp4-to-mp3                          | 提供多种格式转换 |



## 4 网站应用

|      | 名字     | 链接                  | 说明           |
| ---- | -------- | --------------------- | -------------- |
| 1    | chordify | https://chordify.net/ | 在线歌曲乐谱提 |
| 2    |          |                       |                |

