# Packages
用于创建 nuget包 CI/CD 模板项目

* [x] Azure Devops


## LICENSES
![GitHub](https://img.shields.io/github/license/rivenfx/Framework?color=brightgreen)
[![Badge](https://img.shields.io/badge/link-996.icu-%23FF4D5B.svg?style=flat-square)](https://996.icu/#/zh_CN)
[![LICENSE](https://img.shields.io/badge/license-Anti%20996-blue.svg?style=flat-square)](https://github.com/996icu/996.ICU/blob/master/LICENSE)

Please note: once the use of the open source projects as well as the reference for the project or containing the project code for violating labor laws (including but not limited the illegal layoffs, overtime labor, child labor, etc.) in any legal action against the project, the author has the right to punish the project fee, or directly are not allowed to use any contains the source code of this project!


## 目录结构
```
.
├── README.md 
├── LICENSE
├── RELEASE_NOTES.md  # Release信息
├── global.json    # 类库sdk版本限定
├── common.props   # 类库公用配置
├── repository_info.props  # 源代码仓库信息
├── version.props  # 类库版本信息
├── src        # 类库源码所在目录
│   └── SampleNugetPack # 示例项目
├── tests      # 单元测试所在目录
├── nupkg      # nuget打包脚本 
│   ├── common.ps1  # 公共配置
│   ├── pack.ps1    # 打包脚本
│   └── push_packages.ps1 # 推送到nuget脚本
├── docs       # 文档目录
│   └── main.md 
└── azure-pipelines.yml # azure devops 配置

``````

## 快速开始

1. 修改 README.md，修改为你项目的内容
2. 修改 global.json ，默认为限制 sdk 为 3.1，需要修改请自行修改
3. 修改 repository_info.props ，更新项目源码仓库和证书链接
4. 修改 common.props，将 Authors、PackageIconUrl、PackageProjectUrl 替换成你的信息
5. 修改 version.props，将 Version 替换成你的版本
6. 修改 nupkg/common.ps1，在 $projects 数组中增加你的项目名称
7. TODO....
