# tdwnorm - 高精度正态分布 CDF
我用一个独创的、无分段的单一函数，在任意点达到了双精度极限。我的结果与工业标准 Excel 完全一致，而 SciPy 却出现了偏差。而且，我的速度比 SciPy 快 270 倍,更比excel快。
比如：Excel 的NORMSDIST在 x=-15 时返回 3.67096619931275E-51，我这个库返回的也是 **3.67096619931275e-51**。
Excel 的在 x=0.1时返回0.539827837277029,我这个库返回的也是0.539827837277029。  
## 安装
pip install https://github.com/tdwabel/tdwnorm/releases/download/v1.0.0/tdwnorm-1.0.0-py3-none-any.whl
## 使用
import tdwnorm

print(tdwnorm.cdf(-37))  # 输出 5.725571222524576e-300  (excel的结果:5.72557122252458E-300,一致)

## 赞助支持

本库永久免费，如果对你有帮助，欢迎微信扫码赞助。  

<img width="828" height="1124" alt="收款码" src="https://github.com/user-attachments/assets/1f5a5e3d-8699-4b09-9ed7-186e415bc34a" />

## 源码授权

如需源码集成或企业级技术支持，请联系：13025178270@163.com 手机号：13025178270
