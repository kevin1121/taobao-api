# 获取淘宝商品详情

uri：/api/product/item/taobao?goods_id=809860480507



## 参数

| 名称     | 类型   | 是否必须 | 描述         |
| :------- | :----- | :------- | :----------- |
| goods_id | String | 是       | 809860480507 |



## 响应参数



| 名称                     | 类型     | 描述                                                         |
| :----------------------- | :------- | :----------------------------------------------------------- |
| biz_error_code           | String   | 错误码                                                       |
| biz_error_msg            | String   | 错误原因                                                     |
| data                     | Object   | 商品信息                                                     |
| shop_id                  | Number   | 店铺id                                                       |
| \|-- property_image_list | Object[] | 属性图片列表                                                 |
| properties               | String   | 属性                                                         |
| image_url                | String   | 图片                                                         |
| tags                     | String[] | 确认的商品标签 例如： activity_202311_1_tb_manjian （ 第一波淘宝活动(包含满减和立减) ） |
| \|-- multi_language_info | Object   | 多语言翻译信息                                               |
| title                    | String   | 多语言标题                                                   |
| \|-- properties          | Object[] | 多语言属性                                                   |
| prop_id                  | Number   | 属性id                                                       |
| prop_name                | String   | 多语言属性名称                                               |
| value_id                 | Number   | 属性值id                                                     |
| value_name               | String   | 多语言属性值                                                 |
| \|--  sku_properties     | Object[] | 多语言sku属性                                                |
| sku_id                   | Number   | sku id                                                       |
| \|-- properties          | Object[] | 多语言sku属性列表                                            |
| prop_id                  | Number   | 属性id                                                       |
| prop_name                | String   | 多语言属性名称                                               |
| value_id                 | Number   | 属性值id                                                     |
| value_name               | String   | 多语言属性值                                                 |
| value_desc               | String   | 多语言属性值+备注                                            |
| language                 | String   | 多语言翻译语种                                               |
| coupon_price             | Number   | 淘宝实时券后价（单位：分）。 仅供参考，因优惠变动存在与下单价格不一致风险。 |
| \|-- promotion_displays  | Object[] | 优惠明细                                                     |
| type_name                | String   | 商品优惠类型名称                                             |
| \|-- promotion_info_list | Object[] | 优惠明细                                                     |
| activity_code            | String   | 活动code                                                     |
| promotion_name           | String   | 优惠名称                                                     |
| item_resource            | String   | taobao：淘宝/天猫                                            |
| item_id                  | Number   | 商品id                                                       |
| title                    | String   | 标题                                                         |
| pic_urls                 | String[] | 商品主图                                                     |
| shop_name                | String   | 店铺名称                                                     |
| price                    | Number   | 商品原价（单位：分）                                         |
| promotion_price          | Number   | 商品优惠价（单位：分）                                       |
| description              | String   | 商品详情                                                     |
| \|-- properties          | Object[] | 商品参数信息                                                 |
| prop_id                  | Number   | 属性id                                                       |
| prop_name                | String   | 属性名称                                                     |
| value_id                 | Number   | 属性值id                                                     |
| value_name               | String   | 属性值                                                       |
| \|-- sku_list            | Object[] | sku列表(详情无sku，skuId 为 0)                               |
| sku_id                   | Number   | skuId                                                        |
| quantity                 | Number   | 库存                                                         |
| price                    | Number   | 商品原价（单位：分）                                         |
| promotion_price          | Number   | 商品优惠价（单位：分）                                       |
| pic_url                  | String   | 图片                                                         |
| \|-- properties          | Object[] | sku 属性列表                                                 |
| prop_id                  | Number   | 属性id                                                       |
| prop_name                | String   | 属性名称                                                     |
| value_id                 | Number   | 属性值id                                                     |
| value_name               | String   | 属性值                                                       |
| value_desc               | String   | 属性值+备注                                                  |
| coupon_price             | Number   | 淘宝实时券后价（单位：分）。 仅供参考，因优惠变动存在与下单价格不一致风险。 |