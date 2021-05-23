# Getting Started with Debug React@17.0.2

1. 下载[react源码](https://github.com/facebook/react.git)

2. 新建项目, 暴露配置
```
npx create-react-app hello-react
yarn eject
```

3. src下新建react, 复制源码的packages到该目录下

4. 修改配置和导出：[引入alias、环境变量、HostConfig、ReactSharedInternals](https://zhuanlan.zhihu.com/p/336933386)

5. 修改invariant函数
```
// 提前返回，避免抛错
if(condition) return
```

6.  webpack配置中关闭eslint
```
// const disableESLintPlugin = process.env.DISABLE_ESLINT_PLUGIN === 'true';
const disableESLintPlugin = true;
```

7. 修改index.js引入方式
```
import * as React from 'react';
import * as ReactDOM from 'react-dom';
```


#### 参考
[react源码调试环境搭建](https://zhuanlan.zhihu.com/p/336933386)
