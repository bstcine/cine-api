* 功能: 课程详情

* URL: /api/content/course/detail

* request
```
{
    "token":"", //nFmqtqzH
    "sitecode": "cine.ios.iphone",
    "channel": "i5", 
    "locale": "zh_CN",
    "appver": "1.1.3",
    "data":{
      "cid":42
    }
}
```

* response
```
{
    "code": "1",
    "code_desc": "success",
    "except_case": "",
    "except_case_desc": "",
    "result": {
        "lessoncategorys": [
            {
                "id": "d011495787003995KQ847j7eGV",
                "name": "热推新品",
                "status": "1",
                "remark": null,
                "seq": -2,
                "create_at": "2017-05-26 16:23:23",
                "create_by": "A011454493804858vCnC6NpgJi",
                "update_at": "2017-09-06 09:51:37",
                "update_by": "1",
                "delete_at": null,
                "delete_by": null,
                "is_show_pc": "1",
                "is_show_ios": "1",
                "is_show_android": "1",
                "data": "'d0114895451784428WtHSkSvpN','A011473750883473MfD6eUge7h','41'",
                "icon": "hot",
                "tag": null,
                "type": "2",
                "children": [
                    {
                        "id": "d0114895451784428WtHSkSvpN",
                        "name": "《The Cat in The Hat》原版讲读",
                        "price": "28",
                        "img": "2017/03/17/15473133SHy4zRs.jpg",
                        "total_join": 1052,
                        "lessoncategory_id": "d011489544670568frqxJBxBjh",
                        "status": "1",
                        "pay_status": 0
                    },
                    ...
                ]
            },
            ...
        ],
        "lunboImages": [
            {
                "lesson_id": "A011481685662619HkztzzwvxT",
                "name": "《小王子》上册精读课程",
                "img": "http://app.bstcine.com/web/img/picture1.png",
                "type": "1"
            },
            ...
        ]
    }
}
```
* 说明：token为空和正确的token返回值中is_paid、can_learn的值不同 
* 错误token response
```
{
    "code": "1",
    "code_desc": "success",
    "except_case": "",
    "except_case_desc": "no_login"
}
```
