# netty-research

- **sun.misc找不到**

  把JDK设置为8，JDK11删除了该sum.misc

- **io.netty.util.collection找不到**

  - 该类在common模块上，需要在该common文件夹上执行以下代码

    ```
    mvn clean install
    ```

  - 同时maven的mirror设置为默认，启动vpn连接网络
  - 其中如果pom文件有因为IDEA而多添加了设置JDK版本为8的`<plugin>`，需要**删除掉**