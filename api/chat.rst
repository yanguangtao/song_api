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


