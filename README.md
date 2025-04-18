# 解决框架4.7.2安装问题：无法建立到信任根颁发机构的证书链

在尝试安装.NET Framework 4.7.2时，一些用户可能会遇到一个常见错误，即“无法建立到信任根颁发机构的证书链”。这个错误通常由于系统缺少必要的根证书引起，但不用担心，通过几个简单的步骤就能解决这个问题。

### 解决方案步骤：

1. **下载证书**：首先，你需要下载特定的证书文件（.cer格式）。此文件是解决此问题的关键，确保从可信赖来源获取。

2. **打开Microsoft Management Console (MMC)**：
   - 按下键盘上的 `Win + R` 组合键来打开“运行”对话框。
      - 输入 `mmc` 并回车，启动Microsoft Management Console。

      3. **添加管理单元**：
         - 在MMC中，选择 `文件` > `添加/删除管理单元` （或者直接按快捷键 Ctrl+M）。

         4. **配置证书管理单元**：
            - 在添加或删除管理单元窗口中，找到并双击“证书”，之后选择“添加”。
               - 当提示选择管理单元适用范围时，选择 “计算机账户”，点击“下一步”。
                  - 保持默认选项不变，继续点击直到完成向导。

                  5. **导入证书**：
                     - 回到MMC主界面，展开“证书”树状目录，找到“受信任的根证书颁发机构”下的“证书”节点。
                        - 右键点击“证书”，选择 “所有任务” > “导入”。
                           - 在导入向导中，浏览并选择你先前下载的.cer文件，跟随指引进行，默认设置通常是合适的，直至完成导入过程。

                           完成这些步骤后，你的系统应该已经成功添加了所需的根证书，从而解决了在安装.NET Framework 4.7.2时出现的证书链错误。如果之前因该错误而未能成功安装，现在可以尝试重新安装.NET Framework 4.7.2，预计问题将不再出现。

                           请确保在整个过程中仔细操作，避免证书被误导入到不正确的存储位置。这样，您就可以顺畅地完成框架的安装了。

                           ## 下载链接
                           [解决框架4.7.2安装问题无法建立到信任根颁发机构的证书链](https://pan.quark.cn/s/59724aa0d155) 

                           (备用: [备用下载](https://pan.baidu.com/s/1ozEeb3t89G9XzP5rEiIYeA?pwd=1234))

                           ## 说明

                           该仓库仅用于学习交流，请勿用于商业用途。
