# 获取1688商品详情

uri：/api/product/item/1688?goods_id=809860480507

Method：GET

## Header

| 名称          | 类型   | 是否必须 | 描述  | 示例值         |
| :------------ | :----- | :------- | :---- | -------------- |
| Authorization | String | 是       | Token | Bearer {token} |



**参数**

| 名称     | 类型 | 是否必须 | 描述   | 示例值       |
| :------- | :--- | :------- | :----- | ------------ |
| goods_id | Long | 是       | 商品id | 895894241423 |



**返回结果**

| 名称   | 类型                                                | 描述 | 示例值 |
| :----- | :-------------------------------------------------- | :--- | :----- |
| result | product.search.queryProductDetail.resut.ResultModel | -    | -      |
| success | boolean | 是否成功                                                   | true   |
| code | java.lang.String                                           | 返回码   |        |
| message | java.lang.String                                           | 提示     |        |
| result  | product.search.queryProductDetail.model.ProductDetailModel | 结果     |        |





## result

| 名称                | 类型                                                        | 描述                                                         | 示例值                                                       |
| :------------------ | :---------------------------------------------------------- | :----------------------------------------------------------- | ------------------------------------------------------------ |
| offerId             | java.lang.Long                                              | 商品id                                                       | 34513534353434                                               |
| categoryId          | java.lang.Long                                              | 类目id                                                       | 32                                                           |
| categoryName        | java.lang.String                                            | 类目名称                                                     | 裙子                                                         |
| subject             | java.lang.String                                            | 中文标题                                                     | 猫砂盆超大号防外溅猫厕所加高巨无霸开放式宠物用品厂家直销批发 |
| subjectTrans        | java.lang.String                                            | 译文标题                                                     | Cat litter box extra large splash-proof cat toilet heightened giant open pet supplies factory direct sales wholesale |
| description         | java.lang.String                                            | 详情描述                                                     | 1                                                            |
| mainVideo           | java.lang.String                                            | 主视频                                                       | 1                                                            |
| detailVideo         | java.lang.String                                            | 详情视频                                                     | 1                                                            |
| productImage        | product.search.queryProductDetail.model.ProductImage        | 图片模型                                                     | 1                                                            |
| productAttribute    | product.search.queryProductDetail.model.ProductAttribute[]  | 商品CPV属性                                                  | 1                                                            |
| productSkuInfos     | product.search.queryProductDetail.model.SkuInfo[]           | 商品SKU                                                      | 1                                                            |
| productSaleInfo     | product.search.queryProductDetail.model.ProductSaleInfo     | 商品销售信息                                                 | 1                                                            |
| productShippingInfo | product.search.queryProductDetail.model.ProductShippingInfo | 商品包裹配送相关数据                                         | 1                                                            |
| isJxhy              | boolean                                                     | 是否精选货源                                                 | true                                                         |
| sellerOpenId        | java.lang.String                                            | 商家加密ID                                                   | 23tsdvcdsjngp3oj4j3i5                                        |
| minOrderQuantity    | java.lang.Integer                                           | 最小起批量模型                                               | 1                                                            |
| batchNumber         | Integer                                                     | 一手数量                                                     | 200                                                          |
| status              | String                                                      | 商品状态。published:上网状态;member expired:会员撤销;auto expired:自然过期;expired:过期(包含手动过期与自动过期);member deleted:会员删除;modified:修改;new:新发;deleted:删除;TBD:to be delete;approved:审批通过;auditing:审核中;untread:审核不通过; | published                                                    |
| tagInfoList         | com.alibaba.cbu.offer.model.out.ProductTagInfo[]            | 商品服务标签                                                 | 1                                                            |
| traceInfo           | String                                                      | 打点信息，用于向1688上报打点数据                             | object_id@620201390233^object_type@offer                     |
| sellerMixSetting    | product.search.queryProductDetail.model.SellerMixSetting    | 卖家混批配置                                                 | 1                                                            |
| productCargoNumber  | String                                                      | 商品货号                                                     | 1                                                            |
| sellerDataInfo      | product.search.queryProductDetail.model.SellerDataInfo      | 商家属性数据                                                 | {}                                                           |
| soldOut             | String                                                      | 商品销量                                                     | 12342                                                        |
| channelPrice        | product.search.queryProductDetail.model.ChannelPrice        | 渠道价格数据                                                 | 如下                                                         |
| promotionModel      | com.alibaba.cbu.offer.model.PromotionModel                  | 营销                                                         | 营销                                                         |
| tradeScore          | String                                                      | 货品评分                                                     | 5.0                                                          |
| topCategoryId       | Long                                                        | 一级类目                                                     | 1                                                            |
| secondCategoryId    | Long                                                        | 二级类目                                                     | 2                                                            |
| thirdCategoryId     | Long                                                        | 三级类目                                                     | 3                                                            |
| sellingPoint        | String[]                                                    | 多语言卖点                                                   | 卖点:卖点描述                                                |
| offerIdentities     | String[]                                                    | 商家身份                                                     | 超级工厂,实力商家，诚信通                                    |
| createDate          | String                                                      | 创建时间                                                     | 2024-05-24 00:00:00                                          |
| isSelect            | String                                                      | 跨境select货盘                                               | true                                                         |
| certificateList     | com.alibaba.cbu.offer.model.OfferCertificateModel[]         | 商品证书列表                                                 | [ { "certificateCode": "ZL 2018 3 0658542.7", "certificatePhotoList": [ "https://cbu01.alicdn.com/img/ibank/test" ] "certificateName": "外观专利证书或授权书证书", }] |
| promotionUrl        | String                                                      | 具有【AI跨境运营助手】模块的1688商品详情页链接               | 商品详情页链接                                               |



