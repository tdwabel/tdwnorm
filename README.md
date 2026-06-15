# tdwnorm - 高精度正态分布 CDF

Excel 的 `NORM.S.DIST` 在 x=-15 时返回 0，而这个库返回真实的 **3.67096619931275e-51**。  
任意点的精度达到双精度极限（1e-16），并比 SciPy 快 270 倍。

## 安装

pip install https://github.com/tdwabel/tdwnorm/releases/download/v1.0.0/tdwnorm-1.0.0-cp314-none-win_amd64.whl

## 使用

from tdwnorm import cdf
print(cdf(-15))  # 输出 3.67096619931275e-51

## 对比 Excel

| x 值 | Excel `NORM.S.DIST` | **tdwnorm** |
|------|--------------------|--------------|
| -15  | 0（完全失效）      | 3.670966e-51 ✅ |
| -37  | 0（错误）          | 5.725571e-300✅ |

## 赞助支持

本库永久免费，如果对你有帮助，欢迎微信扫码赞助。  


<img width="828" height="1124" alt="收款码" src="https://github.com/user-attachments/assets/1f5a5e3d-8699-4b09-9ed7-186e415bc34a" />

## 源码授权

如需源码集成、定制编译或企业级技术支持，请联系：13025178270@163.com 手机号：13025178270
