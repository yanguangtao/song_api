关注
==============================

关注 or 取消
-------------------
follow  post

参数::

    {
        "follow_id" : 123
        "action": 1   1关注, 0取消关注
    }

返回::

    {
    "msg": "",
    "data": {
    },
    "code": 0
    }

获取关注或被关注列表

follow   get 需要登录

参数::

    {
    "type": 0 我关注的人  ，1关注我的人
    }

返回::

    {
    "code": 0,
    "data": {
        "list": [
            {
                "id": 3,
                "avatarUrl": "32312321323",
                "city": "",
                "country": "",
                "gender": 0,
                "language": "",
                "nickName": "test",
                "province": "",
                "identification": 0,
                "status": "OK",
                "create_time": "2017-12-12 00:04:55",
                "update_time": "2017-12-12 00:05:25",
                "voice_url": "abc",
                "img_url": "[]",
                "price": "0.00",
                "auth_status": 1,
                "voice_type": "豪爽直男",
                "time_start": null,
                "time_end": null,
                "service_type": "sleep",
                "user_id": "2",
                "follow_id": 3,
                "age": 0
            }
        ],
        "total": 1
    },
    "msg": ""
    }

