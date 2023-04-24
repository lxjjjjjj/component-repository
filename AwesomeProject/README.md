# component-repository
## package.json config 
package.json config 对象可以被用来配置 scripts 的参数，例如：
```
{ 
    "name" : "foo",
    "config" : { "port" : "8080" }
}
```
有一个 start 命令，并且可以通过 npm_package_config_port 变量引用设置的 port。用户也可以通过 npm config set foo:port 8001 覆盖配置。

## cz-customizable 作为 commitizen 插件
cz-customizable将首先在您附近的项目根目录中查找名为.cz-config.js或的文件.config/cz-config.js package.json
如果没有找到配置，它将在您的主目录中查找.cz-config.jsor 或 or.config/cz-config.js
或者在您的中添加配置位置package.json。
```
"config": {
  "commitizen": { // not needed for standlone usage
    "path": "node_modules/cz-customizable"
  },
  "cz-customizable": {
    "config": "config/path/to/my/config.js"
  }
}
```
## 首次发布
npm run release -- --first-release


    