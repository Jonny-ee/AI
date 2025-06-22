# 常见大语言模型分享比较

## 1 项目简介



1. 登录并使用魔搭平台，关联阿里云账号来获得免费的CPU云计算资源；

2. 通过Jupyter Notebook进入相应的项目部署环境，完成模型的部署；

3. 针对3个不同的模型进行一些应用场景的测试，并开展不同模型之间的横向对比；



**本项目中横向对比的几个模型分别是：**

- [通义千问Qwen-7B-Chat](https://www.modelscope.cn/models/qwen/Qwen-7B-Chat/summary)

- [智谱ChatGLM3-6B](https://www.modelscope.cn/models/ZhipuAI/chatglm3-6b/summary)

- [ChatGPT-4o]

 

**应用场景样例为：**

- 请说出以下两句话区别在哪里？ 1、冬天：能穿多少穿多少 2、夏天：能穿多少穿多少

- 请说出以下两句话区别在哪里？单身狗产生的原因有两个，一是谁都看不上，二是谁都看不上

- 明明明明明白白白喜欢他，可她就是不说。 这句话里，明明和白白谁喜欢谁？

- 领导：你这是什么意思？ 小明：没什么意思。意思意思。 领导：你这就不够意思了。 小明：小意思，小意思。领导：你这人真有意思。 小明：其实也没有别的意思。 领导：那我就不好意思了。 小明：是我不好意思。请问：以上“意思”分别是什么意思。

- "植物学知识没什么用。"老师劝教室里的向日葵不要再学了。为什么老师说植物学没用？

## 2 配置流程


1. 进入命令行，本项目以linux操作系统的服务器为例：

   运行前需要配置环境。
   ```bash
   pip install -r requirement.txt

2. 下载对应的大模型

   ```
   // 智谱
   git clone https://www.modelscope.cn/ZhipuAI/chatglm3-6b.git
   ```
   ```
   // 千问
   git clone https://www.modelscope.cn/qwen/Qwen-7B-Chat.git
   ```

3. 修改测试文件：

   ```
   vi run.py
   ```
   将model_name = "/mnt/data/Qwen-7B-Chat"改为你的本地路径，

4. 开始测试

   ```
   python run.py
   ```
   

## 3 测试结果和分析
见《AI横向对比分析-2356215-郑功灿》。
