# 搜索淘宝商品

uri：/api/product/search/taobao

method：GET

## Header

| 名称          | 类型   | 是否必须 | 描述  | 示例值         |
| :------------ | :----- | :------- | :---- | -------------- |
| Authorization | String | 是       | Token | Bearer {token} |

## 参数

| 名称    | 类型   | 是否必须 | 描述                   |
| :------ | :----- | :------- | :--------------------- |
| keyword | String | 是       | 搜索关键字             |
| page    | Number | 否       | 页码                   |
| size    | Number | 否       | 页大小，默认20，上限20 |



## 响应参数

| 名称                | 类型     | 描述                                                         |
| :------------------ | :------- | :----------------------------------------------------------- |
| biz_error_code      | String   | 错误码                                                       |
| biz_error_msg       | String   | 错误原因                                                     |
| data                | Object   | 搜索结果                                                     |
| data                | Object[] | -                                                            |
| item_id             | Number   | 商品Id                                                       |
| main_image_url      | String   | 商品主图                                                     |
| price               | String   | 商品优惠价（单位：元）                                       |
| inventory           | Number   | 商品库存                                                     |
| tags                | String[] | 包含的商品活动标签，例如： activity_202311_1_tb_manjian （ 第一波淘宝活动(包含满减和立减) ） activity_202311_1_tm_manjian（第一波天猫活动(包含满减和立减)） activity_202311_2_tb_manjian（第二波淘宝活动(包含满减和立减)） activity_202311_2_tm_manjian （第二波天猫活动(包含满减和立减)） |
| shop_name           | String   | 店铺名称                                                     |
| title               | String   | 商品标题                                                     |
| multi_language_info | Object   | 商品翻译信息                                                 |
| language            | String   | 商品翻译语种                                                 |
| title               | String   | 商品标题（多语言）                                           |
| coupon_price        | String   | 淘宝实时券后价。 仅供参考，因优惠变动存在与下单价格不一致风险。 |
| promotion_displays  | Object[] | 商品营销优惠列表                                             |
| type_name           | String   | 商品优惠类型名称                                             |
| promotion_info_list | Object[] | 优惠明细                                                     |
| activity_code       | String   | 活动code                                                     |
| promotion_name      | String   | 优惠名称                                                     |
| page_no             | Number   | 页码                                                         |
| page_size           | Number   | 页大小                                                       |