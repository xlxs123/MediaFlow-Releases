# MediaFlow Releases

此公开仓库仅托管 MediaFlow 正式 Windows 资产与稳定版更新清单。源码、测试与构建工作流在 [xlxs123/MediaFlow](https://github.com/xlxs123/MediaFlow)。

版本资产见 [Releases](https://github.com/xlxs123/MediaFlow-Releases/releases)。只有已正式发布的版本才是在线更新源；草稿仍处于授权核验阶段。

固定渠道路径：`releases/latest/download/manifest.json`。清单格式 2 使用 Ed25519；`manifest.sig` 是同一签名的独立核验 JSON，与 `signature.json` 字节一致。客户端验证清单内嵌签名和完整 ZIP 大小/SHA-256 后才部署到独立版本目录。

正式 key_id `mediaflow-stable-2026-01`；raw 公钥 SHA-256 `fa54ae69f7a14184681a810dd33bd28cc4cdbe2870ff58db75df48503caf11d1`。旁置公钥仅供独立核对，不会通过未签名网络响应为客户端新增可信根。私钥不在此仓库、任何发布资产或普通 CI 中。

应用源码使用其原有 MIT；二进制包中的第三方组件保留各自许可证，并应按对应版本的第三方源码说明重建。请同时保留完整发布目录的 `licenses` 与 `tools`。发布完成前不声称已有可用稳定资产。
