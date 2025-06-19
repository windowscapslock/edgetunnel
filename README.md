# 🚀 edgetunnel
这是一个基于 CF Worker 平台的脚本，在原版的基础上修改了显示 VLESS 配置信息转换为订阅内容。使用该脚本，你可以方便地将 VLESS 配置信息使用在线配置转换到 Clash 或 Singbox 等工具中。



## ⚠️ 免责声明

本免责声明适用于 GitHub 上的 “edgetunnel” 项目（以下简称“本项目”），项目链接为：https://github.com/windowscapslock/edgetunnel 。

### 用途
本项目仅供教育、研究和安全测试目的而设计和开发。旨在为安全研究人员、学术界人士及技术爱好者提供一个探索和实践网络通信技术的工具。

### 合法性
在下载和使用本项目代码时，必须遵守使用者所适用的法律和规定。使用者有责任确保其行为符合所在地区的法律框架、规章制度及其他相关规定。

### 免责
1. 作为本项目的 **二次开发作者**（以下简称“作者”），我 **windowscapslock** 强调本项目仅应用于合法、道德和教育目的。
2. 作者不认可、不支持亦不鼓励任何形式的非法使用。如果发现本项目被用于任何非法或不道德的活动，作者将对此强烈谴责。
3. 作者对任何人或组织利用本项目代码从事的任何非法活动不承担责任。使用本项目代码所产生的任何后果，均由使用者自行承担。
4. 作者不对使用本项目代码可能引起的任何直接或间接损害负责。
5. 为避免任何意外后果或法律风险，使用者应在使用本项目代码后的 24 小时内删除代码。

通过使用本项目代码，使用者即表示理解并同意本免责声明的所有条款。如使用者不同意这些条款，应立即停止使用本项目。

作者保留随时更新本免责声明的权利，且不另行通知。最新版本的免责声明将发布在本项目的 GitHub 页面上。

## 🔥 风险提示
- 通过提交虚假的节点配置给订阅服务，避免节点配置信息泄露。
- 另外，您也可以选择自行部署 [WorkerVless2sub 订阅生成服务](https://github.com/windowscapslock/WorkerVless2sub)，这样既可以利用订阅生成器的便利。
   
## 💡 如何使用?
### ⚙️ Workers 部署方法 
<details>
<summary><code><strong>「 Workers 部署文字教程 」</strong></code></summary>

1. 部署 CF Worker：
   - 在 CF Worker 控制台中创建一个新的 Worker。
   - 将 [worker.js](https://github.com/windowscapslock/edgetunnel/blob/main/_worker.js) 的内容粘贴到 Worker 编辑器中。
   - 将第 4 行 `userID` 修改成你自己的 **UUID** 。

2. 访问订阅内容：
   - 访问 `https://[YOUR-WORKERS-URL]/[UUID]` 即可获取订阅内容。
   - 例如 `https://vless.google.workers.dev/90cd4a77-141a-43c9-991b-08263cfe9c10` 就是你的通用自适应订阅地址。
   - 例如 `https://vless.google.workers.dev/90cd4a77-141a-43c9-991b-08263cfe9c10?sub` Base64订阅格式，适用PassWall,SSR+等。
   - 例如 `https://vless.google.workers.dev/90cd4a77-141a-43c9-991b-08263cfe9c10?clash` Clash订阅格式，适用OpenClash等。
   - 例如 `https://vless.google.workers.dev/90cd4a77-141a-43c9-991b-08263cfe9c10?sb` singbox订阅格式，适用singbox等。

3. 给 workers绑定 自定义域： 
   - 在 workers控制台的 `触发器`选项卡，下方点击 `添加自定义域`。
   - 填入你已转入 CF 域名解析服务的次级域名，例如:`vless.google.com`后 点击`添加自定义域`，等待证书生效即可。
# 🙏 特别鸣谢
### 💖 赞助支持 - 提供云服务器维持[订阅转换服务](https://sub.cmliussss.net/)
- [Alice Networks LTD](https://url.cmliussss.com/alice)
- [VTEXS Enterprise Cloud](https://console.vtexs.com/?affid=1532)
### 🛠 开源代码引用
- [zizifn/edgetunnel](https://github.com/zizifn/edgetunnel)
- [3Kmfi6HP/EDtunnel](https://github.com/6Kmfi6HP/EDtunnel)
- [SHIJS1999/cloudflare-worker-vless-ip](https://github.com/SHIJS1999/cloudflare-worker-vless-ip)
- [Stanley-baby](https://github.com/Stanley-baby)
- [ACL4SSR](https://github.com/ACL4SSR/ACL4SSR/tree/master/Clash/config)
- [股神](https://t.me/CF_NAT/38889)
