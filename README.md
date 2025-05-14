# QQ音乐无损解析使用方法
先安装 文件所需要的依赖模块 
pip install -r requirements.txt
再运行app.py文件即可

# 环境要求
Python >= 3

# 请求示例

如图箭头显示

![url链接](https://raw.githubusercontent.com/mkr-0920/tencent_url/refs/heads/main/example.png)

## 参数列表

请求链接选择 http://ip:port/song 

请求方式 GET

|  参数列表  | 参数说明 |
|  ----  | ---- |
| url | 解析获取到的QQ音乐地址|

# 返回数据
song[] = 包含歌名 专辑 歌手 图片
lyric[] = 包含原文歌词 翻译歌词(如果有)
music_urls[] = 包含'm4a', '128', '320', 'flac', 'ape'等歌曲链接
其中flac和ape为无损 320为高品质 m4a和128为标准音质

# 注意事项
请先在app.py中的cookie_str填写入你从y.qq.com获取到的cookie才可以解析！
其中 要解析VIP歌曲以及无损以上音质 请获取会员账号的cookie
