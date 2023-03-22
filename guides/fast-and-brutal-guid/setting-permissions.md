# 🌎 服务器端安装

{% hint style="info" %}
TODO:支持docker部署
{% endhint %}

## 服务器配置

以下是我使用的服务器配置，使用场景大概同时能够在线5人。

| 硬件  | 参数                                        |
| --- | ----------------------------------------- |
| CPU | AMD EPYC 7K62 48-Core（双核），主频2.6 GHZ（主频太低） |
| RAM | 4G                                        |
| 带宽  | 30Mb                                      |
| 硬盘  | 60G-ssd                                   |

## 服务端部署

### 安装java-17

<details>

<summary>Linux-ubuntu</summary>

以下是在Ubuntu 20.04上安装Java 17的步骤：

1.  打开终端并更新软件包列表：

    ```bash
    sudo apt update
    ```
2.  安装OpenJDK 17：

    ```bash
    sudo apt install openjdk-17-jdk
    ```
3.  验证Java版本：

    ```bash
    java -version
    ```

    如果一切正常，将显示Java版本信息。
4.  设置Java环境变量：

    在终端中输入以下命令：

    ```bash
    echo 'export JAVA_HOME=/opt/jdk-17' | sudo tee /etc/profile.d/java17.sh 
    echo 'export PATH=$JAVA_HOME/bin:$PATH'|sudo tee -a /etc/profile.d/java17.sh 
    source /etc/profile.d/java17.sh
    ```



现在，Java 17已经成功安装在Ubuntu 20.04上。

参考：[https://zhuanlan.zhihu.com/p/565274672](https://zhuanlan.zhihu.com/p/565274672)

</details>

<details>

<summary>Windows</summary>



</details>

### 部署服务端

<details>

<summary>Linux-ubuntu</summary>

1. 进入一个你希望放置服务器的文件夹，下载服务端。（也可以通过云盘下载后上传到服务器）

```bash
sudo curl -LO https://github.com/buggzd/JuntoFantasyWorld/releases/download/v7.5/server-v7.5.tar
```

如果出现:

```bash
Command 'curl' not found, but can be installed with
```

请安装curl，安装过程中一路按Y

```bash
sudo apt install curl
```

2. 下载后解包

```bash
sudo tar -xvf server-v7.5.tar
```

3. 进入文件夹

```bash
cd server-v7.5
```

4. 运行服务器

```bash
sudo bash run.sh
```

如果没有什么异常情况，服务器将正常启动，启动成功将显示下列文字。

```log
[12:53:00] [Server thread/INFO] [minecraft/DedicatedServer]: Done (55.036s)! For help, type "help"
```

</details>

