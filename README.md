# HelpXiaoAi
帮助小爱同学长脑子

通过 小米公共平台 获取你家小爱同学 输入 信息，将输入信息 抛给 GPT 进行处理并获得返回，将组织结果（可在集成豆包TTS增加音色）在 通过小米公共平台 “让” 小爱同学 读出来，完成 集成小爱和GPT的流程。

部署项目：https://github.com/idootop/mi-gpt

部署位置：家里 群辉

准备：



遇到的问题：

 1、国内 docker镜像不能访问
    -- 通过配置proxy 下载。
    
 2、国外openai 无法充值
   -- https://dash.302.ai ，注册送 1$ 按量付费。
   
 3、我想白嫖API，质量其次
   -- 3.1 gemini
 ```
 google gemini 目前是免费调用的，如果白嫖党想用 MIGPT 通过openai API（格式）访问可以：
1、https://aistudio.google.com/app/apikey   注册一个API token；
2、注册 CloudFlare，白嫖worker资源。
3、准备一个自己的域名，托管到 CloudFlare DNS上（实现从国内访问，不走proxy）。
4、https://github.com/PublicAffairs/openai-gemini?tab=readme-ov-file （实现将gemini 接口转成 openai API 供 MIGPT调用）。---- 有guide 可以一步步完成 在CloudFlare worker部署。
5、在CloudFlare中，给worker 加一个 自己的域名（就可以实现 国内调用国外gemini接口了）
6、修改 MIGPT  .env 文件，将地址改成 自己域名、token 使用 google gemini token（第一步）、模型 自己list 查看哪个好用）

我家小米音响试了，还不错。国内访问 gemini 代理 大概 1.2s 以内的样子。
```
  -- 3.2 deepseek v3 ，国内类 openai api接口，可以适配，赠送credit


有需要的小伙伴参考，不差钱 不太看重质量的 可以参考哈



一些图片：
<img width="1203" alt="image" src="https://github.com/ryanlxb/HelpXiaoAi/assets/28553693/21881af7-e0c9-41c3-9b28-de08026c734f">

![image](https://github.com/ryanlxb/HelpXiaoAi/assets/28553693/9ab32d9d-355b-4888-96a5-333aa636425a)

<img width="862" alt="image" src="https://github.com/ryanlxb/HelpXiaoAi/assets/28553693/a78a7d54-fe82-4626-8f04-78665fa3faf8">

<img width="1046" alt="image" src="https://github.com/ryanlxb/HelpXiaoAi/assets/28553693/5ef885ae-31dc-4d74-90e6-8c9c86f89c76">





