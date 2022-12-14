## 特别声明

- 本仓库发布的脚本及其中涉及的任何解锁和解密分析脚本，仅用于测试和学习研究，禁止用于商业用途，不能保证其合法性，准确性，完整性和有效性，请根据情况自行判断。

- 本项目内所有资源文件，禁止任何公众号、自媒体进行任何形式的转载、发布。

- 本人对任何脚本问题概不负责，包括但不限于由任何脚本错误导致的任何损失或损害。

- 间接使用脚本的任何用户，包括但不限于建立VPS或在某些行为违反国家/地区法律或相关法规的情况下进行传播, 本人对于由此引起的任何隐私泄漏或其他后果概不负责。

- 请勿将本仓库的任何内容用于商业或非法目的，否则后果自负。

- 如果任何单位或个人认为该项目的脚本可能涉嫌侵犯其权利，则应及时通知并提供身份证明，所有权证明，我们将在收到认证文件后删除相关脚本。

- 任何以任何方式查看此项目的人或直接或间接使用该项目的任何脚本的使用者都应仔细阅读此声明。本人保留随时更改或补充此免责声明的权利。一旦使用并复制了任何相关脚本或Script项目的规则，则视为您已接受此免责声明。

**您必须在下载后的24小时内从计算机或手机中完全删除以上内容**

> ***您使用或者复制了本仓库且本人制作的任何脚本，则视为 `已接受` 此声明，请仔细阅读***

## 前提说明
乐心健康刷步，蚂蚁森林轻松每天296g能量（需要自己购买乐心手环，或自购手环sn码绑定）

## 腾讯云函数部署教程
- 0.下载乐心健康APP：官方下载地址：http://www.lifesense.com/app/
- 1.从应用商店下载乐心健康App，打开软件并选择手机号登录
- 2.登录之后，点击我的->设置->账号与安全->设置密码(修改密码)，设置你自己记得住的密码
- 3.绑定自己购买的手环也可以网上购买手环sn码进行绑定）
- 4.回到App首页，点击我的->数据共享，绑定你想同步数据的项目
- 5.在腾讯云函数新建空白模板
 <img src="https://user-images.githubusercontent.com/71224625/182764842-358e3d64-b8c8-46b7-a340-f7a3c9382e31.png"/>
 
- 6.在函数代码处填入上传本仓库的lexin.py或将lexin.py中的代码复制到云函数中
   在代码最低端将自己注册的乐心健康账号密码填入相应的代码段中
      <p>----先点击部署----再点击运行----刷步成功</p>
 <img src="https://user-images.githubusercontent.com/71224625/182765394-b57055ec-24b0-4cf9-8a92-c20e66bcae89.jpg"/>
 
- 7.运行成功后需要创建定时触发，使其每天自动刷步
 <img src="https://user-images.githubusercontent.com/71224625/182765549-d8552405-7339-4470-a658-a0dd285be5fa.png"/>

## 青龙面板部署教程
- 1. 添加订阅管理
  * 青龙v2.13.+
  <img src="https://user-images.githubusercontent.com/71224625/182868238-e04d37d7-2a2f-44ed-897a-9e34d840e4c2.png"/>

  * 青龙v2.13.0之前版本使用原始拉库方法
  ```text
  ql repo https://github.com/Wyatt323/lexin.git "lexin"
  ```
 
- 2. 在脚本中填入对应数据
 <img src="https://user-images.githubusercontent.com/71224625/182869083-39d603b4-3e4c-4e94-99de-dbc8a63d1892.png"/>

- 3. 运行任务查看是否成功
 <img src="https://user-images.githubusercontent.com/71224625/182869737-ffed2ef0-a37c-4d00-9231-6651c2d2977e.png"/>
