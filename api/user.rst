用户中心
==============================
说明::
    参数和返回都带header参数

登录
-------------------
login

参数::
        {
        "header": "login",
        "data":{
            "id_type":"wx",
            "openId":"123",
            "unionId":"",
            "nickName":"test",
            "phone" = "",
            "avatarUrl" = "",
            # 备注名可以修改的
            "name" = ""
            # 性别 0：未知、1：男、2：女
            "gender":0,
            "country": "",
            "province": "",
            "city"：""
            }
        }

返回::
    {
    "header": "user.login",
    "data": ""
    }

