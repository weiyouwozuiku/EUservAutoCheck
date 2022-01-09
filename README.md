# EUservAutoCheck

由于euser的“防御机制”，本脚本目前已失效，推荐另一个项目[eu_ex](https://github.com/a-beam-of-light/eu_ex)


## 描述
本地运行的自动续期EUserv免费IPv6 VPS脚本
本项目基于[EUserv_extend](https://github.com/CokeMine/EUserv_extend)项目，在此基础上采用本地运行脚本的方式并将每次的信息保存到python脚本所在目录下的`EUserLog.txt`，便于查看脚本执行情况。

## 使用说明
1. 安装python3
2. 安装相关依赖`pip3 install beautifulsoup4 requests`
3. 执行项目中的`EUservAutoCheck.py`程序即可(需要先修改该python文件中的帐号信息,以及代理信息)

## 自动化
安装crontab,使用`crontab -e`添加定时任务。`0 7 * * * python3 <项目中python脚本所在绝对路径> `,即每天7.am执行脚本。
