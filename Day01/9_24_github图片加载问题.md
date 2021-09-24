# Github图片加载不出来问题

## 解决方案1：host文件修改（windows）

### 缺点：较为繁琐，要自己去查域名

### 优点：修改后，完美显示

### 复制以下DNS解析到本地host

199.232.96.133 camo.githubusercontent.com

199.232.96.133 cloud.githubusercontent.com

199.232.96.133 raw.githubusercontent.com

199.232.96.133 gist.githubusercontent.com

199.232.96.133 desktop.githubusercontent.com

199.232.96.133 user-images.githubusercontent.com

199.232.96.133 avatars0.githubusercontent.com

199.232.96.133 avatars1.githubusercontent.com

199.232.96.133 avatars2.githubusercontent.com

199.232.96.133 avatars3.githubusercontent.com

199.232.96.133 avatars4.githubusercontent.com

199.232.96.133 avatars5.githubusercontent.com

199.232.96.133 avatars6.githubusercontent.com

199.232.96.133 avatars7.githubusercontent.com

199.232.96.133 avatars8.githubusercontent.com


### host文件路径:C:\Windows\System32\drivers\etc\hosts

### 修改后，命令簿刷新本地DNS解析， 命令为： ipconfig /flushdns

## 解决方案2： DNS自选修改

### 缺点：修改后，有些图片可以显示,有些图片无法显示,强迫症忍不了

### 优点：简单

## 解决参考 https://www.cnblogs.com/stars-one/p/14300463.html
