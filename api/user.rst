用户中心
==============================

登录
-------------------
login

返回::

    {
    "code": 0,
    "data": {
        "id": "2",
        "avatarUrl": "https://wx.qlogo.cn/mmopen/vi_32/Q0j4TwGTfTLCTv2BrmBjvZ4xCnaWPEHN7kpKoaibH2jTb7I5BTK0icf6dAlbf8iaQO8hyyh90WSV8mibfIfmGqXyTw/0",
        "city": "Shenzhen",
        "country": "China",
        "gender": "1",
        "language": "zh_CN",
        "nickName": "爱搞事的boy",
        "openId": "obeUX0Rxu-oHk46zMJya6mrcBKlI",
        "province": "Guangdong",
        "wechat": "",
        "phone": "",
        "identification": "0",
        "status": "OK",
        "create_time": "2017-12-07 21:05:43",
        "update_time": "2017-12-11 23:14:32",
        "voice_url": "",
        "img_url": "[]",
        "price": "1.00",
        "tag": "魅力妖娆",
        "follow": 1,
        "followed": 0,
        "star": 4.9,
        "order_num": 1000
    },
    "msg": ""
}



用户列表
------------------

user   get

返回::

    {
    "code": 0,
    "data": {
        "list": [
            {
                "id": "8",
                "avatarUrl": "",
                "city": "Shenzhen",
                "country": "",
                "gender": "0",
                "language": "",
                "nickName": "果果佳",
                "openId": "12345",
                "province": "Guangdong",
                "wechat": "",
                "phone": "",
                "identification": "0",
                "status": "OK",
                "create_time": "",
                "update_time": "2017-12-13 23:24:09",
                "voice_url": "",
                "img_url": "[]",
                "price": "0.00",
                "tag": "魅力妖娆",
                "follow": 0,
                "followed": 0,
                "star": 4.9,
                "order_num": 1000
            },
            {
                "id": "7",
                "avatarUrl": "",
                "city": "Shenzhen",
                "country": "",
                "gender": "0",
                "language": "",
                "nickName": "樱桃喵",
                "openId": "1234",
                "province": "Guangdong",
                "wechat": "",
                "phone": "",
                "identification": "0",
                "status": "OK",
                "create_time": "",
                "update_time": "2017-12-13 23:23:43",
                "voice_url": "",
                "img_url": "[]",
                "price": "0.00",
                "tag": "魅力妖娆",
                "follow": 0,
                "followed": 0,
                "star": 4.9,
                "order_num": 1000
            }
            ]
            }

获取自己的详细资料   
------------------------

user        get  需要登录

返回参数::

    {
    "code": 0,
    "data": {
        "id": "2",
        "avatarUrl": "https://wx.qlogo.cn/mmopen/vi_32/Q0j4TwGTfTLCTv2BrmBjvZ4xCnaWPEHN7kpKoaibH2jTb7I5BTK0icf6dAlbf8iaQO8hyyh90WSV8mibfIfmGqXyTw/0",
        "city": "Shenzhen",
        "country": "China",
        "gender": "1",
        "language": "zh_CN",
        "nickName": "爱搞事的boy",
        "openId": "obeUX0Rxu-oHk46zMJya6mrcBKlI",
        "province": "Guangdong",
        "wechat": "",
        "phone": "",
        "identification": "0",
        "status": "OK",
        "create_time": "2017-12-07 21:05:43",
        "update_time": "2017-12-11 23:14:32",
        "voice_url": "",
        "img_url": "[]",
        "price": "1.00",
        "tag": "魅力妖娆",
        "follow": 1,
        "followed": 0,
        "star": 4.9,
        "order_num": 1000,
        "is_follow":true,
        "auth_status": 0   0未认证 1认证中 2已认证
        "voice_type": "清纯可爱",
        "time_start": 20, 服务开始时间
        "time_end": "24"  服务结束时间
    },
    "msg": ""
    }


修改资料

user        post   需要登录

参数::
    
    都是可选参数
    {
    "nickName": "爱搞事的boy",
    "img_url": "头像",
    "wechat": "123",
    "phone": "13760221010",
    "city": "城市",
    "time_start": 16,  服务开始时间
    "time_end": 20
    }

返回::

    {
    "code": 0,
    "msg":""
    }


用户认证
---------------------------
user/auth   post    需要登录

参数::

    {
    "voice_url":"http://" 必填,
    "voice_type": "清纯可爱"   必填
    }

返回::

    {
    "code": 0,
    "msg":""
    }  

查看声音类型
-------------------

user/voice_type   get

参数:: 

    {
        "gender":0   女生  1男生
    }

返回::
    
    {
    "code": 0,
    "data": [
        {
            "id": 1,
            "voice_type": "娇萌萝莉",
            "status": "OK",
            "update_time": "2017-12-16 17:01:34",
            "gender": 0
        },
        {
            "id": 2,
            "voice_type": "知性丽人",
            "status": "OK",
            "update_time": "2017-12-16 17:02:07",
            "gender": 0
        },
        {
            "id": 3,
            "voice_type": "热情辣妹",
            "status": "OK",
            "update_time": "2017-12-16 17:02:52",
            "gender": 0
        }
    ],
    "msg": ""
}

查看用户资料
------------
user/@id   get

返回::

    {
    "code": 0,
    "data": {
        "id": "2",
        "avatarUrl": "https://wx.qlogo.cn/mmopen/vi_32/Q0j4TwGTfTLCTv2BrmBjvZ4xCnaWPEHN7kpKoaibH2jTb7I5BTK0icf6dAlbf8iaQO8hyyh90WSV8mibfIfmGqXyTw/0",
        "city": "Shenzhen",
        "country": "China",
        "gender": "1",
        "language": "zh_CN",
        "nickName": "爱搞事的boy",
        "openId": "obeUX0Rxu-oHk46zMJya6mrcBKlI",
        "province": "Guangdong",
        "wechat": "",
        "phone": "",
        "identification": "0",
        "status": "OK",
        "create_time": "2017-12-07 21:05:43",
        "update_time": "2017-12-11 23:14:32",
        "voice_url": "",
        "img_url": "[]",
        "price": "1.00",
        "tag": "魅力妖娆",
        "follow": 1,
        "followed": 0,
        "star": 4.9,
        "order_num": 1000,
        "is_follow":true,
        "auth_status": 0   0未认证 1认证中 2已认证
        "voice_type": "清纯可爱"
    },
    "msg": ""
    }

