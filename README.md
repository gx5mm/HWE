# 😁😁😁😁😁😁😁😁😁😁😁
##  Forked/Changed from biozzl:Woiden_Extend

HE: `https://github.com/ThekingMX1998/HWE/tree/Hax`

WE: `https://github.com/ThekingMX1998/HWE/tree/Woiden`

-----------------------------------------------------------

## Hax/Woiden Extend with Github Action


原脚本有些小问题，在此做如下更新修复：
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
1. 跳过cloudflare ddos check（selenium.webdriver更换成undetected_chromedriver）
2. 隐私模式启动（防止cf验证不显示，被识别成机器人）
3. 修改点击 Extend VPS不跳转的bug（替换成driver.get(url)的方式）
4. 替换WebDriverWait()为driver.find_element(),不然总抛异常TimeoutException
5. 系统换成windows-2022，指定python脚本version为3.9.5
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

### 感谢原作者！！

#### 计划
- Helium 版本研究中

#### Secret 增加以下变量
- ```USERNAME```
- ```PASSWORD```
- ```USERNAME_WOIDEN```
- ```PASSWORD_WOIDEN```
- ```BARKKEY```

#### ```随缘 Extend，Possibly blocked by google```，
- 原因： 
```因为github的Actions虚机托管在Azure上， 每次重新执行Actions的run workflow都会导致切换公网IP，有的IP被别人使用过（干啥就不知道了嘿嘿！），所以识别成了机器人，报出这个错。```
- 解决方法：
```多次重新执行run workflow，切换到好IP可以正常运行为止。```
<img src=./result.jpeg width=50% />

#### 参考
- https://www.python.org/
- https://www.selenium.dev/
- https://www.youtube.com/watch?v=As-_hfZUyIs
- https://github.com/actions/virtual-environments/blob/main/images/macos/macos-12-Readme.md
