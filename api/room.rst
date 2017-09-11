房间
==============================
说明::
    参数和返回都带header参数

创建房间
-------------------
create_room

参数::

    {
    "header": "create_room",
    "data": {
        "game_type": "offline",   #online 线上 ，offline线下
        "battle_type": "freestyle" # freestyle自由模式，1v1， 2v2
    }
    }

返回::

    {
    "msg": "",
    "header": "room.create",
    "data": {
        "status": "waiting",
        "blue": [
            "1"
        ],
        "room_id": "1-E5ylPGI4hgQu5NPxCNmcf31BywX1fUdb87JNKdb3vU4OevK8VBnrVAEgzmh1d",
        "users": [],
        "battle_type": "freestyle",
        "game_type": "offline",
        "room_manege": 0,
        "red": [],
        "w_id": "64050008"
    },
    "ret": 0
    }