### productImage

| 名称       | 类型               | 描述   | 示例值                                                       |
| :--------- | :----------------- | :----- | ------------------------------------------------------------ |
| images     | java.lang.String[] | 图片   | 图片                                                         |
| whiteImage | String             | 白底图 | https://cbu01.alicdn.com/img/ibank/O1CN01pEsVS41Bs2uny9oka_!!0-0-cib.jpg |

### productAttribute

| 名称               | 类型             | 描述         | 示例值 |
| :----------------- | :--------------- | :----------- | ------ |
| attributeId        | java.lang.String | 属性id       | 1      |
| attributeName      | java.lang.String | 属性名称     | 1      |
| value              | java.lang.String | 属性值       | 1      |
| attributeNameTrans | java.lang.String | 属性名称翻译 | 1      |
| valueTrans         | java.lang.String | 属性值翻译   | 1      |

### productSkuInfos

| 名称             | 类型                                                   | 描述     | 示例值       |
| :--------------- | :----------------------------------------------------- | :------- | ------------ |
| amountOnSale     | Integer                                                | 库存     | 库存         |
| price            | java.lang.String                                       | 价格     | 价格         |
| jxhyPrice        | java.lang.String                                       | 废弃     | 精选货源价格 |
| skuId            | Long                                                   | sku      | sku          |
| specId           | java.lang.String                                       | specid   | specid       |
| skuAttributes    | product.search.queryProductDetail.model.SkuAttribute[] | 属性     | 属性         |
| pfJxhyPrice      | String                                                 | 废弃     | 1            |
| consignPrice     | String                                                 | 废弃     | 1            |
| cargoNumber      | String                                                 | sku级别  | 1            |
| promotionPrice   | String                                                 | 营销价   | 1            |
| fenxiaoPriceInfo | com.alibaba.cbu.offer.model.FenxiaoPriceInfo           | 分销价格 | 1            |

#### skuAttributes

| 名称               | 类型             | 描述       | 示例值 |
| :----------------- | :--------------- | :--------- | ------ |
| attributeId        | java.lang.Long   | 属性id     | 1      |
| attributeName      | java.lang.String | 属性名     | 1      |
| attributeNameTrans | java.lang.String | 属性名翻译 | 1      |
| value              | java.lang.String | 值         | 1      |
| valueTrans         | java.lang.String | 值翻译     | 1      |
| skuImageUrl        | java.lang.String | sku图片    | 1      |