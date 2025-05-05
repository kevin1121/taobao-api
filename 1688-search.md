# 1688商品搜索

**参数**

| 名称    | 类型   | 是否必须 | 描述       | 示例值 |
| :------ | :----- | :------- | :--------- | ------ |
| keyword | String | 是       | 商品关键词 | 衣服   |
| page    | Int    | 否       | 页码       | 1      |
| size    | Int    | 否       | 页大小     | 20     |



## result

| 名称    | 类型                                         | 描述     | 示例值   |
| :------ | :------------------------------------------- | :------- | -------- |
| success | Boolean                                      | 正否正常 | 正否正常 |
| code    | String                                       | 状态码   | 状态码   |
| message | String                                       | 提示     | 提示     |
| result  | product.search.keywordQuery.model.PageInfoV3 | 内容     | 内容     |

### result

| 名称         | 类型                                                   | 描述   | 示例值 |
| :----------- | :----------------------------------------------------- | :----- | ------ |
| totalRecords | Integer                                                | 总条数 | 分页   |
| totalPage    | Integer                                                | 总页码 | 分页   |
| pageSize     | Integer                                                | 分页   | 分页   |
| currentPage  | Integer                                                | 分页   | 分页   |
| data         | product.search.keywordQuery.model.ProductInfoModelV2[] | 数据   | 数据   |

#### data

| 名称                      | 类型                                                        | 描述                                           | 示例值                                                       |
| :------------------------ | :---------------------------------------------------------- | :--------------------------------------------- | ------------------------------------------------------------ |
| imageUrl                  | String                                                      | 图片地址                                       | 图片地址                                                     |
| subject                   | String                                                      | 中文标题                                       | 中文标题                                                     |
| subjectTrans              | String                                                      | 外文标题                                       | 外文标题                                                     |
| offerId                   | Long                                                        | 商品id                                         | 2                                                            |
| isJxhy                    | Boolean                                                     | 是否精选货源                                   | true                                                         |
| priceInfo                 | product.search.keywordQuery.model.PriceInfoV2               | 价格                                           | 1                                                            |
| repurchaseRate            | String                                                      | 复购率                                         | 10%                                                          |
| monthSold                 | Integer                                                     | 30天销量                                       | 1213                                                         |
| traceInfo                 | String                                                      | 向1688上报打点数据                             | object_id@620201390233^object_type@offer                     |
| isOnePsale                | Boolean                                                     | 是否一件代发                                   | true                                                         |
| sellerIdentities          | String[]                                                    | 商家身份                                       | super_factory-超级工厂 powerful_merchants-实力商家 tp_member-诚信通会员 |
| offerIdentities           | String[]                                                    | 商品标                                         | yx-严选，select-跨境select                                   |
| tradeScore                | String                                                      | 商品交易评分                                   | 5.0                                                          |
| whiteImage                | String                                                      | 商品白底图                                     | 商品白底图                                                   |
| promotionModel            | product.search.keywordQuery.model.PromotionModelV2          | 是否有营销信息                                 | 目前只透plus                                                 |
| topCategoryId             | Long                                                        | 一级类目                                       | 1                                                            |
| secondCategoryId          | Long                                                        | 二级类目                                       | 2                                                            |
| thirdCategoryId           | Long                                                        | 三级类目                                       | 3                                                            |
| isPatentProduct           | Boolean                                                     | 是否专利商品                                   | true                                                         |
| createDate                | String                                                      | 商品上架时间                                   | 2024-04-20 08:00:00                                          |
| modifyDate                | String                                                      | 商品修改时间                                   | 2024-04-20 08:00:00                                          |
| isSelect                  | Boolean                                                     | 跨境select货盘                                 | true                                                         |
| minOrderQuantity          | Integer                                                     | 最小起批量                                     | 1                                                            |
| sellerDataInfo            | product.search.keywordQuery.model.SellerDataInfoV1          | 商品数据                                       | 1                                                            |
| productSimpleShippingInfo | product.search.keywordQuery.model.ProductSimpleShippingInfo | 简略发货信息                                   | 1                                                            |
| token                     | String                                                      | 插件返佣token                                  | abc                                                          |
| promotionURL              | String                                                      | 具有【AI跨境运营助手】模块的1688商品详情页链接 | 商品详情页链接                                               |
