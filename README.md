# Live2D前端API

服务器状态监控系统：[筱锋服务器状态监控](https://status.xiaolfeng.cn/)

Docs构建文档：[Live2D](https://blog.xiaolfeng.cn/doc-live2d.html)

Live2D网页前端： [前端构建](https://github.com/XiaoLFeng/live2d-widget)
* * *

快速一键使用

```code
# 正常
<script src="https://cdn.jsdelivr.net/gh/XiaoLFeng/live2d-widget@master/autoload.js"></script>
# 右边（修改了CSS）
<script src="https://cdn.jsdelivr.net/gh/XiaoLFeng/live2d-widget@masrer/autoload-right.js"></script>
```

## 使用方法

### 调取地址

* jsdelivr:

    ```code
    https://cdn.jsdelivr.net/gh/XiaoLFeng/live2d-API@latest/
    ```

* API服务

    ```code
    https://live2d.xiaolfeng.top/
    ```

### 接口调取方法

jsdelivr无法进行API调取，只能作为使用，如果需要调取请使用上方API服务，而不是jsdelivr服务

* 调用方法
    - /add/ **检测更新加缓存（正常勿需用到）**
    - /get/?id=X-Y **获取第X分组第Y号皮肤**
        - 其中分组为Live2d排列顺序
    - /rand/?id=X **根据上一个分组随即切换顺序**
    - /switch/?id=X **根据 上一分组 顺序切换**
    - /rand_textures/?id=X-Y **根据 上一皮肤 随机切换 同分组其他皮肤**
    - /switch_textures/?id=X-Y **根据 上一皮肤 顺序切换 同分组其他皮肤**

* 调用例子
    - /add/  **检测 新增皮肤 并更新 缓存列表**
    - /get/?id=1-23 **获取 分组 1 的 第 23 号 皮肤**
    - /rand/?id=1 **根据 上一分组 随机切换**
    - /switch/?id=1 **根据 上一分组 顺序切换**
    - /rand_textures/?id=1-23 **根据 上一皮肤 随机切换 同分组其他皮肤**
    - /switch_textures/?id=1-23 **根据 上一皮肤 顺序切换 同分组其他皮肤**

### 接口调用示例图片

* get
![](https://fp1.fghrsh.net/2020/08/22/1b29f437b0119dea9d2e907f6947647f.png)

* rand
![](https://fp1.fghrsh.net/2020/08/22/c2c12cd77c56f8b9b87fcf0282597397.png)

* switch
![](https://fp1.fghrsh.net/2020/08/22/c8a3b0a8179dd1c1528e62912d8dbeca.png)
