# git commit规范说明

commit message 由type、scope、subject组成

## 示例

> ```shell
> # type(scope):subject（50个字以内）
> git commit -m 'fix(登陆模块):修复登陆后没有跳转'
> ```

## 示例说明

> **type（类型）**：这次commit类型
>
> - feat：添加新功能；模块的第一次或模块完成后的最后一次试用；开发中每次都是用wip
> - fix：bug修复
> - wip：工作进行中，还没有彻底完成；
> - docs：仅修改文档
> - style：修改格式（空格，格式化，样式等），对代码逻辑没有影响
> - refactor：代码重构（不是fix bug，也不是add feat，在所有功能都正常情况下用新技术或者新逻辑重构）
> - build：构建流程、外部依赖变更；比如升级npm包，修改webpack等cli工具配置文件
> - test：测试相关

> **scope**:涉及到的模块
>
> - 开发项目中，简单概括涉及到的模块（举例：登陆模块、用户个人模块等；多个模块用&连接）
> - 文档内容新增时，概括是哪一部分（举例：文章、项目等；多个模块用&连接）

> **subject**：本次提交简单描述，做了什么改动
>
> - 举例：修改登陆逻辑、新增跳转逻辑等；多个描述&连接

# 分支规范

- 要保证仓库的commit干净，不要出现无用的合并代码，试用git pull --rebase提交
- 本地处理好冲突，有多余commit，注意合并后在push

[demo](./文章/文章.md)