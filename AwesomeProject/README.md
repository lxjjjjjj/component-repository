# component-repository
config 对象可以被用来配置 scripts 的参数，例如：
{ 
    "name" : "foo",
    "config" : { "port" : "8080" }
}
有一个 start 命令，并且可以通过 npm_package_config_port 变量引用设置的 port。用户也可以通过 npm config set foo:port 8001 覆盖配置。
    