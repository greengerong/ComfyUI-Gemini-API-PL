# ComfyUI Gemini API

用于在comfyUI中调用Google Gemini API。

## 功能点

- 支持Gemini 2.0 Flash模型
- 修正图片强制宽高变形问题
- 支持api_key本地文件配置插件界面不展示，便于本地分享
- 支持api_key在开放平台界面手动输入不自动保持本地文件，便于key安全性

## 安装说明

### 方法一：手动安装

1. 将此存储库克隆到ComfyUI的`custom_nodes`目录：
   ```
   cd ComfyUI/custom_nodes
   git clone https://github.com/CY-CHENYUE/ComfyUI-Gemini-API-PL
   ```

2. 安装所需依赖：

   如果你使用ComfyUI便携版
   ```
   ..\..\..\python_embeded\python.exe -m pip install -r requirements.txt
   ```

   如果你使用自己的Python环境
   ```
   path\to\your\python.exe -m pip install -r requirements.txt
   ```


安装完成后重启ComfyUI

## 获取API密钥
**注意：**地区限制。

1. 访问[Google AI Studio](https://aistudio.google.com/apikey?hl=zh-cn)
2. 创建一个账户或登录
3. 在"API Keys"部分创建一个新的API密钥
4. 复制API密钥并粘贴到节点的api_key参数中（只需首次输入，之后会自动保存）


本项目fork自[ComfyUI-Gemini-API](https://github.com/CY-CHENYUE/ComfyUI-Gemini-API)，感谢原作者的贡献。