## **问题记录与解决方案**

## **1.模型路径识别错误**

## 问题：本地模型路径被误判为 Hugging Face Hub 仓库 ID，报HFValidationError

## 解决步骤：

## 确认模型本地路径存在（如/home/user/vla\_model），用ls /home/user/vla\_model验证文件完整性（需包含config.json、权重文件等）；

## 重新更改路径。 **2.config.json语法错误**

## 问题：报JSONDecodeError，提示 “单引号未用双引号”“多余逗号”“包含注释”。

## 解决步骤：

## 用nano config.json打开文件，删除所有//注释（JSON 不支持注释） ；

## 替换所有单引号为双引号（如'model\_type'→"model\_type"）；

## 删除最后一个元素后的多余逗号（如["a", "b",]→["a", "b"]）；

## 验证合法性：python3 -m json.tool config.json（无报错则正确）。

## **缺少各种环境**

## 问题：出现缺失transformers等等 。

## 解决步骤：依据大模型来逐步排查安装。

## **缺少 libero 库**

## 问题：ModuleNotFoundError: No module named 'libero'

## 解决步骤；

## 安装 Git for Windows

## 验证安装：git --version

## 配置全局用户名和邮箱：git config --global user.name "YourGitHubUsername"

## git config --global user.email "YourGitHubEmail"

# **二、学习心得**

## **1.技术能力提升**

## 依赖管理优化：学会conda与pip协同使用：conda管理基础环境，pip安装项目包。pip install -e .的可编辑模式大幅提升开发效率，Pillow替代PIL的实践让我关注库的更新动态。

## **2.问题解决方法论**

## 三层分析法：现象→原因→方案：遇ModuleNotFoundError先查pip list，区分网络 / 环境 / 版本问题，通过官方文档验证方案。

## 工具链活用：用git clone报错定位认证问题，tree查看目录结构，将重复操作写脚本减少错误。

## 持续沉淀分类整理问题与方案，标注关键参数（如-e模式），跟踪仓库releases掌握更新。