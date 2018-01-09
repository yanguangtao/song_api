websocket聊天
=========================

websocket连接
------------------

wss://game.erduu.com/ws/

返回::
	onconnect 连接时返回client_id
	

绑定client   
-------------

chat/bind   post

参数::

	{
	    "client_id": 'fesfsef'
	}

返回::
	
    {
    "msg": "绑定成功",
    "data": {
    },
    "code": 0
    }


和某人聊天
------------------
chat/chat  post
参数::

	{
	"to_id": 123,
	"msg": "test",
	"msg_type":"text"   voice
	}

返回::

	{
    "msg": "",
    "data": {
    },
    "code": 0
    }

    websocket

   {
   "url": "chat",
   "data":{
	"to_id": 123,
	"from_id": 12,
	"msg": "test",
	"msg_type":"text" 
	}

聊天记录
--------------------

chat/history  get

参数::

	user_id:123

返回::

	{
    "code": 0,
    "data": {
        "list": [
            {
                "id": 1,
                "from_id": "2",
                "to_id": "123",
                "msg_type": "text",
                "from_status": "OK",
                "msg": "test",
                "to_status": "OK",
                "create_time": "2018-01-09 23:25:04",
                "update_time": "2018-01-09 23:25:04"
            }
        ],
        "total": 1
    },
    "msg": ""
	}



