订单
==================

参数说明::

	 {
        "id": 3,
        "order_sn": "123",
        "service_id": 1, 服务者id
        "consignee_id": 1,  下单人id
        "order_amount": "0.00",   订单总金额
        "bonus": "0.00",  红包抵扣金额
        "pay_fee": "0.00",   支付金额 order_amount = bonus + pay_fee
        "pay_name": "wx",
        "order_status": 0, 订单状态。0，未确认；1，已确认；2，已取消；
        "pay_status": 0,  支付状态；0，未付款；1，付款中；2，已付款
        "service_status": 0,   服务情况，0，未开始；1，已开始；2，已结束
        "create_time": "", 订单确认时间
        "confirm_time": "",
        "start_time": "", 开始服务时间
        "bonus_id": 0,  红包id
        "product_price": "1.00",  即user中的price
        "product_total": 1  
       }

订单列表
--------------------

order  get

返回::

   {
    "code": 0,
    "data": [
        {
            "id": 3,
            "order_sn": "123",
            "service_id": 1,
            "consignee_id": 1,
            "order_amount": "0.00",
            "bonus": "0.00",
            "pay_fee": "0.00",
            "pay_name": "wx",
            "order_status": 0,
            "pay_status": 0,
            "service_status": 0,
            "create_time": "",
            "confirm_time": "",
            "start_time": "",
            "bonus_id": 0,
            "product_price": "1.00",
            "product_total": 1
    ],
    "msg": ""
	}

订单详情
---------------------

order/@order_sn    get

返回::

	{
    "code": 0,
    "data": {
        "id": 3,
        "order_sn": "123",
        "service_id": 1, 服务者id
        "consignee_id": 1,  下单人id
        "order_amount": "0.00",   订单总金额
        "bonus": "0.00",  红包抵扣金额
        "pay_fee": "0.00",   支付金额 order_amount = bonus + pay_fee
        "pay_name": "wx",
        "order_status": 0, 订单状态。0，未确认；1，已确认；2，已取消；
        "pay_status": 0,  支付状态；0，未付款；1，付款中；2，已付款
        "service_status": 0,   服务情况，0，未开始；1，已开始；2，已结束
        "create_time": "", 订单确认时间
        "confirm_time": "",
        "start_time": "", 开始服务时间
        "bonus_id": 0,  红包id
        "product_price": "1.00",  即user中的price
        "product_total": 1  
    },
    "msg": ""
	}

下订单
-----------------

order   post

参数::

	{
	"service_id":123,
	"order_amount": 2.00,
	"bonus": "0.00",
	"pay_fee":"2.00",
	"bonus_id":0 前期先不传,
	"product_price": 1.00,
	"product_total":2,
	"pay_name":"wx"
	}


返回::

    {
    "code": 0,
    "data": {
        "product_price": "1",
        "product_total": "2",
        "consignee_id": 2,
        "service_id": "2",
        "order_sn": "2017121400213394",
        "order_amount": "2",
        "create_time": "2017-12-14 00:21:33",
        "id": "9"
    },
    "msg": ""
	}


