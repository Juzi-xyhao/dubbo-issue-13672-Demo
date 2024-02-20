# 启动路径
demo-consumer模块的org.example.Main类
要复现这个[issue](https://github.com/apache/dubbo/issues/13672)只要在org/apache/dubbo/config/spring/ReferenceBean.java最后一段的if语句里加上“&& SCOPE_LOCAL.equals(serviceBean.getScope())“即可
