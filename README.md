# 通用机场签到😍<br/>
>只要机场网站 "Powered by SSPANEL"，就可以进行签到。要确认是否是 "Powered by SSPANEL"，在机场首页滑到最底端就可以看到。<br/>例如：
![Y0}SY$J`8837H8T5GXM1DZY](https://user-images.githubusercontent.com/21276183/214764546-4f66333a-cb9b-420e-8260-697d26fb4547.png)
## 作用
>每天进行签到，获取额外的流量奖励。
## 推送方式
>🚀🚀该脚本采用的是 <a href = 'https://sct.ftqq.com/r/5126'>Server酱</a> 的推送方式，如果不需要推送，就下面的 SCKEY 参数的值设置为 <b>空</b> 就行。
# 部署过程
1. 右上角`Fork`此仓库。
2. 然后到`Settings`→`Secrets and variables`→`Actions`新建以下`Secrets`：

    | 参数 | 是否必须 | 内容 |
    | ---- | -------- | ---- |
    | URL | 是 | 机场网址 |
    | CONFIG | 是 | 用户和密码 |
    | SCKEY | 否 | Server酱秘钥 |

    <b>URL 的值必须是机场网站的地址</b>，例如：<https://example.com>，尾部不要加 /。<br/>CONFIG 写法：一行用户一行密码。
    
    若想签到不同的机场，须创建不同的 URL 和 CONFIG:

    <img width="960" height="474" alt="image" src="https://github.com/user-attachments/assets/bbb3c1ce-16bc-4197-b66a-8cc4c4f5bc9e" />

4. 到`Actions`中为每个机场创建一个 workflow，根据创建的`Secrets`填写 Run sign 中 env 部分变量的值，以后每天项目都会自动运行。

    <img width="330" height="120" alt="image" src="https://github.com/user-attachments/assets/063f1ce5-a941-4b56-925f-84acca4ee651" />

5. 最后，可以到`Run sign`查看签到情况，同时也会也会将签到详情推送到 Server酱。
