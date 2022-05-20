# 定时自动脚本（Github-Actions版）

**注意**：本master分支版本代码使用Github-Actions定时运行，无需部署在服务器。如需在服务器中运行，请使用service分支中的代码。


4. 查看运行情况

    打开Actions页面，此时在workflows中应该出现了正在运行的工作流。当提交文件时会马上进行一次打卡，以后将会默认在每天的7:55进行打卡

    如果打卡失败请重新运行workflows并检查账号密码设置是否正确
    
    ![20200817192416](https://i.loli.net/2020/12/06/P31tu5einhLpArk.png)

## <span id="dksj">修改打卡时间</span>

打开项目中的/.github/workflows/python-package.yml文件，修改corn中的值，注意使用UTC零区时间。

例如，当前默认打卡时间是北京时间(UTC+8)每天7:05，换算成UTC零区时间为23:05。

更多关于时间的具体书写格式请参考[POSIX cron 语法](https://crontab.guru/)和[官方文档](https://docs.github.com/cn/actions/reference/events-that-trigger-workflows#)。

![20200817194102](https://i.loli.net/2020/12/06/zqXQvYCJwfrN3Pc.png)

![20200817194250](https://i.loli.net/2020/12/06/oRjts1Yy5NV9TI8.png)

---
参考开源仓库：

1. [zsu](https://github.com/Tishacy/ZJU-nCov-Hitcarder)
2. [buct](https://github.com/W0n9/BUCT_nCoV_Report)

鸣谢：

[@sumowi](https://github.com/sumowi)

[@hidragonma](https://github.com/hidragonma)

[@adamqqq](https://github.com/adamqqqplay)
