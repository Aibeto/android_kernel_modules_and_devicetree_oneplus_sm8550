# 支持说明

此仓库是 [android_kernel_oneplus_sm8550](https://github.com/Aibeto/android_kernel_oneplus_sm8550) 的子模块

主仓库的 `scripts/setup-tree.sh` 会把 `vendor/` 和 `oplus/` 链接到这里

PPS 适配的更改在分支 `feat/16.0/oneplus_11/pps`（从 `oneplus/sm8550_b_16.0.0_oneplus_11` 的 `46a66233` 签出）。两个提交：

| 提交       | 内容                                                            |
| ---------- | --------------------------------------------------------------- |
| `4d11ef49` | `oplus-chg-22811.dtsi` 打开第三方 PPS，补 11 V / 5 A 的策略属性 |
| `2a79fb5a` | 5 个驱动文件，让 v1 PPS 引擎在无电荷泵的 22811 上工作           |

**构建、打包、刷写的说明不在这个仓库**，都在主仓库根目录的 [SUPPORT.md](https://github.com/Aibeto/android_kernel_oneplus_sm8550/blob/feat/16.0/oneplus_11/pps/SUPPORT.md)（本地是 `../../SUPPORT.md`）

编译和构建的脚本也在主仓库
