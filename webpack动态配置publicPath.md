### webpack动态配置publicPath

#### 
- 多套环境部署
- 代码一致
- cdn路径不同
- 避免重复构建
#### 
```text
__webpack_public_path__ = path;
```