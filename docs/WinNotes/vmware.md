### 优化VMware虚拟机性能，解决运行卡顿

> 虚拟机「VMware」对电脑配置要求较高，一些配置比较低的用户使用起来会比较卡顿，虽然你可以降低虚拟机系统的配置，不过「VMware」本身对硬件资源占用也是蛮大的，所以本文教大家优化 VMware 虚拟机性能。

#### 禁用内存页面修整

- 打开你的虚拟机系统 - 编辑虚拟机设置 - 选项 - 高级 - `禁用内存页面修整`。
- 禁用后可以解决运行虚拟机磁盘容易占用100%的问题。

#### 调整优先级

- 打开你的虚拟机系统 - 编辑虚拟机设置 - 选项 - 高级 - 进程优先级 - 抓取的输入内容，选择`高`。

#### 调整虚拟机内存分配

- 虚拟机菜单 - 编辑 - 首选项 - 内存，选择`调整所有虚拟内存使其适应预留的主机`。
- 这样可以让虚拟机只用物理内存，不会去读取虚拟内存，减少硬盘读取占用。

#### 远程虚拟机硬件加速

- 如果你远程方式操作虚拟机系统，遇到操作反应延迟、缓慢，可以尝试开启远程虚拟机硬件加速功能。
- 虚拟机菜单 - 编辑 -首选项 - 显示 - `远程虚拟机的硬件加速`。
