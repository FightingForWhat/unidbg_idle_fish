# unidbg_idle_fish
探寻闲鱼x-sign/x-mini-wua加解密算法

```
本篇文章仅供学习讨论。

文章中涉及到的代码、实例，仅是个人日常学习研究的部分成果。

如有不当，请联系删除。
```


一直都对阿里系的签名搞那么复杂而腹诽不止，一直也对其签名原理深表好奇。
经常一系列的学习，学到了很多，表示可以应用到自己的应用上面，相对来说更安全了，但也多少有点用6位数的密码，保存2位数的存款的意思了。

展示下成果吧。纯粹炫耀。如侵可删。

![](QQ截图20240428152452.jpg)
请求参数部分截图

![](QQ截图20240428152624.jpg)
请求数据部分截图


下面是部分数据展示

```json
[
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "picWidth": "164.0",
                                    "zhimaOffline": "false",
                                    "item_type": "goods",
                                    "disableHierarchicalSort": "0",
                                    "searchProjectLayerInfo": "DoubleShade_21|DEFAULT_26|202305152329_3090_1",
                                    "pageSize": "10",
                                    "type": "1",
                                    "q_type": "0",
                                    "search_from_page": "xyHome",
                                    "tagname": "全新/包邮",
                                    "wantNum": "0",
                                    "id": "788636250267",
                                    "tag": "new/freeship",
                                    "keyword": "iphone",
                                    "scm": "1007.32845.290827.0",
                                    "seller_id": "GjU2ReiYTXiaeaRUzzrLCQ==",
                                    "publishTime": "1714139629000",
                                    "search_tab_from": "SEARCH_TAB_MAIN",
                                    "picHeight": "123.0",
                                    "cCatId": "126862528",
                                    "biz_type": "item",
                                    "tbCatId": "1512",
                                    "index": "0",
                                    "spm": "a2170.8011571.1.0",
                                    "catId": "50025386",
                                    "original_q": "iphone",
                                    "p_type": "2",
                                    "page": "1",
                                    "position": "0",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "tcDistance": "0.0",
                                    "abid": "290827",
                                    "singleControl": "false",
                                    "cpvNavWlTbCatId": "1512",
                                    "layerInfo": "22845#0#290827#5_22845#10269#446628#67_22845#12929#480547#54_22845#26994#481509#6_22845#12961#449492#47_22845#26899#481719#11_22845#25306#477353#13_22845#12936#453303#2_22845#12926#482457#52_22845#12928#482555#57",
                                    "item_id": "788636250267",
                                    "oldZhima": "false",
                                    "unShowLabelParams": "{}",
                                    "userIsUseFishShopCard": "false",
                                    "bucketid": "26",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": "a5507830d9f36fc69894e2684c958bc9",
                                    "idle_mount_tai_task_abs": "0:T:1;1192:T:0;768:T:0;793:T:0;130:T:0;343:T:0;467:T:0;573:T:0;1222:T:0;123:T:0;350:T:0;1209:C:0;212:T:0;505:T:0;1193:T:0;354:C:0;353:T:0;892:T:0;972:T:0;193:T:0;370:T:0;-4:C:1;340:T:0;359:T:0;363:T:0;536:T:0;169:T:0;788:T:0;487:T:0;199:T:0;223:T:0;792:T:0;598:T:0;1134:T:0;126:T:0;517:T:0;542:T:0;470:T:0;1229:C:0;356:T:0;593:T:0;-10:T:1;551:T:0;789:T:0;194:T:0;1210:C:0;592:T:0;543:T:0;225:T:0;552:T:0;500:T:0;226:T:0;366:T:0;933:T:0;337:T:0;1156:T:0;1173:T:0;558:T:0;341:T:0;1075:T:0;514:T:0;1190:T:0;244:T:0;893:T:0;969:T:0;227:T:0;1211:T:0;1142:T:0;1185:T:0;361:T:0;368:T:0;1228:C:0;766:T:0;1205:T:0;342:T:0;797:T:0;466:T:0;533:T:0",
                                    "q": "iphone",
                                    "CoinPay_Morediscount": "false",
                                    "isFromAISuggestion": "false",
                                    "tai_match_type": "0",
                                    "HideUserInfo": "false",
                                    "serviceUtParams": "[{\"arg1\":\"4_tag_r2_36\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"全新未拆封\"}},{\"arg1\":\"4_tag_r2_38\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"Apple/苹果\"}},{\"arg1\":\"4_tag_r2_34\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"512GB\"}},{\"arg1\":\"4_tag_r3_9\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"12人想要\"}},{\"arg1\":\"4_tag_r4_750\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"百分百好评\"}},{\"arg1\":\"4_tag_r1_13\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"freeShippingIcon\"}}]",
                                    "labelBucketId": "9",
                                    "zhimaLogBucketId": "9"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "河南",
                                "detailParams": {
                                    "picWidth": "1440",
                                    "itemId": "788636250267",
                                    "itemType": "detailCommonBuy",
                                    "picHeight": "1080",
                                    "userNick": "诚信第一",
                                    "soldPrice": "1306",
                                    "isVideo": "false",
                                    "title": "女生自用闲置苹果iPhone 14pro灵动岛暗紫色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！"
                                },
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "788636250267",
                                            "bizType": "item",
                                            "picHeight": "123.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "1",
                                            "keyword": "iphone",
                                            "referPage": "Page_xySearchResult_FindSimilar"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "itemPicUrl": "http://img.alicdn.com/bao/uploaded/i3/O1CN01jHshLo1oNbdtg6cmF_!!0-fleamarket.jpg",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "GjU2ReiYTXiaeaRUzzrLCQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788636250267",
                                                "targetIndex": "1",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "788636250267",
                                                    "bizType": "item",
                                                    "picHeight": "123.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "1",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "GjU2ReiYTXiaeaRUzzrLCQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788636250267",
                                                "targetIndex": "1",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "788636250267",
                                                    "bizType": "item",
                                                    "picHeight": "123.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "1",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "GjU2ReiYTXiaeaRUzzrLCQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788636250267",
                                                "targetIndex": "1",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "788636250267",
                                                    "bizType": "item",
                                                    "picHeight": "123.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "1",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "GjU2ReiYTXiaeaRUzzrLCQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788636250267",
                                                "targetIndex": "1",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "788636250267",
                                                    "bizType": "item",
                                                    "picHeight": "123.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "1",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "GjU2ReiYTXiaeaRUzzrLCQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788636250267",
                                                "targetIndex": "1",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "788636250267",
                                                    "bizType": "item",
                                                    "picHeight": "123.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "1",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01nEHAUr1bTw528ELSv_!!6000000003467-2-tps-96-96.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "GjU2ReiYTXiaeaRUzzrLCQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788636250267",
                                                "targetIndex": "1",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "788636250267",
                                                    "bizType": "item",
                                                    "picHeight": "123.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "1",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i4/O1CN01d2x4An1z5FVcHazR1_!!6000000006662-2-tps-96-96.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "GjU2ReiYTXiaeaRUzzrLCQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788636250267",
                                                "targetIndex": "1",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "788636250267",
                                                    "bizType": "item",
                                                    "picHeight": "123.0",
                                                    "picWicth": "164.0",
                                                    "name": "结果不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "1",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01XMrXCG1W2OB7JmJIY_!!6000000002730-2-tps-96-96.png",
                                            "index": "3",
                                            "text": "结果不相关"
                                        }
                                    ],
                                    "similarTargetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-photo-search/pages/home?kun=true&wh_ttid=native&opaque=false&extra=%7B%22imageInfo%22%3A%7B%22bizCode%22%3A%22graph_similarity%22%2C%22reqFromPage%22%3A%22main_search_feeds_dislike%22%2C%22source%22%3A%22itemPic%22%2C%22url%22%3A%22http%3A%2F%2Fimg.alicdn.com%2Fbao%2Fuploaded%2Fi3%2FO1CN01jHshLo1oNbdtg6cmF_%21%210-fleamarket.jpg_640x640q90.jpg%22%7D%7D",
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTagCustomParam": {
                                    "feedStyle202208": "1",
                                    "feedStyle202304": "1"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "36",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "全新未拆封"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "全新未拆封"
                                                    },
                                                    "arg1": "4_tag_r2_36"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "38",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "Apple/苹果"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "Apple/苹果"
                                                    },
                                                    "arg1": "4_tag_r2_38"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "34",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "512GB"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "512GB"
                                                    },
                                                    "arg1": "4_tag_r2_34"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "delimiterMarginRight": "4.5",
                                            "delimiterWidth": "0.5",
                                            "delimiterPosition": "between",
                                            "delimiterColor": "#D6D6D6",
                                            "delimiterHeight": "10",
                                            "hasDelimiter": "true",
                                            "delimiterMarginLeft": "4.5",
                                            "delimiterMarginBottom": "3",
                                            "mutualLabelBizGroup": "true",
                                            "delimiterMarginTop": "3"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "9",
                                                    "lineHeight": "1.3",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "12人想要",
                                                    "marginLeft": "4"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "12人想要"
                                                    },
                                                    "arg1": "4_tag_r3_9"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r4": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "bgColor": "#FFF4EB",
                                                    "color": "#FF7900",
                                                    "borderRadius": "8",
                                                    "size": "11",
                                                    "labelId": "750",
                                                    "borderPaddingLeft": "6",
                                                    "lineHeight": "1.3",
                                                    "borderPaddingRight": "6",
                                                    "type": "gradientImageText",
                                                    "content": "百分百好评",
                                                    "height": "16"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "百分百好评"
                                                    },
                                                    "arg1": "4_tag_r4_750"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r1": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "marginRight": "4",
                                                    "labelId": "13",
                                                    "width": "28",
                                                    "type": "img",
                                                    "alignment": "middle",
                                                    "content": "freeShippingIcon",
                                                    "url": "https://gw.alicdn.com/imgextra/i3/O1CN01PuymOm1I7yIlVyFV9_!!6000000000847-2-tps-84-48.png",
                                                    "height": "16"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "freeShippingIcon"
                                                    },
                                                    "arg1": "4_tag_r1_13"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "false",
                                "isAuction": "false",
                                "itemId": "788636250267",
                                "jump2XianYuHao": {
                                    "clickParam": {
                                        "arg1": "Jump2User",
                                        "args": {
                                            "bucket_id": "26",
                                            "spm": "a2170.8011571.Jump2User.1",
                                            "user_id": "9VqNOYOLgTeQTHkg/H/fnQ==",
                                            "item_id": "788636250267",
                                            "userIsUseFishShopCard": "false",
                                            "HideUserInfo": "false",
                                            "seller_id": "GjU2ReiYTXiaeaRUzzrLCQ=="
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "targetUrl": "z9xpXnwzz6eu3JHQFPK2nb4PAGLvMlrcMmttP6latEqZfAPLXlS0S2DIuSzLBfgwbrpBTDLSuq50jVIOHj1q8sWdH9r5DUfri00EPe3RM6A="
                                },
                                "picHeight": "123.0",
                                "picUrl": "http://img.alicdn.com/bao/uploaded/i3/O1CN01jHshLo1oNbdtg6cmF_!!0-fleamarket.jpg",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1306",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [],
                                "richTitle": [
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1eCD602b2gK0jSZK9XXaEgFXa-84-48.png",
                                            "width": "35.0"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "女生自用闲置苹果iPhone 14pro灵动岛暗紫色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "stuffStatusTagHeight": "0.0",
                                "stuffStatusTagWidth": "0.0",
                                "title": "女生自用闲置苹果iPhone 14pro灵动岛暗紫色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "女生自用闲置苹果iPhone 14pro灵动岛暗紫色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userActiveUrl": "https://gw.alicdn.com/tfs/TB1zIymVUz1gK0jSZLeXXb9kVXa-30-30.png",
                                "userAvatarUrl": "http://img.alicdn.com/bao/uploaded/i1/O1CN01NltjNJ1oNbdci6O8z_!!0-mtopupload.jpg",
                                "userFishShopLabel": {
                                    "config": {
                                        "delimiterColor": "#D6D6D6",
                                        "delimiterHeight": "12",
                                        "delimiterMarginLeft": "4.5",
                                        "delimiterMarginRight": "4.5",
                                        "delimiterPosition": "between",
                                        "delimiterWidth": "0.5",
                                        "hasDelimiter": "true",
                                        "mutualLabelBizGroup": "true"
                                    },
                                    "tagList": [
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "6条评价",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        },
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "好评率100%",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        }
                                    ]
                                },
                                "userIdentityShow": "",
                                "userIsUseFishShopCard": "false",
                                "userNickName": "诚信第一",
                                "want": ""
                            },
                            "targetUrl": "fleamarket://awesome_detail?id=788636250267&flutter=true&referPageArgs=iphone&gulSource=search&extra=%7B%22labelIds%22%3A%2236%2C38%2C34%2C9%2C750%2C13%22%2C%22source%22%3A%227%22%7D&referPage=Page_xySearchResult&trackParamsJson=%7B%22q%22%3A%22iphone%22%2C%22item_id%22%3A%22788636250267%22%2C%22item_type%22%3A%22goods%22%2C%22index%22%3A%221%22%2C%22page%22%3A%221%22%2C%22id%22%3A%22788636250267%22%2C%22rn%22%3A%227403a9b4d78f5a8665effe56a1b9c058%22%2C%22search_from_page%22%3A%22xyHome%22%2C%22search_id%22%3A%22a5507830d9f36fc69894e2684c958bc9%22%7D"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            },
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "picWidth": "164.0",
                                    "zhimaOffline": "false",
                                    "item_type": "goods",
                                    "disableHierarchicalSort": "0",
                                    "searchProjectLayerInfo": "DoubleShade_21|DEFAULT_26|202305152329_3090_1",
                                    "pageSize": "10",
                                    "type": "1",
                                    "q_type": "0",
                                    "search_from_page": "xyHome",
                                    "tagname": "包邮",
                                    "wantNum": "0",
                                    "id": "788939114686",
                                    "tag": "freeship",
                                    "keyword": "iphone",
                                    "scm": "1007.32845.290827.0",
                                    "seller_id": "yebbZRAuXAJuZikskQujAA==",
                                    "publishTime": "1714207371000",
                                    "search_tab_from": "SEARCH_TAB_MAIN",
                                    "picHeight": "217.0",
                                    "cCatId": "126862528",
                                    "biz_type": "item",
                                    "tbCatId": "1512",
                                    "index": "1",
                                    "spm": "a2170.8011571.1.1",
                                    "catId": "50025386",
                                    "original_q": "iphone",
                                    "p_type": "2",
                                    "page": "1",
                                    "position": "1",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "tcDistance": "0.0",
                                    "abid": "290827",
                                    "singleControl": "false",
                                    "cpvNavWlTbCatId": "1512",
                                    "layerInfo": "22845#0#290827#5_22845#10269#446628#67_22845#12929#480547#54_22845#26994#481509#6_22845#12961#449492#47_22845#26899#481719#11_22845#25306#477353#13_22845#12936#453303#2_22845#12926#482457#52_22845#12928#482555#57",
                                    "item_id": "788939114686",
                                    "oldZhima": "false",
                                    "unShowLabelParams": "{}",
                                    "userIsUseFishShopCard": "false",
                                    "bucketid": "26",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": "a5507830d9f36fc69894e2684c958bc9",
                                    "idle_mount_tai_task_abs": "0:T:1;1192:T:0;768:T:0;793:T:0;130:T:0;343:T:0;467:T:0;573:T:0;1222:T:0;123:T:0;350:T:0;1209:C:1;212:T:0;505:T:0;1193:T:0;354:C:0;353:T:0;892:T:0;972:T:0;193:T:0;370:T:0;-4:C:1;340:T:0;359:T:0;363:T:0;536:T:0;169:T:0;788:T:0;487:T:0;199:T:0;223:T:0;792:T:0;598:T:0;1134:T:0;126:T:0;517:T:0;542:T:0;470:T:0;1229:C:0;356:T:0;593:T:0;-10:T:1;551:T:0;789:T:0;194:T:0;1210:C:0;592:T:0;543:T:0;225:T:0;552:T:0;500:T:0;226:T:0;366:T:0;933:T:0;337:T:0;1156:T:0;1173:T:0;558:T:0;341:T:0;1075:T:0;514:T:0;1190:T:0;244:T:0;893:T:0;969:T:0;227:T:0;1211:T:0;1142:T:0;1185:T:0;361:T:0;368:T:0;1228:C:0;766:T:0;1205:T:0;342:T:0;797:T:0;466:T:0;533:T:0",
                                    "q": "iphone",
                                    "CoinPay_Morediscount": "false",
                                    "isFromAISuggestion": "false",
                                    "tai_match_type": "18",
                                    "HideUserInfo": "false",
                                    "serviceUtParams": "[{\"arg1\":\"4_tag_r2_752\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"22小时前发布\"}},{\"arg1\":\"4_tag_r3_9\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"28人想要\"}},{\"arg1\":\"4_tag_r1_13\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"freeShippingIcon\"}}]",
                                    "labelBucketId": "9",
                                    "zhimaLogBucketId": "9"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "安徽",
                                "detailParams": {
                                    "picWidth": "1080",
                                    "itemId": "788939114686",
                                    "itemType": "detailCommonBuy",
                                    "picHeight": "1434",
                                    "userNick": "晚风温柔",
                                    "soldPrice": "1006",
                                    "isVideo": "false",
                                    "title": "女生自用闲置苹果iPhone 15pro灵动岛原色国行  5 12G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！"
                                },
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "788939114686",
                                            "bizType": "item",
                                            "picHeight": "217.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "2",
                                            "keyword": "iphone",
                                            "referPage": "Page_xySearchResult_FindSimilar"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "itemPicUrl": "http://img.alicdn.com/bao/uploaded/i3/O1CN01uU975i24SfsUdj0vT_!!53-fleamarket.heic",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "yebbZRAuXAJuZikskQujAA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788939114686",
                                                "targetIndex": "2",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "788939114686",
                                                    "bizType": "item",
                                                    "picHeight": "217.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "2",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "yebbZRAuXAJuZikskQujAA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788939114686",
                                                "targetIndex": "2",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "788939114686",
                                                    "bizType": "item",
                                                    "picHeight": "217.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "2",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "yebbZRAuXAJuZikskQujAA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788939114686",
                                                "targetIndex": "2",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "788939114686",
                                                    "bizType": "item",
                                                    "picHeight": "217.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "2",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "yebbZRAuXAJuZikskQujAA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788939114686",
                                                "targetIndex": "2",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "788939114686",
                                                    "bizType": "item",
                                                    "picHeight": "217.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "2",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "yebbZRAuXAJuZikskQujAA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788939114686",
                                                "targetIndex": "2",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "788939114686",
                                                    "bizType": "item",
                                                    "picHeight": "217.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "2",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01nEHAUr1bTw528ELSv_!!6000000003467-2-tps-96-96.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "yebbZRAuXAJuZikskQujAA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788939114686",
                                                "targetIndex": "2",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "788939114686",
                                                    "bizType": "item",
                                                    "picHeight": "217.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "2",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i4/O1CN01d2x4An1z5FVcHazR1_!!6000000006662-2-tps-96-96.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "yebbZRAuXAJuZikskQujAA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788939114686",
                                                "targetIndex": "2",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "788939114686",
                                                    "bizType": "item",
                                                    "picHeight": "217.0",
                                                    "picWicth": "164.0",
                                                    "name": "结果不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "2",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01XMrXCG1W2OB7JmJIY_!!6000000002730-2-tps-96-96.png",
                                            "index": "3",
                                            "text": "结果不相关"
                                        }
                                    ],
                                    "similarTargetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-photo-search/pages/home?kun=true&wh_ttid=native&opaque=false&extra=%7B%22imageInfo%22%3A%7B%22bizCode%22%3A%22graph_similarity%22%2C%22reqFromPage%22%3A%22main_search_feeds_dislike%22%2C%22source%22%3A%22itemPic%22%2C%22url%22%3A%22http%3A%2F%2Fimg.alicdn.com%2Fbao%2Fuploaded%2Fi3%2FO1CN01uU975i24SfsUdj0vT_%21%2153-fleamarket.heic_640x640q90.jpg%22%7D%7D",
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTagCustomParam": {
                                    "feedStyle202208": "1",
                                    "feedStyle202304": "1"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "gradientColors": [
                                                        "#F7F7CC",
                                                        "#FFFFFF"
                                                    ],
                                                    "color": "#48483B",
                                                    "borderRadius": "9",
                                                    "size": "12",
                                                    "labelId": "752",
                                                    "lineHeight": "1.2",
                                                    "gradientDirection": "to right",
                                                    "gradientType": "linear",
                                                    "type": "gradientImageText",
                                                    "content": "22小时前发布",
                                                    "height": "16",
                                                    "leftImage": {
                                                        "marginRight": "2",
                                                        "width": "14",
                                                        "url": "https://gw.alicdn.com/imgextra/i3/O1CN01Z6BeDa1w4qA2xZLFJ_!!6000000006255-2-tps-42-42.png",
                                                        "height": "14",
                                                        "marginLeft": "2"
                                                    }
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "22小时前发布"
                                                    },
                                                    "arg1": "4_tag_r2_752"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "true"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "9",
                                                    "lineHeight": "1.3",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "28人想要",
                                                    "marginLeft": "4"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "28人想要"
                                                    },
                                                    "arg1": "4_tag_r3_9"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r1": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "marginRight": "4",
                                                    "labelId": "13",
                                                    "width": "28",
                                                    "type": "img",
                                                    "alignment": "middle",
                                                    "content": "freeShippingIcon",
                                                    "url": "https://gw.alicdn.com/imgextra/i3/O1CN01PuymOm1I7yIlVyFV9_!!6000000000847-2-tps-84-48.png",
                                                    "height": "16"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "freeShippingIcon"
                                                    },
                                                    "arg1": "4_tag_r1_13"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "false",
                                "isAuction": "false",
                                "itemId": "788939114686",
                                "jump2XianYuHao": {
                                    "clickParam": {
                                        "arg1": "Jump2User",
                                        "args": {
                                            "bucket_id": "26",
                                            "spm": "a2170.8011571.Jump2User.2",
                                            "user_id": "9VqNOYOLgTeQTHkg/H/fnQ==",
                                            "item_id": "788939114686",
                                            "userIsUseFishShopCard": "false",
                                            "HideUserInfo": "false",
                                            "seller_id": "yebbZRAuXAJuZikskQujAA=="
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "targetUrl": "z9xpXnwzz6eu3JHQFPK2nb4PAGLvMlrcMmttP6latEo/1UFGqq2bZyVdepdRQmMhWYG9We1TzWq0EITUfL6a4Eh37joM7WWLUAdqAgxux9w="
                                },
                                "picHeight": "217.75555555555556",
                                "picUrl": "http://img.alicdn.com/bao/uploaded/i3/O1CN01uU975i24SfsUdj0vT_!!53-fleamarket.heic",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1006",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [],
                                "richTitle": [
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1eCD602b2gK0jSZK9XXaEgFXa-84-48.png",
                                            "width": "35.0"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "女生自用闲置苹果iPhone 15pro灵动岛原色国行  5 12G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "stuffStatusTagHeight": "0.0",
                                "stuffStatusTagWidth": "0.0",
                                "title": "女生自用闲置苹果iPhone 15pro灵动岛原色国行  5 12G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "女生自用闲置苹果iPhone 15pro灵动岛原色国行  5 12G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userActiveUrl": "https://gw.alicdn.com/tfs/TB1zIymVUz1gK0jSZLeXXb9kVXa-30-30.png",
                                "userAvatarUrl": "http://img.alicdn.com/bao/uploaded/i2/O1CN01NrWKQL24SfsKpDv2j_!!0-mtopupload.jpg",
                                "userFishShopLabel": {
                                    "config": {
                                        "delimiterColor": "#D6D6D6",
                                        "delimiterHeight": "12",
                                        "delimiterMarginLeft": "4.5",
                                        "delimiterMarginRight": "4.5",
                                        "delimiterPosition": "between",
                                        "delimiterWidth": "0.5",
                                        "hasDelimiter": "true",
                                        "mutualLabelBizGroup": "true"
                                    },
                                    "tagList": [
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "3条评价",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        },
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "好评率100%",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        }
                                    ]
                                },
                                "userIdentityShow": "",
                                "userIsUseFishShopCard": "false",
                                "userNickName": "晚风温柔",
                                "want": ""
                            },
                            "targetUrl": "fleamarket://awesome_detail?id=788939114686&flutter=true&referPageArgs=iphone&gulSource=search&extra=%7B%22labelIds%22%3A%22752%2C9%2C13%22%2C%22source%22%3A%227%22%7D&referPage=Page_xySearchResult&trackParamsJson=%7B%22q%22%3A%22iphone%22%2C%22item_id%22%3A%22788939114686%22%2C%22item_type%22%3A%22goods%22%2C%22index%22%3A%222%22%2C%22page%22%3A%221%22%2C%22id%22%3A%22788939114686%22%2C%22rn%22%3A%227403a9b4d78f5a8665effe56a1b9c058%22%2C%22search_from_page%22%3A%22xyHome%22%2C%22search_id%22%3A%22a5507830d9f36fc69894e2684c958bc9%22%7D"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            },
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "picWidth": "164.0",
                                    "zhimaOffline": "false",
                                    "item_type": "goods",
                                    "disableHierarchicalSort": "0",
                                    "searchProjectLayerInfo": "DoubleShade_21|DEFAULT_26|202305152329_3090_1",
                                    "pageSize": "10",
                                    "type": "1",
                                    "q_type": "0",
                                    "search_from_page": "xyHome",
                                    "tagname": "全新",
                                    "wantNum": "0",
                                    "id": "788890039397",
                                    "tag": "new",
                                    "keyword": "iphone",
                                    "scm": "1007.32845.290827.0",
                                    "seller_id": "Q3OeIlLuVjGYvKnGt8d7ZA==",
                                    "publishTime": "1714206823000",
                                    "search_tab_from": "SEARCH_TAB_MAIN",
                                    "picHeight": "164.0",
                                    "cCatId": "126862528",
                                    "biz_type": "item",
                                    "tbCatId": "1512",
                                    "index": "2",
                                    "spm": "a2170.8011571.1.2",
                                    "catId": "50025386",
                                    "original_q": "iphone",
                                    "p_type": "2",
                                    "page": "1",
                                    "position": "2",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "tcDistance": "0.0",
                                    "abid": "290827",
                                    "singleControl": "false",
                                    "cpvNavWlTbCatId": "1512",
                                    "layerInfo": "22845#0#290827#5_22845#10269#446628#67_22845#12929#480547#54_22845#26994#481509#6_22845#12961#449492#47_22845#26899#481719#11_22845#25306#477353#13_22845#12936#453303#2_22845#12926#482457#52_22845#12928#482555#57",
                                    "item_id": "788890039397",
                                    "oldZhima": "false",
                                    "unShowLabelParams": "{}",
                                    "userIsUseFishShopCard": "false",
                                    "bucketid": "26",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": "a5507830d9f36fc69894e2684c958bc9",
                                    "idle_mount_tai_task_abs": "0:T:1;1192:T:0;768:T:0;793:T:0;130:T:0;343:T:0;467:T:0;573:T:0;1222:T:0;123:T:0;350:T:0;1209:C:0;212:T:0;505:T:0;1193:T:0;354:C:0;353:T:0;892:T:0;972:T:0;193:T:0;370:T:0;-4:C:1;340:T:0;359:T:0;363:T:0;536:T:0;169:T:0;788:T:0;487:T:0;199:T:0;223:T:0;792:T:0;598:T:0;1134:T:0;126:T:0;517:T:0;542:T:0;470:T:0;1229:C:0;356:T:0;593:T:0;-10:T:1;551:T:0;789:T:0;194:T:0;1210:C:0;592:T:0;543:T:0;225:T:0;552:T:0;500:T:0;226:T:0;366:T:0;933:T:0;337:T:0;1156:T:0;1173:T:0;558:T:0;341:T:0;1075:T:0;514:T:0;1190:T:0;244:T:0;893:T:0;969:T:0;227:T:0;1211:T:0;1142:T:0;1185:T:0;361:T:0;368:T:0;1228:C:0;766:T:0;1205:T:0;342:T:0;797:T:0;466:T:0;533:T:0",
                                    "q": "iphone",
                                    "CoinPay_Morediscount": "false",
                                    "isFromAISuggestion": "false",
                                    "tai_match_type": "18",
                                    "HideUserInfo": "false",
                                    "serviceUtParams": "[{\"arg1\":\"4_tag_r2_752\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"22小时前发布\"}},{\"arg1\":\"4_tag_r3_749\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"累计降价82.00元\"}},{\"arg1\":\"4_tag_r3_9\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"9人想要\"}},{\"arg1\":\"4_tag_r4_12\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"芝麻信用优秀\"}}]",
                                    "labelBucketId": "9",
                                    "zhimaLogBucketId": "9"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "广东",
                                "detailParams": {
                                    "picWidth": "1276",
                                    "itemId": "788890039397",
                                    "itemType": "detailCommonBuy",
                                    "picHeight": "1276",
                                    "userNick": "下水道小美",
                                    "soldPrice": "1006",
                                    "isVideo": "false",
                                    "title": "女生自用闲置苹果iPhone 14pro灵动岛暗紫色国行   256G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！"
                                },
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "788890039397",
                                            "bizType": "item",
                                            "picHeight": "164.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "3",
                                            "keyword": "iphone",
                                            "referPage": "Page_xySearchResult_FindSimilar"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "itemPicUrl": "http://img.alicdn.com/bao/uploaded/i2/O1CN01kxuAzW1JSPiAklpQ7_!!0-fleamarket.jpg",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "Q3OeIlLuVjGYvKnGt8d7ZA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788890039397",
                                                "targetIndex": "3",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "788890039397",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "3",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "Q3OeIlLuVjGYvKnGt8d7ZA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788890039397",
                                                "targetIndex": "3",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "788890039397",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "3",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "Q3OeIlLuVjGYvKnGt8d7ZA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788890039397",
                                                "targetIndex": "3",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "788890039397",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "3",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "Q3OeIlLuVjGYvKnGt8d7ZA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788890039397",
                                                "targetIndex": "3",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "788890039397",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "3",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "Q3OeIlLuVjGYvKnGt8d7ZA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788890039397",
                                                "targetIndex": "3",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "788890039397",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "3",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01nEHAUr1bTw528ELSv_!!6000000003467-2-tps-96-96.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "Q3OeIlLuVjGYvKnGt8d7ZA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788890039397",
                                                "targetIndex": "3",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "788890039397",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "3",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i4/O1CN01d2x4An1z5FVcHazR1_!!6000000006662-2-tps-96-96.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "Q3OeIlLuVjGYvKnGt8d7ZA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788890039397",
                                                "targetIndex": "3",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "788890039397",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "结果不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "3",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01XMrXCG1W2OB7JmJIY_!!6000000002730-2-tps-96-96.png",
                                            "index": "3",
                                            "text": "结果不相关"
                                        }
                                    ],
                                    "similarTargetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-photo-search/pages/home?kun=true&wh_ttid=native&opaque=false&extra=%7B%22imageInfo%22%3A%7B%22bizCode%22%3A%22graph_similarity%22%2C%22reqFromPage%22%3A%22main_search_feeds_dislike%22%2C%22source%22%3A%22itemPic%22%2C%22url%22%3A%22http%3A%2F%2Fimg.alicdn.com%2Fbao%2Fuploaded%2Fi2%2FO1CN01kxuAzW1JSPiAklpQ7_%21%210-fleamarket.jpg_640x640q90.jpg%22%7D%7D",
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTagCustomParam": {
                                    "feedStyle202208": "1",
                                    "feedStyle202304": "1"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "gradientColors": [
                                                        "#F7F7CC",
                                                        "#FFFFFF"
                                                    ],
                                                    "color": "#48483B",
                                                    "borderRadius": "9",
                                                    "size": "12",
                                                    "labelId": "752",
                                                    "lineHeight": "1.2",
                                                    "gradientDirection": "to right",
                                                    "gradientType": "linear",
                                                    "type": "gradientImageText",
                                                    "content": "22小时前发布",
                                                    "height": "16",
                                                    "leftImage": {
                                                        "marginRight": "2",
                                                        "width": "14",
                                                        "url": "https://gw.alicdn.com/imgextra/i3/O1CN01Z6BeDa1w4qA2xZLFJ_!!6000000006255-2-tps-42-42.png",
                                                        "height": "14",
                                                        "marginLeft": "2"
                                                    }
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "22小时前发布"
                                                    },
                                                    "arg1": "4_tag_r2_752"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "true"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#FF4400",
                                                    "size": "12",
                                                    "labelId": "749",
                                                    "lineHeight": "1.3",
                                                    "type": "gradientImageText",
                                                    "content": "累计降价82.00元",
                                                    "leftImage": {
                                                        "marginRight": "3",
                                                        "width": "6",
                                                        "url": "https://gw.alicdn.com/imgextra/i4/O1CN01jkcmvf1jktWeur5JU_!!6000000004587-2-tps-18-33.png",
                                                        "height": "11",
                                                        "marginLeft": "2"
                                                    }
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "累计降价82.00元"
                                                    },
                                                    "arg1": "4_tag_r3_749"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "9",
                                                    "lineHeight": "1.3",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "9人想要",
                                                    "marginLeft": "4"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "9人想要"
                                                    },
                                                    "arg1": "4_tag_r3_9"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r4": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "bgColor": "#EFF5FF",
                                                    "color": "#1677FF",
                                                    "borderRadius": "8",
                                                    "size": "11",
                                                    "labelId": "12",
                                                    "borderPaddingLeft": "1",
                                                    "lineHeight": "1.3",
                                                    "borderPaddingRight": "6",
                                                    "type": "gradientImageText",
                                                    "content": "芝麻信用优秀",
                                                    "height": "16",
                                                    "leftImage": {
                                                        "marginRight": "0",
                                                        "width": "12",
                                                        "url": "https://gw.alicdn.com/imgextra/i1/O1CN018ujC6b1wyG65cktUo_!!6000000006376-2-tps-36-36.png",
                                                        "height": "12",
                                                        "marginLeft": "4"
                                                    }
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "芝麻信用优秀"
                                                    },
                                                    "arg1": "4_tag_r4_12"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "false",
                                "isAuction": "false",
                                "itemId": "788890039397",
                                "jump2XianYuHao": {
                                    "clickParam": {
                                        "arg1": "Jump2User",
                                        "args": {
                                            "bucket_id": "26",
                                            "spm": "a2170.8011571.Jump2User.3",
                                            "user_id": "9VqNOYOLgTeQTHkg/H/fnQ==",
                                            "item_id": "788890039397",
                                            "userIsUseFishShopCard": "false",
                                            "HideUserInfo": "false",
                                            "seller_id": "Q3OeIlLuVjGYvKnGt8d7ZA=="
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "targetUrl": "z9xpXnwzz6eu3JHQFPK2nb4PAGLvMlrcMmttP6latEoghjVaGPXWf9lZx56T/TwVXd1INrK48HKjkhtzz6pM0S/CkM0UIhyFbMvvxc7xx+0="
                                },
                                "picHeight": "164.0",
                                "picUrl": "http://img.alicdn.com/bao/uploaded/i2/O1CN01kxuAzW1JSPiAklpQ7_!!0-fleamarket.jpg",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1006",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [],
                                "richTitle": [
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "女生自用闲置苹果iPhone 14pro灵动岛暗紫色国行   256G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "stuffStatusTagHeight": "0.0",
                                "stuffStatusTagWidth": "0.0",
                                "title": "女生自用闲置苹果iPhone 14pro灵动岛暗紫色国行   256G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "女生自用闲置苹果iPhone 14pro灵动岛暗紫色国行   256G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userActiveUrl": "https://gw.alicdn.com/tfs/TB1zIymVUz1gK0jSZLeXXb9kVXa-30-30.png",
                                "userAvatarUrl": "http://img.alicdn.com/bao/uploaded/i3/O1CN01U5B8Vp1JSPh6zFlEA_!!0-mtopupload.jpg",
                                "userFishShopLabel": {
                                    "config": {
                                        "delimiterColor": "#D6D6D6",
                                        "delimiterHeight": "12",
                                        "delimiterMarginLeft": "4.5",
                                        "delimiterMarginRight": "4.5",
                                        "delimiterPosition": "between",
                                        "delimiterWidth": "0.5",
                                        "hasDelimiter": "true",
                                        "mutualLabelBizGroup": "true"
                                    },
                                    "tagList": [
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "1条评价",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        },
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "好评率100%",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        }
                                    ]
                                },
                                "userIdentityShow": "",
                                "userIsUseFishShopCard": "false",
                                "userNickName": "下水道小美",
                                "want": ""
                            },
                            "targetUrl": "fleamarket://awesome_detail?id=788890039397&flutter=true&referPageArgs=iphone&gulSource=search&extra=%7B%22labelIds%22%3A%22752%2C749%2C9%2C12%22%2C%22source%22%3A%227%22%7D&referPage=Page_xySearchResult&trackParamsJson=%7B%22q%22%3A%22iphone%22%2C%22item_id%22%3A%22788890039397%22%2C%22item_type%22%3A%22goods%22%2C%22index%22%3A%223%22%2C%22page%22%3A%221%22%2C%22id%22%3A%22788890039397%22%2C%22rn%22%3A%227403a9b4d78f5a8665effe56a1b9c058%22%2C%22search_from_page%22%3A%22xyHome%22%2C%22search_id%22%3A%22a5507830d9f36fc69894e2684c958bc9%22%7D"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            },
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "picWidth": "164.0",
                                    "zhimaOffline": "false",
                                    "item_type": "goods",
                                    "disableHierarchicalSort": "0",
                                    "searchProjectLayerInfo": "DoubleShade_21|DEFAULT_26|202305152329_3090_1",
                                    "pageSize": "10",
                                    "type": "1",
                                    "q_type": "0",
                                    "search_from_page": "xyHome",
                                    "tagname": "包邮",
                                    "wantNum": "0",
                                    "id": "789388812276",
                                    "tag": "freeship",
                                    "keyword": "iphone",
                                    "scm": "1007.32845.290827.0",
                                    "seller_id": "SiY9GKqpO6dWGxiavjrhaQ==",
                                    "publishTime": "1714284832000",
                                    "search_tab_from": "SEARCH_TAB_MAIN",
                                    "picHeight": "218.0",
                                    "cCatId": "126862528",
                                    "biz_type": "item",
                                    "tbCatId": "1512",
                                    "index": "3",
                                    "spm": "a2170.8011571.1.3",
                                    "catId": "50025386",
                                    "original_q": "iphone",
                                    "p_type": "2",
                                    "page": "1",
                                    "position": "3",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "tcDistance": "0.0",
                                    "abid": "290827",
                                    "singleControl": "false",
                                    "cpvNavWlTbCatId": "1512",
                                    "layerInfo": "22845#0#290827#5_22845#10269#446628#67_22845#12929#480547#54_22845#26994#481509#6_22845#12961#449492#47_22845#26899#481719#11_22845#25306#477353#13_22845#12936#453303#2_22845#12926#482457#52_22845#12928#482555#57",
                                    "item_id": "789388812276",
                                    "oldZhima": "false",
                                    "unShowLabelParams": "{}",
                                    "userIsUseFishShopCard": "false",
                                    "bucketid": "26",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": "a5507830d9f36fc69894e2684c958bc9",
                                    "idle_mount_tai_task_abs": "0:T:1;1192:T:0;768:T:0;793:T:0;130:T:0;343:T:0;467:T:0;1222:T:1;573:T:0;123:T:0;350:T:0;1209:C:0;505:T:0;1193:T:0;212:T:1;354:C:0;353:T:0;892:T:0;972:T:0;193:T:0;370:T:0;-4:C:1;340:T:0;359:T:0;363:T:0;536:T:0;169:T:0;788:T:0;487:T:0;199:T:0;223:T:0;792:T:0;598:T:0;1134:T:0;126:T:0;517:T:0;542:T:0;470:T:0;1229:C:0;356:T:0;593:T:0;-10:T:1;551:T:0;789:T:0;194:T:0;1210:C:0;592:T:0;543:T:0;225:T:0;552:T:0;500:T:0;226:T:0;366:T:0;933:T:0;337:T:0;1156:T:0;1173:T:0;558:T:0;341:T:0;1075:T:0;514:T:0;1190:T:0;244:T:0;893:T:0;969:T:0;227:T:0;1211:T:0;1142:T:0;1185:T:0;361:T:0;368:T:0;1228:C:0;766:T:0;1205:T:0;342:T:0;797:T:0;466:T:0;533:T:0",
                                    "q": "iphone",
                                    "CoinPay_Morediscount": "false",
                                    "isFromAISuggestion": "false",
                                    "tai_match_type": "18",
                                    "HideUserInfo": "false",
                                    "serviceUtParams": "[{\"arg1\":\"4_tag_r2_752\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"1小时前发布\"}},{\"arg1\":\"4_tag_r3_9\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"1人想要\"}},{\"arg1\":\"4_tag_r1_472\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"验货宝\"}}]",
                                    "labelBucketId": "9",
                                    "zhimaLogBucketId": "9"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "河北",
                                "detailParams": {
                                    "picWidth": "1280",
                                    "itemId": "789388812276",
                                    "itemType": "detailCommonBuy",
                                    "picHeight": "1706",
                                    "userNick": "洋ledo",
                                    "soldPrice": "1000",
                                    "isVideo": "false",
                                    "title": "急出女生自用苹果15promax 原色 256g国行手机 双 卡双待 购买半年。\n不怎么用，没有暗病，双卡双待，个人一手自用，支持验机，\n全套齐全几乎全新，所有功能一切正常 没有拆修都是原装，"
                                },
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "789388812276",
                                            "bizType": "item",
                                            "picHeight": "218.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "4",
                                            "keyword": "iphone",
                                            "referPage": "Page_xySearchResult_FindSimilar"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "itemPicUrl": "http://img.alicdn.com/bao/uploaded/i2/O1CN01RjKXE81ZA7kHrPsCg_!!0-fleamarket.jpg",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "SiY9GKqpO6dWGxiavjrhaQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789388812276",
                                                "targetIndex": "4",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "789388812276",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "4",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "SiY9GKqpO6dWGxiavjrhaQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789388812276",
                                                "targetIndex": "4",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "789388812276",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "4",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "SiY9GKqpO6dWGxiavjrhaQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789388812276",
                                                "targetIndex": "4",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "789388812276",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "4",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "SiY9GKqpO6dWGxiavjrhaQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789388812276",
                                                "targetIndex": "4",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "789388812276",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "4",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "SiY9GKqpO6dWGxiavjrhaQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789388812276",
                                                "targetIndex": "4",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "789388812276",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "4",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01nEHAUr1bTw528ELSv_!!6000000003467-2-tps-96-96.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "SiY9GKqpO6dWGxiavjrhaQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789388812276",
                                                "targetIndex": "4",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "789388812276",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "4",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i4/O1CN01d2x4An1z5FVcHazR1_!!6000000006662-2-tps-96-96.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "SiY9GKqpO6dWGxiavjrhaQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789388812276",
                                                "targetIndex": "4",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "789388812276",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "结果不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "4",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01XMrXCG1W2OB7JmJIY_!!6000000002730-2-tps-96-96.png",
                                            "index": "3",
                                            "text": "结果不相关"
                                        }
                                    ],
                                    "similarTargetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-photo-search/pages/home?kun=true&wh_ttid=native&opaque=false&extra=%7B%22imageInfo%22%3A%7B%22bizCode%22%3A%22graph_similarity%22%2C%22reqFromPage%22%3A%22main_search_feeds_dislike%22%2C%22source%22%3A%22itemPic%22%2C%22url%22%3A%22http%3A%2F%2Fimg.alicdn.com%2Fbao%2Fuploaded%2Fi2%2FO1CN01RjKXE81ZA7kHrPsCg_%21%210-fleamarket.jpg_640x640q90.jpg%22%7D%7D",
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTagCustomParam": {
                                    "feedStyle202208": "1",
                                    "feedStyle202304": "1"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "gradientColors": [
                                                        "#F7F7CC",
                                                        "#FFFFFF"
                                                    ],
                                                    "color": "#48483B",
                                                    "borderRadius": "9",
                                                    "size": "12",
                                                    "labelId": "752",
                                                    "lineHeight": "1.2",
                                                    "gradientDirection": "to right",
                                                    "gradientType": "linear",
                                                    "type": "gradientImageText",
                                                    "content": "1小时前发布",
                                                    "height": "16",
                                                    "leftImage": {
                                                        "marginRight": "2",
                                                        "width": "14",
                                                        "url": "https://gw.alicdn.com/imgextra/i3/O1CN01Z6BeDa1w4qA2xZLFJ_!!6000000006255-2-tps-42-42.png",
                                                        "height": "14",
                                                        "marginLeft": "2"
                                                    }
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "1小时前发布"
                                                    },
                                                    "arg1": "4_tag_r2_752"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "true"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "9",
                                                    "lineHeight": "1.3",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "1人想要",
                                                    "marginLeft": "4"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "1人想要"
                                                    },
                                                    "arg1": "4_tag_r3_9"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r1": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "marginRight": "4",
                                                    "labelId": "472",
                                                    "width": "41",
                                                    "type": "img",
                                                    "alignment": "middle",
                                                    "content": "验货宝",
                                                    "url": "https://gw.alicdn.com/imgextra/i3/O1CN01gVzTNw1nMrFzcRUFt_!!6000000005076-2-tps-123-48.png",
                                                    "height": "16"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "验货宝"
                                                    },
                                                    "arg1": "4_tag_r1_472"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "false",
                                "isAuction": "false",
                                "itemId": "789388812276",
                                "jump2XianYuHao": {
                                    "clickParam": {
                                        "arg1": "Jump2User",
                                        "args": {
                                            "bucket_id": "26",
                                            "spm": "a2170.8011571.Jump2User.4",
                                            "user_id": "9VqNOYOLgTeQTHkg/H/fnQ==",
                                            "item_id": "789388812276",
                                            "userIsUseFishShopCard": "false",
                                            "HideUserInfo": "false",
                                            "seller_id": "SiY9GKqpO6dWGxiavjrhaQ=="
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "targetUrl": "z9xpXnwzz6eu3JHQFPK2nb4PAGLvMlrcMmttP6latEqLTNqBTDPvJxF43XgsWv9c49hfzvkKPdftCyWnZzYDOX2VHh8u0oN4p9CgSJDIvYM="
                                },
                                "picHeight": "218.58124999999998",
                                "picUrl": "http://img.alicdn.com/bao/uploaded/i2/O1CN01RjKXE81ZA7kHrPsCg_!!0-fleamarket.jpg",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1000",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [],
                                "richTitle": [
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1nTuTp0Tfau8jSZFwXXX1mVXa-114-48.png",
                                            "width": "47.5"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1eCD602b2gK0jSZK9XXaEgFXa-84-48.png",
                                            "width": "35.0"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "急出女生自用苹果15promax 原色 256g国行手机 双 卡双待 购买半年。不怎么用，没有暗病，双卡双待，个人一手自用，支持验机，全套齐全几乎全新，所有功能一切正常 没有拆修都是原装，",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "stuffStatusTagHeight": "0.0",
                                "stuffStatusTagWidth": "0.0",
                                "title": "急出女生自用苹果15promax 原色 256g国行手机 双 卡双待 购买半年。不怎么用，没有暗病，双卡双待，个人一手自用，支持验机，全套齐全几乎全新，所有功能一切正常 没有拆修都是原装，",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "急出女生自用苹果15promax 原色 256g国行手机 双 卡双待 购买半年。不怎么用，没有暗病，双卡双待，个人一手自用，支持验机，全套齐全几乎全新，所有功能一切正常 没有拆修都是原装，",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userActiveUrl": "https://gw.alicdn.com/tfs/TB1zIymVUz1gK0jSZLeXXb9kVXa-30-30.png",
                                "userAvatarUrl": "http://gtms03.alicdn.com/tps/i3/TB1LFGeKVXXXXbCaXXX07tlTXXX-200-200.png",
                                "userFishShopLabel": {
                                    "config": {
                                        "delimiterColor": "#D6D6D6",
                                        "delimiterHeight": "12",
                                        "delimiterMarginLeft": "4.5",
                                        "delimiterMarginRight": "4.5",
                                        "delimiterPosition": "between",
                                        "delimiterWidth": "0.5",
                                        "hasDelimiter": "true",
                                        "mutualLabelBizGroup": "true"
                                    },
                                    "tagList": [
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "0条评价",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        },
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "好评率0%",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        }
                                    ]
                                },
                                "userIdentityShow": "",
                                "userIsUseFishShopCard": "false",
                                "userNickName": "洋ledo",
                                "want": ""
                            },
                            "targetUrl": "fleamarket://awesome_detail?id=789388812276&flutter=true&referPageArgs=iphone&gulSource=search&extra=%7B%22labelIds%22%3A%22752%2C9%2C472%22%2C%22source%22%3A%227%22%7D&referPage=Page_xySearchResult&trackParamsJson=%7B%22q%22%3A%22iphone%22%2C%22item_id%22%3A%22789388812276%22%2C%22item_type%22%3A%22goods%22%2C%22index%22%3A%224%22%2C%22page%22%3A%221%22%2C%22id%22%3A%22789388812276%22%2C%22rn%22%3A%227403a9b4d78f5a8665effe56a1b9c058%22%2C%22search_from_page%22%3A%22xyHome%22%2C%22search_id%22%3A%22a5507830d9f36fc69894e2684c958bc9%22%7D"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            },
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "picWidth": "164.0",
                                    "zhimaOffline": "false",
                                    "item_type": "goods",
                                    "disableHierarchicalSort": "0",
                                    "searchProjectLayerInfo": "DoubleShade_21|DEFAULT_26|202305152329_3090_1",
                                    "pageSize": "10",
                                    "type": "1",
                                    "q_type": "0",
                                    "search_from_page": "xyHome",
                                    "tagname": "包邮/优秀",
                                    "wantNum": "0",
                                    "id": "783516173983",
                                    "tag": "freeship/credit-5",
                                    "keyword": "iphone",
                                    "scm": "1007.32845.290827.0",
                                    "seller_id": "fZIwCy4VnN8JwpVDqrZSNQ==",
                                    "publishTime": "1712982225000",
                                    "search_tab_from": "SEARCH_TAB_MAIN",
                                    "picHeight": "218.0",
                                    "cCatId": "126862528",
                                    "biz_type": "item",
                                    "tbCatId": "1512",
                                    "index": "4",
                                    "spm": "a2170.8011571.1.4",
                                    "catId": "50025386",
                                    "original_q": "iphone",
                                    "p_type": "2",
                                    "page": "1",
                                    "position": "4",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "tcDistance": "0.0",
                                    "abid": "290827",
                                    "singleControl": "false",
                                    "cpvNavWlTbCatId": "1512",
                                    "layerInfo": "22845#0#290827#5_22845#10269#446628#67_22845#12929#480547#54_22845#26994#481509#6_22845#12961#449492#47_22845#26899#481719#11_22845#25306#477353#13_22845#12936#453303#2_22845#12926#482457#52_22845#12928#482555#57",
                                    "item_id": "783516173983",
                                    "oldZhima": "false",
                                    "unShowLabelParams": "{}",
                                    "userIsUseFishShopCard": "false",
                                    "bucketid": "26",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": "a5507830d9f36fc69894e2684c958bc9",
                                    "idle_mount_tai_task_abs": "0:T:1;1192:T:0;768:T:0;793:T:0;130:T:0;343:T:0;467:T:0;573:T:0;1222:T:0;123:T:0;350:T:0;1209:C:0;505:T:0;1193:T:0;212:T:1;354:C:0;353:T:0;892:T:0;972:T:0;193:T:0;370:T:0;-4:C:1;340:T:0;359:T:0;363:T:0;536:T:0;169:T:0;788:T:0;487:T:0;199:T:0;223:T:0;792:T:0;598:T:0;1134:T:0;126:T:0;517:T:0;542:T:0;470:T:0;1229:C:0;356:T:0;593:T:0;-10:T:1;551:T:0;789:T:0;194:T:0;1210:C:0;592:T:0;543:T:0;225:T:0;552:T:0;500:T:0;226:T:0;366:T:0;933:T:0;337:T:0;1156:T:0;1173:T:0;558:T:0;341:T:0;1075:T:0;514:T:0;1190:T:0;244:T:0;893:T:0;969:T:0;227:T:0;1211:T:0;1142:T:0;1185:T:0;361:T:0;368:T:0;1228:C:0;766:T:0;1205:T:0;342:T:0;797:T:0;466:T:0;533:T:0",
                                    "q": "iphone",
                                    "CoinPay_Morediscount": "false",
                                    "isFromAISuggestion": "false",
                                    "tai_match_type": "14",
                                    "HideUserInfo": "false",
                                    "serviceUtParams": "[{\"arg1\":\"4_tag_r2_36\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"几乎全新\"}},{\"arg1\":\"4_tag_r2_38\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"Apple/苹果\"}},{\"arg1\":\"4_tag_r2_34\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"128GB\"}},{\"arg1\":\"4_tag_r3_9\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"53人想要\"}},{\"arg1\":\"4_tag_r4_12\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"芝麻信用极好\"}},{\"arg1\":\"4_tag_r1_472\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"验货宝\"}}]",
                                    "labelBucketId": "9",
                                    "zhimaLogBucketId": "9"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "浙江",
                                "detailParams": {
                                    "picWidth": "1280",
                                    "itemId": "783516173983",
                                    "itemType": "detailCommonBuy",
                                    "picHeight": "1707",
                                    "userNick": "腾讯腾讯各种业务",
                                    "soldPrice": "1300",
                                    "isVideo": "false",
                                    "title": "iphone13 128G白色，成色99新，要换折叠屏手机， 电池健康95全套盒子都在。不还价，还价不回，成色绝对99新。"
                                },
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "783516173983",
                                            "bizType": "item",
                                            "picHeight": "218.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "5",
                                            "keyword": "iphone",
                                            "referPage": "Page_xySearchResult_FindSimilar"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "itemPicUrl": "http://img.alicdn.com/bao/uploaded/i3/O1CN01QxIcmx1cWVx84w7g2_!!53-fleamarket.heic",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "fZIwCy4VnN8JwpVDqrZSNQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "783516173983",
                                                "targetIndex": "5",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "783516173983",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "5",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "fZIwCy4VnN8JwpVDqrZSNQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "783516173983",
                                                "targetIndex": "5",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "783516173983",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "5",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "fZIwCy4VnN8JwpVDqrZSNQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "783516173983",
                                                "targetIndex": "5",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "783516173983",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "5",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "fZIwCy4VnN8JwpVDqrZSNQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "783516173983",
                                                "targetIndex": "5",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "783516173983",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "5",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "fZIwCy4VnN8JwpVDqrZSNQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "783516173983",
                                                "targetIndex": "5",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "783516173983",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "5",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01nEHAUr1bTw528ELSv_!!6000000003467-2-tps-96-96.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "fZIwCy4VnN8JwpVDqrZSNQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "783516173983",
                                                "targetIndex": "5",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "783516173983",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "5",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i4/O1CN01d2x4An1z5FVcHazR1_!!6000000006662-2-tps-96-96.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "fZIwCy4VnN8JwpVDqrZSNQ==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "783516173983",
                                                "targetIndex": "5",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "783516173983",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "结果不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "5",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01XMrXCG1W2OB7JmJIY_!!6000000002730-2-tps-96-96.png",
                                            "index": "3",
                                            "text": "结果不相关"
                                        }
                                    ],
                                    "similarTargetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-photo-search/pages/home?kun=true&wh_ttid=native&opaque=false&extra=%7B%22imageInfo%22%3A%7B%22bizCode%22%3A%22graph_similarity%22%2C%22reqFromPage%22%3A%22main_search_feeds_dislike%22%2C%22source%22%3A%22itemPic%22%2C%22url%22%3A%22http%3A%2F%2Fimg.alicdn.com%2Fbao%2Fuploaded%2Fi3%2FO1CN01QxIcmx1cWVx84w7g2_%21%2153-fleamarket.heic_640x640q90.jpg%22%7D%7D",
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTagCustomParam": {
                                    "feedStyle202208": "1",
                                    "feedStyle202304": "1"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "36",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "几乎全新"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "几乎全新"
                                                    },
                                                    "arg1": "4_tag_r2_36"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "38",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "Apple/苹果"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "Apple/苹果"
                                                    },
                                                    "arg1": "4_tag_r2_38"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "34",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "128GB"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "128GB"
                                                    },
                                                    "arg1": "4_tag_r2_34"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "delimiterMarginRight": "4.5",
                                            "delimiterWidth": "0.5",
                                            "delimiterPosition": "between",
                                            "delimiterColor": "#D6D6D6",
                                            "delimiterHeight": "10",
                                            "hasDelimiter": "true",
                                            "delimiterMarginLeft": "4.5",
                                            "delimiterMarginBottom": "3",
                                            "mutualLabelBizGroup": "true",
                                            "delimiterMarginTop": "3"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "9",
                                                    "lineHeight": "1.3",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "53人想要",
                                                    "marginLeft": "4"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "53人想要"
                                                    },
                                                    "arg1": "4_tag_r3_9"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r4": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "bgColor": "#EFF5FF",
                                                    "color": "#1677FF",
                                                    "borderRadius": "8",
                                                    "size": "11",
                                                    "labelId": "12",
                                                    "borderPaddingLeft": "1",
                                                    "lineHeight": "1.3",
                                                    "borderPaddingRight": "6",
                                                    "type": "gradientImageText",
                                                    "content": "芝麻信用极好",
                                                    "height": "16",
                                                    "leftImage": {
                                                        "marginRight": "0",
                                                        "width": "12",
                                                        "url": "https://gw.alicdn.com/imgextra/i1/O1CN018ujC6b1wyG65cktUo_!!6000000006376-2-tps-36-36.png",
                                                        "height": "12",
                                                        "marginLeft": "4"
                                                    }
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "芝麻信用极好"
                                                    },
                                                    "arg1": "4_tag_r4_12"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r1": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "marginRight": "4",
                                                    "labelId": "472",
                                                    "width": "41",
                                                    "type": "img",
                                                    "alignment": "middle",
                                                    "content": "验货宝",
                                                    "url": "https://gw.alicdn.com/imgextra/i3/O1CN01gVzTNw1nMrFzcRUFt_!!6000000005076-2-tps-123-48.png",
                                                    "height": "16"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "验货宝"
                                                    },
                                                    "arg1": "4_tag_r1_472"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "false",
                                "isAuction": "false",
                                "itemId": "783516173983",
                                "jump2XianYuHao": {
                                    "clickParam": {
                                        "arg1": "Jump2User",
                                        "args": {
                                            "bucket_id": "26",
                                            "spm": "a2170.8011571.Jump2User.5",
                                            "user_id": "9VqNOYOLgTeQTHkg/H/fnQ==",
                                            "item_id": "783516173983",
                                            "userIsUseFishShopCard": "false",
                                            "HideUserInfo": "false",
                                            "seller_id": "fZIwCy4VnN8JwpVDqrZSNQ=="
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "targetUrl": "z9xpXnwzz6eu3JHQFPK2nb4PAGLvMlrcMmttP6latEqXWmSkhVEEuiq0RCQGjteTi1r3M0lsT+Ph7/LBxhlHgTT/vG9C2//36iEvP9irMwI="
                                },
                                "picHeight": "218.66666666666666",
                                "picUrl": "http://img.alicdn.com/bao/uploaded/i3/O1CN01QxIcmx1cWVx84w7g2_!!53-fleamarket.heic",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1300",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [],
                                "richTitle": [
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1nTuTp0Tfau8jSZFwXXX1mVXa-114-48.png",
                                            "width": "47.5"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1eCD602b2gK0jSZK9XXaEgFXa-84-48.png",
                                            "width": "35.0"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "iphone13 128G白色，成色99新，要换折叠屏手机， 电池健康95全套盒子都在。不还价，还价不回，成色绝对99新。",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "stuffStatusTagHeight": "16.0",
                                "stuffStatusTagUrl": "https://gw.alicdn.com/tfs/TB1656k1XY7gK0jSZKzXXaikpXa-240-48.png",
                                "stuffStatusTagWidth": "80.0",
                                "title": "iphone13 128G白色，成色99新，要换折叠屏手机， 电池健康95全套盒子都在。不还价，还价不回，成色绝对99新。",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "iphone13 128G白色，成色99新，要换折叠屏手机， 电池健康95全套盒子都在。不还价，还价不回，成色绝对99新。",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userActiveUrl": "https://gw.alicdn.com/tfs/TB1zIymVUz1gK0jSZLeXXb9kVXa-30-30.png",
                                "userAvatarUrl": "http://img.alicdn.com/bao/uploaded/i3/O1CN011msh5h1cWVnKJqiN5_!!0-mtopupload.jpg",
                                "userFishShopLabel": {
                                    "config": {
                                        "delimiterColor": "#D6D6D6",
                                        "delimiterHeight": "12",
                                        "delimiterMarginLeft": "4.5",
                                        "delimiterMarginRight": "4.5",
                                        "delimiterPosition": "between",
                                        "delimiterWidth": "0.5",
                                        "hasDelimiter": "true",
                                        "mutualLabelBizGroup": "true"
                                    },
                                    "tagList": [
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "331条评价",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        },
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "好评率99%",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        }
                                    ]
                                },
                                "userIdentityShow": "",
                                "userIsUseFishShopCard": "false",
                                "userNickName": "腾讯腾讯各种业务",
                                "want": ""
                            },
                            "targetUrl": "fleamarket://awesome_detail?id=783516173983&flutter=true&referPageArgs=iphone&gulSource=search&extra=%7B%22labelIds%22%3A%2236%2C38%2C34%2C9%2C12%2C472%22%2C%22source%22%3A%227%22%7D&referPage=Page_xySearchResult&trackParamsJson=%7B%22q%22%3A%22iphone%22%2C%22item_id%22%3A%22783516173983%22%2C%22item_type%22%3A%22goods%22%2C%22index%22%3A%225%22%2C%22page%22%3A%221%22%2C%22id%22%3A%22783516173983%22%2C%22rn%22%3A%227403a9b4d78f5a8665effe56a1b9c058%22%2C%22search_from_page%22%3A%22xyHome%22%2C%22search_id%22%3A%22a5507830d9f36fc69894e2684c958bc9%22%7D"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            },
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "item_type": "ad",
                                    "pageSize": "10",
                                    "pid": "430792_1006",
                                    "type": "1",
                                    "search_from_page": "xyHome",
                                    "tagname": "广告",
                                    "singleControl": "false",
                                    "tag": "ad",
                                    "ad_service_id": "70096838061_70081485976_14041073622_1380082351940",
                                    "keyword": "iphone",
                                    "idle_dynamic_slot_ver": "3",
                                    "item_id": "769244853610",
                                    "biz_type": "ad",
                                    "index": "6",
                                    "bucketid": "26",
                                    "bucketIdForAlimamaAdTest": "18",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": null,
                                    "spm": "a2170.8011571.1.6",
                                    "q": "iphone",
                                    "idle_search_ad_text_ver": "1",
                                    "searchAdIndex": "true",
                                    "expUrl": "http://kgb-ifs.tanx.com/kgb?i=%B9%B8rz%B4%B1%AC%CA7%11%F3%B9%FD%D5%F0%A3%10%25_%FC%0F%3B%F8%B4%83t%BB%976%ED%BB%01%15%E3B%04%C3%E3%9F%112%04i%B7c%AB%9C%EA%14%A7%C8%CBkkT%18%2B0%C5%EC%0A%FC%C3%0C%91%90%3D%09%5C%18%FF%05%14%E4lg%AD%7E%19L%F8R%3C%CF%09i%C9%14%86%29%EC%EBM%98z%5Di%BF%DD%B6K%04%B9%FFC",
                                    "page": "1",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "searchAdIndexNew": "idx3"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "上海",
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "769244853610",
                                            "bizType": "ad",
                                            "picHeight": "164.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "6",
                                            "keyword": "iphone"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "769244853610",
                                                "targetIndex": "6",
                                                "targetType": "ad"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "769244853610",
                                                    "bizType": "ad",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "6",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "769244853610",
                                                "targetIndex": "6",
                                                "targetType": "ad"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "769244853610",
                                                    "bizType": "ad",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "6",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "769244853610",
                                                "targetIndex": "6",
                                                "targetType": "ad"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "769244853610",
                                                    "bizType": "ad",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "6",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "769244853610",
                                                "targetIndex": "6",
                                                "targetType": "ad"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "769244853610",
                                                    "bizType": "ad",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "6",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "769244853610",
                                                "targetIndex": "6",
                                                "targetType": "ad"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "769244853610",
                                                    "bizType": "ad",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "6",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i2/O1CN01lSnvCu2271oKLPY3l_!!6000000007072-2-tps-84-84.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "769244853610",
                                                "targetIndex": "6",
                                                "targetType": "ad"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "769244853610",
                                                    "bizType": "ad",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "6",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01iKwQfB1drrvJlThy9_!!6000000003790-2-tps-84-84.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "769244853610",
                                                "targetIndex": "6",
                                                "targetType": "ad"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "769244853610",
                                                    "bizType": "ad",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "搜索词不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "6",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01IXxKIW1nx2YLN784B_!!6000000005155-2-tps-84-84.png",
                                            "index": "3",
                                            "text": "搜索词不相关"
                                        }
                                    ],
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "labelId": "27",
                                                    "size": "12",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "全新"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "labelId": "27",
                                                    "size": "12",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "超值低价"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "delimiterMarginRight": "4.5",
                                            "delimiterWidth": "0.5",
                                            "delimiterPosition": "between",
                                            "delimiterColor": "#D6D6D6",
                                            "delimiterHeight": "11",
                                            "hasDelimiter": "true",
                                            "delimiterMarginLeft": "4.5",
                                            "mutualLabelBizGroup": "true",
                                            "delimiterMarginTop": "3"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "labelId": "15",
                                                    "size": "12",
                                                    "isStrikeThrough": "true",
                                                    "lineHeight": "1.5",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "¥5000.00",
                                                    "marginLeft": "2"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "labelId": "15",
                                                    "size": "12",
                                                    "isStrikeThrough": "false",
                                                    "lineHeight": "1.5",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "200+人想要",
                                                    "marginLeft": "3"
                                                }
                                            }
                                        ]
                                    },
                                    "r4": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "gradientDirection": "toright",
                                                    "borderPaddingRight": "6",
                                                    "type": "gradientImageText",
                                                    "content": "广告",
                                                    "leftImage": {
                                                        "marginRight": "0",
                                                        "width": "16",
                                                        "url": "https://gw.alicdn.com/imgextra/i1/O1CN01p77SiP1RtuOTRWE8N_!!6000000002170-2-tps-48-48.png",
                                                        "height": "16",
                                                        "marginLeft": "2"
                                                    },
                                                    "gradientColors": [
                                                        "#F7F7F7",
                                                        "#F7F7F7"
                                                    ],
                                                    "bgColor": "#F7F7F7",
                                                    "borderRadius": "8",
                                                    "labelId": "16",
                                                    "size": "11",
                                                    "borderPaddingLeft": "0",
                                                    "gradientType": "linear",
                                                    "lineHeight": "1.3",
                                                    "height": "16"
                                                }
                                            }
                                        ]
                                    },
                                    "r5": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "borderColor": "#FFA17F",
                                                    "color": "#FF4400",
                                                    "borderPaddingRight": "3",
                                                    "type": "text",
                                                    "content": "分期免息",
                                                    "marginLeft": "0",
                                                    "marginRight": "4",
                                                    "borderRadius": "3",
                                                    "labelId": "501",
                                                    "size": "10",
                                                    "borderPaddingLeft": "3",
                                                    "borderWidth": "0.5",
                                                    "lineHeight": "1.3"
                                                }
                                            }
                                        ]
                                    },
                                    "r1": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#0D9EFF",
                                                    "bold": "true",
                                                    "type": "img",
                                                    "content": "freeShippingIcon",
                                                    "url": "https://img.alicdn.com/imgextra/i4/O1CN01M5b5vh1jgm1ZPeNHI_!!6000000004578-2-tps-84-48.png",
                                                    "marginLeft": "0",
                                                    "marginRight": "4",
                                                    "labelId": "24",
                                                    "size": "14",
                                                    "width": "28",
                                                    "lineHeight": "1.1",
                                                    "alignment": "middle",
                                                    "height": "16"
                                                }
                                            }
                                        ]
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "true",
                                "isAuction": "false",
                                "picHeight": "164.0",
                                "picUrl": "http://g.search2.alicdn.com/img/i2/12979683/O1CN01z4yATo2LOs2qxCzt5_!!0-saturn_solar.jpg_sum.jpg",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1300",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [
                                    {
                                        "data": {
                                            "bold": "true",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.6",
                                            "text": "200+人想要",
                                            "textColor": "#FFA3A3A3",
                                            "textSize": "10.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "richTitle": [
                                    {
                                        "data": {
                                            "height": "16.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1eCD602b2gK0jSZK9XXaEgFXa-84-48.png",
                                            "width": "28.0"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "height": "16.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/imgextra/i3/O1CN01gOAXcD1iFv0n1NYwy_!!6000000004384-2-tps-144-48.png",
                                            "width": "48.0"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "Apple/苹果 iPhone XS Max全网通国行苹果xs xsmax手机分期免息",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "singleStyleFishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "labelId": "27",
                                                    "size": "12",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "全新"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "labelId": "27",
                                                    "size": "12",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "超值低价"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "delimiterMarginRight": "4.5",
                                            "delimiterWidth": "0.5",
                                            "delimiterPosition": "between",
                                            "delimiterColor": "#D6D6D6",
                                            "delimiterHeight": "11",
                                            "hasDelimiter": "true",
                                            "delimiterMarginLeft": "4.5",
                                            "mutualLabelBizGroup": "true",
                                            "delimiterMarginTop": "3"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "labelId": "15",
                                                    "size": "12",
                                                    "isStrikeThrough": "true",
                                                    "lineHeight": "1",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "¥5000.00",
                                                    "marginLeft": "2"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "labelId": "15",
                                                    "size": "12",
                                                    "isStrikeThrough": "false",
                                                    "lineHeight": "1",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "200+人想要",
                                                    "marginLeft": "3"
                                                }
                                            }
                                        ]
                                    },
                                    "r4": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "gradientDirection": "toright",
                                                    "borderPaddingRight": "6",
                                                    "type": "gradientImageText",
                                                    "content": "广告",
                                                    "gradientColors": [
                                                        "#F7F7F7",
                                                        "#F7F7F7"
                                                    ],
                                                    "bgColor": "#F7F7F7",
                                                    "borderRadius": "8",
                                                    "labelId": "16",
                                                    "size": "11",
                                                    "borderPaddingLeft": "6",
                                                    "gradientType": "linear",
                                                    "lineHeight": "1.3",
                                                    "height": "16"
                                                }
                                            }
                                        ]
                                    },
                                    "r5": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "borderColor": "#FFA17F",
                                                    "color": "#FF4400",
                                                    "borderPaddingRight": "3",
                                                    "type": "text",
                                                    "content": "分期免息",
                                                    "marginLeft": "0",
                                                    "marginRight": "4",
                                                    "borderRadius": "3",
                                                    "labelId": "501",
                                                    "size": "10",
                                                    "borderPaddingLeft": "3",
                                                    "borderWidth": "0.5",
                                                    "lineHeight": "1.3"
                                                }
                                            }
                                        ]
                                    },
                                    "r1": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#0D9EFF",
                                                    "bold": "true",
                                                    "type": "img",
                                                    "content": "freeShippingIcon",
                                                    "url": "https://img.alicdn.com/imgextra/i4/O1CN01M5b5vh1jgm1ZPeNHI_!!6000000004578-2-tps-84-48.png",
                                                    "marginLeft": "0",
                                                    "marginRight": "4",
                                                    "labelId": "24",
                                                    "size": "14",
                                                    "width": "28",
                                                    "lineHeight": "1.1",
                                                    "alignment": "middle",
                                                    "height": "16"
                                                }
                                            }
                                        ]
                                    }
                                },
                                "stuffStatusTagHeight": "16.0",
                                "stuffStatusTagUrl": "https://gw.alicdn.com/imgextra/i2/O1CN01b14ybA1jqqcOrtBWI_!!6000000004600-2-tps-90-48.png",
                                "stuffStatusTagWidth": "30.0",
                                "title": "Apple/苹果 iPhone XS Max全网通国行苹果xs xsmax手机分期免息",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "Apple/苹果 iPhone XS Max全网通国行苹果xs xsmax手机分期免息",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userAvatarUrl": "http://gdp.alicdn.com/shop-logo/https://img.alicdn.com/imgextra/i1/53142010/O1CN01k6t2891Qid24uukUh_!!53142010.jpg",
                                "want": "200+人想要"
                            },
                            "targetUrl": "http://item.taobao.com/item.htm?id=769244853610&etype=1&eurl=http%3A%2F%2Fmclick.simba.taobao.com%2Fcc_im%3Fp%3Diphone%26s%3D1418995303%26k%3D1549%26e%3DwLRaZU8VkTAHq%252FGrc4HmFQeyS8eyxLF9ipxkZImB6DZZqouXlanfDovNCQpZ5Uu1QhZY%252BAx1hn%252FYlAQd6wTX1p8nEAhgSDf46cFRvR%252F6%252BvBbdLWQv8Wp%252BBoZlNyEcQ3kpjAdbcDL9V9h1X7bLllWibiI3dloCfklpshghcklSIp9U1ZwE4utuzPugDj3%252BVEcFUEY%252F3IqxbUpRvskclWLD8S5mle8XSel4UZs38eqJ8bCfPKOBpdCfZNQQPNLJlnYH%252BLR9FWajrhqkG7iKY5Qkj93w9PRiE1Q6K8%252FoEV01NOOLyBvvcYmm6eGnMkET3KTX7wXxUABh%252FCv44%252FQWo8aVwhYsumtG1oiPcjcVihx3Af1d2C7sTWn3ThxCu5ODCCdE%252FL3IQfC6yA6FVF9wgyhIIimEiswyC5HTDvQ8NVOd5QieefCy24q5cNF4Cl%252F6qOIB7lqwkpVF%252BroliZBWmKXlihXvvjXyOivdrtkchrYu%252Bx9dHXrn4XrCpue0hNRIkhRHXU3DsbcMUchXxv1tKcdIlojjywaYoSvgJMxAb%252B7DbBUqQSB7UZZzXUEbV7rwseCF9R%252BBYgAUwF%252BK%252FMsVm9it09cUPq9u1ioZIwEwbYqZlOZNDOTuWnclDq0pouKf6Xc8Tcd2eeceCKolR2B0wscFWDM%252B9z7eJNvRdI0rE0%252Fcb4tbjJfgrfKL9nCTrfcfa3HYyOe6ilKgdBTm84z3Lwu1Ph5cljoercxyKhMYXk2d6EHNau%252B%252F7d54gBMaS1Kmy%252Bc9Wzx8gHBToNEXN1B8jyUEmoNIVRJyvM%252FVks8sc4z6cWybIVHjuEPNLaCDaUDcD0EfITY3WEr7raY0rcyK0ssaM7w1FF%252BOt3ER5mJ2zBbtLwZBitJTZUXpsbEMhvisutSePMdJtH3BPAzK4sjX7diYTK30AxrxMTcYPlJ8fCygCA6ZCWSwAAmRvKwybeNEED5%252FssLeVXNYWUg6SNaHXQZW7z1imcsgRzIlxrOYzC1%252FArwEk%252FYXA5bpoUyP%252BPdy3wH6auoG6dDWfha2uA3n4tCv3%252BbMn6aSu4mw0XgKX%252Fqo4htJImVg1GW2xVIXCacmr%252FeiKYSKzDILkfw1jq%252BW4GUZeiWJkFaYpeWXUl6pjA0f1A2gExtFAa8uBITLCk%252B5bYr%252BLKMPM6hPnyN86uPWlZ7SuKIfBH1pxYV8hbPNtrC7iMX28QT9l65YScKG9tOXa09viUI3LSg1tcaMYlyyMGjCNeOvep4F4VGZJSuHxRFvx99bEjhY7jokS6OAFgCssmbvU15hDuO0RY7poDwlLXi7Kit2ZDmCt4Bw7wIHyI7ylF0vFxJSi7zcfZ6%252BYb9QFSFPu%252Baugom%252BlpbRMUU06mt72Hy6E4h8WFAQDYoAhMk648fd8lasaed5u6EAOhaAvIWYBvkpswM3ciBXLwjGn5e9vpRMqs6j7QzXj%252FMEhm4xO%252F5156YRozCBq6l7W6RjQoE1MQULPg1TjZU%252Fi3AOyrqGBfbxBP2XrlhqwDglCeruZkBzi8O%252F5BMR3JT9%252F3IKHvF74CSrXsImUk%253D%26eadt%3D1%26ver%3D18&epid=430792_1006&cityid=138&bidword=%E8%8B%B9%E6%9E%9C%E6%89%8B%E6%9C%BA%E5%85%A8%E6%96%B0&bc_fl_src=alimama_direct_xianyu_430792_1006&disableSJ=true"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            },
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "picWidth": "164.0",
                                    "zhimaOffline": "false",
                                    "item_type": "goods",
                                    "disableHierarchicalSort": "0",
                                    "searchProjectLayerInfo": "DoubleShade_21|DEFAULT_26|202305152329_3090_1",
                                    "pageSize": "10",
                                    "type": "1",
                                    "q_type": "0",
                                    "search_from_page": "xyHome",
                                    "tagname": "全新/包邮/极好",
                                    "wantNum": "0",
                                    "id": "788456099426",
                                    "tag": "new/freeship/credit-6",
                                    "keyword": "iphone",
                                    "scm": "1007.32845.290827.0",
                                    "seller_id": "u0ruluXBixRVs5K8Con0gA==",
                                    "publishTime": "1714113736000",
                                    "search_tab_from": "SEARCH_TAB_MAIN",
                                    "picHeight": "218.0",
                                    "cCatId": "126862528",
                                    "biz_type": "item",
                                    "tbCatId": "1512",
                                    "index": "5",
                                    "spm": "a2170.8011571.1.5",
                                    "catId": "50025386",
                                    "original_q": "iphone",
                                    "p_type": "2",
                                    "page": "1",
                                    "position": "5",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "tcDistance": "0.0",
                                    "abid": "290827",
                                    "singleControl": "false",
                                    "cpvNavWlTbCatId": "1512",
                                    "layerInfo": "22845#0#290827#5_22845#10269#446628#67_22845#12929#480547#54_22845#26994#481509#6_22845#12961#449492#47_22845#26899#481719#11_22845#25306#477353#13_22845#12936#453303#2_22845#12926#482457#52_22845#12928#482555#57",
                                    "item_id": "788456099426",
                                    "oldZhima": "false",
                                    "unShowLabelParams": "{}",
                                    "userIsUseFishShopCard": "false",
                                    "bucketid": "26",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": "a5507830d9f36fc69894e2684c958bc9",
                                    "idle_mount_tai_task_abs": "0:T:1;1192:T:0;768:T:0;793:T:0;130:T:0;343:T:0;467:T:0;573:T:0;1222:T:0;123:T:0;350:T:0;1209:C:0;212:T:0;505:T:0;1193:T:0;354:C:0;353:T:0;892:T:0;972:T:0;193:T:0;370:T:0;-4:C:1;340:T:0;359:T:0;363:T:0;536:T:0;169:T:0;788:T:0;487:T:0;199:T:0;223:T:0;792:T:0;598:T:0;1134:T:0;126:T:0;517:T:0;542:T:0;470:T:0;1229:C:0;356:T:0;593:T:0;-10:T:1;551:T:0;789:T:0;194:T:0;1210:C:0;592:T:0;543:T:0;225:T:0;552:T:0;500:T:0;226:T:0;366:T:0;933:T:0;337:T:0;1156:T:0;1173:T:0;558:T:0;341:T:0;1075:T:0;514:T:0;1190:T:0;244:T:0;893:T:0;969:T:0;227:T:0;1211:T:0;1142:T:0;1185:T:0;361:T:0;368:T:0;1228:C:0;766:T:0;1205:T:0;342:T:0;797:T:0;466:T:0;533:T:0",
                                    "q": "iphone",
                                    "CoinPay_Morediscount": "false",
                                    "isFromAISuggestion": "false",
                                    "tai_match_type": "0",
                                    "HideUserInfo": "false",
                                    "serviceUtParams": "[{\"arg1\":\"4_tag_r2_36\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"全新未拆封\"}},{\"arg1\":\"4_tag_r2_38\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"Apple/苹果\"}},{\"arg1\":\"4_tag_r2_34\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"512GB\"}},{\"arg1\":\"4_tag_r3_9\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"5人想要\"}},{\"arg1\":\"4_tag_r1_472\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"验货宝\"}}]",
                                    "labelBucketId": "9",
                                    "zhimaLogBucketId": "9"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "江苏",
                                "detailParams": {
                                    "picWidth": "1280",
                                    "itemId": "788456099426",
                                    "itemType": "detailCommonBuy",
                                    "picHeight": "1706",
                                    "userNick": "迷茫的小?",
                                    "soldPrice": "1005",
                                    "isVideo": "false",
                                    "title": "闲置苹果15promax国行512G。白色成色99新 电池容 量100，全网通，双卡双待，纯原装，无拆无修，没有磕碰，没有暗病，没有划痕，因为换了华为手机了 手机所有功能都正常的使用，面容好用，支持15天无理由退货，"
                                },
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "788456099426",
                                            "bizType": "item",
                                            "picHeight": "218.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "7",
                                            "keyword": "iphone",
                                            "referPage": "Page_xySearchResult_FindSimilar"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "itemPicUrl": "http://img.alicdn.com/bao/uploaded/i1/O1CN01hmcbPH2Hjhbkui08T_!!53-fleamarket.heic",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "u0ruluXBixRVs5K8Con0gA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788456099426",
                                                "targetIndex": "7",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "788456099426",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "7",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "u0ruluXBixRVs5K8Con0gA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788456099426",
                                                "targetIndex": "7",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "788456099426",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "7",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "u0ruluXBixRVs5K8Con0gA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788456099426",
                                                "targetIndex": "7",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "788456099426",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "7",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "u0ruluXBixRVs5K8Con0gA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788456099426",
                                                "targetIndex": "7",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "788456099426",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "7",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "u0ruluXBixRVs5K8Con0gA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788456099426",
                                                "targetIndex": "7",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "788456099426",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "7",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01nEHAUr1bTw528ELSv_!!6000000003467-2-tps-96-96.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "u0ruluXBixRVs5K8Con0gA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788456099426",
                                                "targetIndex": "7",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "788456099426",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "7",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i4/O1CN01d2x4An1z5FVcHazR1_!!6000000006662-2-tps-96-96.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "u0ruluXBixRVs5K8Con0gA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "788456099426",
                                                "targetIndex": "7",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "788456099426",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "结果不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "7",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01XMrXCG1W2OB7JmJIY_!!6000000002730-2-tps-96-96.png",
                                            "index": "3",
                                            "text": "结果不相关"
                                        }
                                    ],
                                    "similarTargetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-photo-search/pages/home?kun=true&wh_ttid=native&opaque=false&extra=%7B%22imageInfo%22%3A%7B%22bizCode%22%3A%22graph_similarity%22%2C%22reqFromPage%22%3A%22main_search_feeds_dislike%22%2C%22source%22%3A%22itemPic%22%2C%22url%22%3A%22http%3A%2F%2Fimg.alicdn.com%2Fbao%2Fuploaded%2Fi1%2FO1CN01hmcbPH2Hjhbkui08T_%21%2153-fleamarket.heic_640x640q90.jpg%22%7D%7D",
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTagCustomParam": {
                                    "feedStyle202208": "1",
                                    "feedStyle202304": "1"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "36",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "全新未拆封"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "全新未拆封"
                                                    },
                                                    "arg1": "4_tag_r2_36"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "38",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "Apple/苹果"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "Apple/苹果"
                                                    },
                                                    "arg1": "4_tag_r2_38"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "34",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "512GB"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "512GB"
                                                    },
                                                    "arg1": "4_tag_r2_34"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "delimiterMarginRight": "4.5",
                                            "delimiterWidth": "0.5",
                                            "delimiterPosition": "between",
                                            "delimiterColor": "#D6D6D6",
                                            "delimiterHeight": "10",
                                            "hasDelimiter": "true",
                                            "delimiterMarginLeft": "4.5",
                                            "delimiterMarginBottom": "3",
                                            "mutualLabelBizGroup": "true",
                                            "delimiterMarginTop": "3"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "9",
                                                    "lineHeight": "1.3",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "5人想要",
                                                    "marginLeft": "4"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "5人想要"
                                                    },
                                                    "arg1": "4_tag_r3_9"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r1": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "marginRight": "4",
                                                    "labelId": "472",
                                                    "width": "41",
                                                    "type": "img",
                                                    "alignment": "middle",
                                                    "content": "验货宝",
                                                    "url": "https://gw.alicdn.com/imgextra/i3/O1CN01gVzTNw1nMrFzcRUFt_!!6000000005076-2-tps-123-48.png",
                                                    "height": "16"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "验货宝"
                                                    },
                                                    "arg1": "4_tag_r1_472"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "false",
                                "isAuction": "false",
                                "itemId": "788456099426",
                                "jump2XianYuHao": {
                                    "clickParam": {
                                        "arg1": "Jump2User",
                                        "args": {
                                            "bucket_id": "26",
                                            "spm": "a2170.8011571.Jump2User.7",
                                            "user_id": "9VqNOYOLgTeQTHkg/H/fnQ==",
                                            "item_id": "788456099426",
                                            "userIsUseFishShopCard": "false",
                                            "HideUserInfo": "false",
                                            "seller_id": "u0ruluXBixRVs5K8Con0gA=="
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "targetUrl": "z9xpXnwzz6eu3JHQFPK2nb4PAGLvMlrcMmttP6latErYW4R6IwVHckT/LrbSyVN+YsOs+PNA9Fizgw6pZVUwuzZPXVLVVgSH0Ra6fHXCXFc="
                                },
                                "picHeight": "218.58124999999998",
                                "picUrl": "http://img.alicdn.com/bao/uploaded/i1/O1CN01hmcbPH2Hjhbkui08T_!!53-fleamarket.heic",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1005",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [],
                                "richTitle": [
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1nTuTp0Tfau8jSZFwXXX1mVXa-114-48.png",
                                            "width": "47.5"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1eCD602b2gK0jSZK9XXaEgFXa-84-48.png",
                                            "width": "35.0"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "闲置苹果15promax国行512G。白色成色99新 电池容 量100，全网通，双卡双待，纯原装，无拆无修，没有磕碰，没有暗病，没有划痕，因为换了华为手机了 手机所有功能都正常的使用，面容好用，支持15天无理由退货，",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "stuffStatusTagHeight": "16.0",
                                "stuffStatusTagUrl": "https://gw.alicdn.com/tfs/TB1nehXk4vbeK8jSZPfXXariXXa-240-48.png",
                                "stuffStatusTagWidth": "80.0",
                                "title": "闲置苹果15promax国行512G。白色成色99新 电池容 量100，全网通，双卡双待，纯原装，无拆无修，没有磕碰，没有暗病，没有划痕，因为换了华为手机了 手机所有功能都正常的使用，面容好用，支持15天无理由退货，",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "闲置苹果15promax国行512G。白色成色99新 电池容 量100，全网通，双卡双待，纯原装，无拆无修，没有磕碰，没有暗病，没有划痕，因为换了华为手机了 手机所有功能都正常的使用，面容好用，支持15天无理由退货，",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userActiveUrl": "https://gw.alicdn.com/tfs/TB1zIymVUz1gK0jSZLeXXb9kVXa-30-30.png",
                                "userAvatarUrl": "http://img.alicdn.com/bao/uploaded/i1/T1DRj7Xn8cXXb1upjX.jpg",
                                "userFishShopLabel": {
                                    "config": {
                                        "delimiterColor": "#D6D6D6",
                                        "delimiterHeight": "12",
                                        "delimiterMarginLeft": "4.5",
                                        "delimiterMarginRight": "4.5",
                                        "delimiterPosition": "between",
                                        "delimiterWidth": "0.5",
                                        "hasDelimiter": "true",
                                        "mutualLabelBizGroup": "true"
                                    },
                                    "tagList": [
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "6条评价",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        },
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "好评率100%",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        }
                                    ]
                                },
                                "userIdentityShow": "",
                                "userIsUseFishShopCard": "false",
                                "userNickName": "迷茫的小?",
                                "want": ""
                            },
                            "targetUrl": "fleamarket://awesome_detail?id=788456099426&flutter=true&referPageArgs=iphone&gulSource=search&extra=%7B%22labelIds%22%3A%2236%2C38%2C34%2C9%2C472%22%2C%22source%22%3A%227%22%7D&referPage=Page_xySearchResult&trackParamsJson=%7B%22q%22%3A%22iphone%22%2C%22item_id%22%3A%22788456099426%22%2C%22item_type%22%3A%22goods%22%2C%22index%22%3A%227%22%2C%22page%22%3A%221%22%2C%22id%22%3A%22788456099426%22%2C%22rn%22%3A%227403a9b4d78f5a8665effe56a1b9c058%22%2C%22search_from_page%22%3A%22xyHome%22%2C%22search_id%22%3A%22a5507830d9f36fc69894e2684c958bc9%22%7D"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            },
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "picWidth": "164.0",
                                    "zhimaOffline": "false",
                                    "item_type": "goods",
                                    "disableHierarchicalSort": "0",
                                    "searchProjectLayerInfo": "DoubleShade_21|DEFAULT_26|202305152329_3090_1",
                                    "pageSize": "10",
                                    "type": "1",
                                    "q_type": "0",
                                    "search_from_page": "xyHome",
                                    "tagname": "全新/良好",
                                    "wantNum": "0",
                                    "id": "789173665224",
                                    "tag": "new/credit-4",
                                    "keyword": "iphone",
                                    "scm": "1007.32845.290827.0",
                                    "seller_id": "znjdihFGY79CUlM8dbb8zg==",
                                    "publishTime": "1714236527000",
                                    "search_tab_from": "SEARCH_TAB_MAIN",
                                    "picHeight": "218.0",
                                    "cCatId": "126862528",
                                    "biz_type": "item",
                                    "tbCatId": "1512",
                                    "index": "6",
                                    "spm": "a2170.8011571.1.6",
                                    "catId": "50025386",
                                    "original_q": "iphone",
                                    "p_type": "2",
                                    "page": "1",
                                    "position": "6",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "tcDistance": "0.0",
                                    "abid": "290827",
                                    "singleControl": "false",
                                    "cpvNavWlTbCatId": "1512",
                                    "layerInfo": "22845#0#290827#5_22845#10269#446628#67_22845#12929#480547#54_22845#26994#481509#6_22845#12961#449492#47_22845#26899#481719#11_22845#25306#477353#13_22845#12936#453303#2_22845#12926#482457#52_22845#12928#482555#57",
                                    "item_id": "789173665224",
                                    "oldZhima": "false",
                                    "unShowLabelParams": "{}",
                                    "userIsUseFishShopCard": "false",
                                    "bucketid": "26",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": "a5507830d9f36fc69894e2684c958bc9",
                                    "idle_mount_tai_task_abs": "0:T:1;1192:T:0;768:T:0;793:T:0;130:T:0;343:T:0;467:T:0;573:T:0;1222:T:0;123:T:0;350:T:0;1209:C:0;212:T:0;505:T:0;1193:T:0;354:C:0;353:T:0;892:T:0;972:T:0;193:T:0;370:T:0;-4:C:1;340:T:0;359:T:0;363:T:0;536:T:0;169:T:0;788:T:0;487:T:0;199:T:0;223:T:0;792:T:0;598:T:0;1134:T:0;126:T:0;517:T:0;542:T:0;470:T:0;1229:C:0;356:T:0;593:T:0;-10:T:1;551:T:0;789:T:0;194:T:0;1210:C:0;592:T:0;543:T:0;225:T:0;552:T:0;500:T:0;226:T:0;366:T:0;933:T:0;337:T:0;1156:T:0;1173:T:0;558:T:0;341:T:0;1075:T:0;514:T:0;1190:T:0;244:T:0;893:T:0;969:T:0;227:T:0;1211:T:0;1142:T:0;1185:T:0;361:T:0;368:T:0;1228:C:0;766:T:0;1205:T:0;342:T:0;797:T:0;466:T:0;533:T:0",
                                    "q": "iphone",
                                    "CoinPay_Morediscount": "false",
                                    "isFromAISuggestion": "false",
                                    "tai_match_type": "18",
                                    "HideUserInfo": "false",
                                    "serviceUtParams": "[{\"arg1\":\"4_tag_r2_752\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"14小时前发布\"}},{\"arg1\":\"4_tag_r3_9\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"4人想要\"}}]",
                                    "labelBucketId": "9",
                                    "zhimaLogBucketId": "9"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "云南",
                                "detailParams": {
                                    "picWidth": "1080",
                                    "itemId": "789173665224",
                                    "itemType": "detailCommonBuy",
                                    "picHeight": "1440",
                                    "userNick": "三一一丫",
                                    "soldPrice": "1006",
                                    "isVideo": "false",
                                    "title": "女生自用闲置苹果iPhone 14pro灵动岛银白色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！"
                                },
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "789173665224",
                                            "bizType": "item",
                                            "picHeight": "218.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "8",
                                            "keyword": "iphone",
                                            "referPage": "Page_xySearchResult_FindSimilar"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "itemPicUrl": "http://img.alicdn.com/bao/uploaded/i4/O1CN018fppgT1vIIMRPxi07_!!53-fleamarket.heic",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "znjdihFGY79CUlM8dbb8zg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789173665224",
                                                "targetIndex": "8",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "789173665224",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "8",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "znjdihFGY79CUlM8dbb8zg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789173665224",
                                                "targetIndex": "8",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "789173665224",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "8",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "znjdihFGY79CUlM8dbb8zg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789173665224",
                                                "targetIndex": "8",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "789173665224",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "8",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "znjdihFGY79CUlM8dbb8zg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789173665224",
                                                "targetIndex": "8",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "789173665224",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "8",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "znjdihFGY79CUlM8dbb8zg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789173665224",
                                                "targetIndex": "8",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "789173665224",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "8",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01nEHAUr1bTw528ELSv_!!6000000003467-2-tps-96-96.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "znjdihFGY79CUlM8dbb8zg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789173665224",
                                                "targetIndex": "8",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "789173665224",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "8",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i4/O1CN01d2x4An1z5FVcHazR1_!!6000000006662-2-tps-96-96.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "znjdihFGY79CUlM8dbb8zg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789173665224",
                                                "targetIndex": "8",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "789173665224",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "结果不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "8",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01XMrXCG1W2OB7JmJIY_!!6000000002730-2-tps-96-96.png",
                                            "index": "3",
                                            "text": "结果不相关"
                                        }
                                    ],
                                    "similarTargetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-photo-search/pages/home?kun=true&wh_ttid=native&opaque=false&extra=%7B%22imageInfo%22%3A%7B%22bizCode%22%3A%22graph_similarity%22%2C%22reqFromPage%22%3A%22main_search_feeds_dislike%22%2C%22source%22%3A%22itemPic%22%2C%22url%22%3A%22http%3A%2F%2Fimg.alicdn.com%2Fbao%2Fuploaded%2Fi4%2FO1CN018fppgT1vIIMRPxi07_%21%2153-fleamarket.heic_640x640q90.jpg%22%7D%7D",
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTagCustomParam": {
                                    "feedStyle202208": "1",
                                    "feedStyle202304": "1"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "gradientColors": [
                                                        "#F7F7CC",
                                                        "#FFFFFF"
                                                    ],
                                                    "color": "#48483B",
                                                    "borderRadius": "9",
                                                    "size": "12",
                                                    "labelId": "752",
                                                    "lineHeight": "1.2",
                                                    "gradientDirection": "to right",
                                                    "gradientType": "linear",
                                                    "type": "gradientImageText",
                                                    "content": "14小时前发布",
                                                    "height": "16",
                                                    "leftImage": {
                                                        "marginRight": "2",
                                                        "width": "14",
                                                        "url": "https://gw.alicdn.com/imgextra/i3/O1CN01Z6BeDa1w4qA2xZLFJ_!!6000000006255-2-tps-42-42.png",
                                                        "height": "14",
                                                        "marginLeft": "2"
                                                    }
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "14小时前发布"
                                                    },
                                                    "arg1": "4_tag_r2_752"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "true"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "9",
                                                    "lineHeight": "1.3",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "4人想要",
                                                    "marginLeft": "4"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "4人想要"
                                                    },
                                                    "arg1": "4_tag_r3_9"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "false",
                                "isAuction": "false",
                                "itemId": "789173665224",
                                "jump2XianYuHao": {
                                    "clickParam": {
                                        "arg1": "Jump2User",
                                        "args": {
                                            "bucket_id": "26",
                                            "spm": "a2170.8011571.Jump2User.8",
                                            "user_id": "9VqNOYOLgTeQTHkg/H/fnQ==",
                                            "item_id": "789173665224",
                                            "userIsUseFishShopCard": "false",
                                            "HideUserInfo": "false",
                                            "seller_id": "znjdihFGY79CUlM8dbb8zg=="
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "targetUrl": "z9xpXnwzz6eu3JHQFPK2nb4PAGLvMlrcMmttP6latEoPMLzS5KXEXTmJP2neMJkERKkeWV/1IcPKxZARlWVDVw1IGBawano235xY0B6bQ9M="
                                },
                                "picHeight": "218.66666666666666",
                                "picUrl": "http://img.alicdn.com/bao/uploaded/i4/O1CN018fppgT1vIIMRPxi07_!!53-fleamarket.heic",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1006",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [],
                                "richTitle": [
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "女生自用闲置苹果iPhone 14pro灵动岛银白色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "stuffStatusTagHeight": "16.0",
                                "stuffStatusTagUrl": "https://gw.alicdn.com/tfs/TB1756k1XY7gK0jSZKzXXaikpXa-240-48.png",
                                "stuffStatusTagWidth": "80.0",
                                "title": "女生自用闲置苹果iPhone 14pro灵动岛银白色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "女生自用闲置苹果iPhone 14pro灵动岛银白色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userActiveUrl": "https://gw.alicdn.com/tfs/TB1zIymVUz1gK0jSZLeXXb9kVXa-30-30.png",
                                "userAvatarUrl": "http://img.alicdn.com/bao/uploaded/i2/3026676149/TB28exmb1IPyuJjSspcXXXiApXa_!!0-mytaobao.jpg",
                                "userFishShopLabel": {
                                    "config": {
                                        "delimiterColor": "#D6D6D6",
                                        "delimiterHeight": "12",
                                        "delimiterMarginLeft": "4.5",
                                        "delimiterMarginRight": "4.5",
                                        "delimiterPosition": "between",
                                        "delimiterWidth": "0.5",
                                        "hasDelimiter": "true",
                                        "mutualLabelBizGroup": "true"
                                    },
                                    "tagList": [
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "1条评价",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        },
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "好评率0%",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        }
                                    ]
                                },
                                "userIdentityShow": "",
                                "userIsUseFishShopCard": "false",
                                "userNickName": "三一一丫",
                                "want": ""
                            },
                            "targetUrl": "fleamarket://awesome_detail?id=789173665224&flutter=true&referPageArgs=iphone&gulSource=search&extra=%7B%22labelIds%22%3A%22752%2C9%22%2C%22source%22%3A%227%22%7D&referPage=Page_xySearchResult&trackParamsJson=%7B%22q%22%3A%22iphone%22%2C%22item_id%22%3A%22789173665224%22%2C%22item_type%22%3A%22goods%22%2C%22index%22%3A%228%22%2C%22page%22%3A%221%22%2C%22id%22%3A%22789173665224%22%2C%22rn%22%3A%227403a9b4d78f5a8665effe56a1b9c058%22%2C%22search_from_page%22%3A%22xyHome%22%2C%22search_id%22%3A%22a5507830d9f36fc69894e2684c958bc9%22%7D"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            },
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "picWidth": "164.0",
                                    "zhimaOffline": "false",
                                    "item_type": "goods",
                                    "disableHierarchicalSort": "0",
                                    "searchProjectLayerInfo": "DoubleShade_21|DEFAULT_26|202305152329_3090_1",
                                    "pageSize": "10",
                                    "type": "1",
                                    "q_type": "0",
                                    "search_from_page": "xyHome",
                                    "tagname": "包邮",
                                    "wantNum": "0",
                                    "id": "789365661990",
                                    "tag": "freeship",
                                    "keyword": "iphone",
                                    "scm": "1007.32845.290827.0",
                                    "seller_id": "2On+h3CAFRqEhPp8VOQEWA==",
                                    "publishTime": "1714280793000",
                                    "search_tab_from": "SEARCH_TAB_MAIN",
                                    "picHeight": "214.0",
                                    "cCatId": "126862528",
                                    "biz_type": "item",
                                    "tbCatId": "1512",
                                    "index": "7",
                                    "spm": "a2170.8011571.1.7",
                                    "catId": "50025386",
                                    "original_q": "iphone",
                                    "p_type": "2",
                                    "page": "1",
                                    "position": "7",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "tcDistance": "0.0",
                                    "abid": "290827",
                                    "singleControl": "false",
                                    "cpvNavWlTbCatId": "1512",
                                    "layerInfo": "22845#0#290827#5_22845#10269#446628#67_22845#12929#480547#54_22845#26994#481509#6_22845#12961#449492#47_22845#26899#481719#11_22845#25306#477353#13_22845#12936#453303#2_22845#12926#482457#52_22845#12928#482555#57",
                                    "item_id": "789365661990",
                                    "oldZhima": "false",
                                    "unShowLabelParams": "{}",
                                    "userIsUseFishShopCard": "false",
                                    "bucketid": "26",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": "a5507830d9f36fc69894e2684c958bc9",
                                    "idle_mount_tai_task_abs": "0:T:1;1192:T:0;768:T:0;793:T:0;130:T:0;343:T:0;467:T:0;573:T:0;1222:T:0;123:T:0;350:T:0;1209:C:0;212:T:0;505:T:0;1193:T:0;354:C:0;353:T:0;892:T:0;972:T:0;193:T:0;370:T:0;-4:C:1;340:T:0;359:T:0;363:T:0;536:T:0;169:T:0;788:T:0;487:T:0;199:T:0;223:T:0;792:T:0;598:T:0;1134:T:0;126:T:0;517:T:0;542:T:0;470:T:0;1229:C:0;356:T:0;593:T:0;-10:T:1;551:T:0;789:T:0;194:T:0;1210:C:0;592:T:0;543:T:0;225:T:0;552:T:0;500:T:0;226:T:0;366:T:0;933:T:0;337:T:0;1156:T:0;1173:T:0;558:T:0;341:T:0;1075:T:0;514:T:0;1190:T:0;244:T:0;893:T:0;969:T:0;227:T:0;1211:T:0;1142:T:0;1185:T:0;361:T:0;368:T:0;1228:C:0;766:T:0;1205:T:0;342:T:0;797:T:0;466:T:0;533:T:0",
                                    "q": "iphone",
                                    "CoinPay_Morediscount": "false",
                                    "isFromAISuggestion": "false",
                                    "tai_match_type": "0",
                                    "HideUserInfo": "false",
                                    "serviceUtParams": "[{\"arg1\":\"4_tag_r2_752\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"2小时前发布\"}},{\"arg1\":\"4_tag_r3_9\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"1人想要\"}},{\"arg1\":\"4_tag_r1_13\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"freeShippingIcon\"}}]",
                                    "labelBucketId": "9",
                                    "zhimaLogBucketId": "9"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "广东",
                                "detailParams": {
                                    "picWidth": "1242",
                                    "itemId": "789365661990",
                                    "itemType": "detailCommonBuy",
                                    "picHeight": "1621",
                                    "userNick": "xxxi",
                                    "soldPrice": "1399",
                                    "isVideo": "false",
                                    "title": "14plus 感兴趣的话点“我想要”和我私聊吧～"
                                },
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "789365661990",
                                            "bizType": "item",
                                            "picHeight": "214.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "9",
                                            "keyword": "iphone",
                                            "referPage": "Page_xySearchResult_FindSimilar"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "itemPicUrl": "http://img.alicdn.com/bao/uploaded/i4/O1CN018q46XX2HkA0N352sI_!!0-fleamarket.jpg",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "2On+h3CAFRqEhPp8VOQEWA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789365661990",
                                                "targetIndex": "9",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "789365661990",
                                                    "bizType": "item",
                                                    "picHeight": "214.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "9",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "2On+h3CAFRqEhPp8VOQEWA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789365661990",
                                                "targetIndex": "9",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "789365661990",
                                                    "bizType": "item",
                                                    "picHeight": "214.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "9",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "2On+h3CAFRqEhPp8VOQEWA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789365661990",
                                                "targetIndex": "9",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "789365661990",
                                                    "bizType": "item",
                                                    "picHeight": "214.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "9",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "2On+h3CAFRqEhPp8VOQEWA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789365661990",
                                                "targetIndex": "9",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "789365661990",
                                                    "bizType": "item",
                                                    "picHeight": "214.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "9",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "2On+h3CAFRqEhPp8VOQEWA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789365661990",
                                                "targetIndex": "9",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "789365661990",
                                                    "bizType": "item",
                                                    "picHeight": "214.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "9",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01nEHAUr1bTw528ELSv_!!6000000003467-2-tps-96-96.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "2On+h3CAFRqEhPp8VOQEWA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789365661990",
                                                "targetIndex": "9",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "789365661990",
                                                    "bizType": "item",
                                                    "picHeight": "214.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "9",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i4/O1CN01d2x4An1z5FVcHazR1_!!6000000006662-2-tps-96-96.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "2On+h3CAFRqEhPp8VOQEWA==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789365661990",
                                                "targetIndex": "9",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "789365661990",
                                                    "bizType": "item",
                                                    "picHeight": "214.0",
                                                    "picWicth": "164.0",
                                                    "name": "结果不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "9",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01XMrXCG1W2OB7JmJIY_!!6000000002730-2-tps-96-96.png",
                                            "index": "3",
                                            "text": "结果不相关"
                                        }
                                    ],
                                    "similarTargetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-photo-search/pages/home?kun=true&wh_ttid=native&opaque=false&extra=%7B%22imageInfo%22%3A%7B%22bizCode%22%3A%22graph_similarity%22%2C%22reqFromPage%22%3A%22main_search_feeds_dislike%22%2C%22source%22%3A%22itemPic%22%2C%22url%22%3A%22http%3A%2F%2Fimg.alicdn.com%2Fbao%2Fuploaded%2Fi4%2FO1CN018q46XX2HkA0N352sI_%21%210-fleamarket.jpg_640x640q90.jpg%22%7D%7D",
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTagCustomParam": {
                                    "feedStyle202208": "1",
                                    "feedStyle202304": "1"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "gradientColors": [
                                                        "#F7F7CC",
                                                        "#FFFFFF"
                                                    ],
                                                    "color": "#48483B",
                                                    "borderRadius": "9",
                                                    "size": "12",
                                                    "labelId": "752",
                                                    "lineHeight": "1.2",
                                                    "gradientDirection": "to right",
                                                    "gradientType": "linear",
                                                    "type": "gradientImageText",
                                                    "content": "2小时前发布",
                                                    "height": "16",
                                                    "leftImage": {
                                                        "marginRight": "2",
                                                        "width": "14",
                                                        "url": "https://gw.alicdn.com/imgextra/i3/O1CN01Z6BeDa1w4qA2xZLFJ_!!6000000006255-2-tps-42-42.png",
                                                        "height": "14",
                                                        "marginLeft": "2"
                                                    }
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "2小时前发布"
                                                    },
                                                    "arg1": "4_tag_r2_752"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "true"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "9",
                                                    "lineHeight": "1.3",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "1人想要",
                                                    "marginLeft": "4"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "1人想要"
                                                    },
                                                    "arg1": "4_tag_r3_9"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r1": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "marginRight": "4",
                                                    "labelId": "13",
                                                    "width": "28",
                                                    "type": "img",
                                                    "alignment": "middle",
                                                    "content": "freeShippingIcon",
                                                    "url": "https://gw.alicdn.com/imgextra/i3/O1CN01PuymOm1I7yIlVyFV9_!!6000000000847-2-tps-84-48.png",
                                                    "height": "16"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "freeShippingIcon"
                                                    },
                                                    "arg1": "4_tag_r1_13"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "false",
                                "isAuction": "false",
                                "itemId": "789365661990",
                                "jump2XianYuHao": {
                                    "clickParam": {
                                        "arg1": "Jump2User",
                                        "args": {
                                            "bucket_id": "26",
                                            "spm": "a2170.8011571.Jump2User.9",
                                            "user_id": "9VqNOYOLgTeQTHkg/H/fnQ==",
                                            "item_id": "789365661990",
                                            "userIsUseFishShopCard": "false",
                                            "HideUserInfo": "false",
                                            "seller_id": "2On+h3CAFRqEhPp8VOQEWA=="
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "targetUrl": "z9xpXnwzz6eu3JHQFPK2nb4PAGLvMlrcMmttP6latEqMz/uXT1vwj+Q09oJCnGdei+Ym+8CxGeCxfex+A0gH6AC9YKtonEzxvVz2EAlFgsg="
                                },
                                "picHeight": "214.0450885668277",
                                "picUrl": "http://img.alicdn.com/bao/uploaded/i4/O1CN018q46XX2HkA0N352sI_!!0-fleamarket.jpg",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1399",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [],
                                "richTitle": [
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1eCD602b2gK0jSZK9XXaEgFXa-84-48.png",
                                            "width": "35.0"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "14plus 感兴趣的话点“我想要”和我私聊吧～",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "stuffStatusTagHeight": "0.0",
                                "stuffStatusTagWidth": "0.0",
                                "title": "14plus 感兴趣的话点“我想要”和我私聊吧～",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "14plus 感兴趣的话点“我想要”和我私聊吧～",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userActiveUrl": "https://gw.alicdn.com/tfs/TB1zIymVUz1gK0jSZLeXXb9kVXa-30-30.png",
                                "userAvatarUrl": "http://img.alicdn.com/bao/uploaded/i1/O1CN01Lf1kHx2HkA0CyPK8C_!!0-mtopupload.jpg",
                                "userFishShopLabel": {
                                    "config": {
                                        "delimiterColor": "#D6D6D6",
                                        "delimiterHeight": "12",
                                        "delimiterMarginLeft": "4.5",
                                        "delimiterMarginRight": "4.5",
                                        "delimiterPosition": "between",
                                        "delimiterWidth": "0.5",
                                        "hasDelimiter": "true",
                                        "mutualLabelBizGroup": "true"
                                    },
                                    "tagList": [
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "0条评价",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        },
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "好评率0%",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        }
                                    ]
                                },
                                "userIdentityShow": "",
                                "userIsUseFishShopCard": "false",
                                "userNickName": "xxxi",
                                "want": ""
                            },
                            "targetUrl": "fleamarket://awesome_detail?id=789365661990&flutter=true&referPageArgs=iphone&gulSource=search&extra=%7B%22labelIds%22%3A%22752%2C9%2C13%22%2C%22source%22%3A%227%22%7D&referPage=Page_xySearchResult&trackParamsJson=%7B%22q%22%3A%22iphone%22%2C%22item_id%22%3A%22789365661990%22%2C%22item_type%22%3A%22goods%22%2C%22index%22%3A%229%22%2C%22page%22%3A%221%22%2C%22id%22%3A%22789365661990%22%2C%22rn%22%3A%227403a9b4d78f5a8665effe56a1b9c058%22%2C%22search_from_page%22%3A%22xyHome%22%2C%22search_id%22%3A%22a5507830d9f36fc69894e2684c958bc9%22%7D"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            },
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "picWidth": "164.0",
                                    "zhimaOffline": "false",
                                    "item_type": "goods",
                                    "disableHierarchicalSort": "0",
                                    "searchProjectLayerInfo": "DoubleShade_21|DEFAULT_26|202305152329_3090_1",
                                    "pageSize": "10",
                                    "type": "1",
                                    "q_type": "0",
                                    "search_from_page": "xyHome",
                                    "wantNum": "0",
                                    "id": "782639796439",
                                    "keyword": "iphone",
                                    "scm": "1007.32845.290827.0",
                                    "seller_id": "zvE2/UpTi78mU48aJoJfww==",
                                    "publishTime": "1712782963000",
                                    "search_tab_from": "SEARCH_TAB_MAIN",
                                    "picHeight": "218.0",
                                    "cCatId": "126862528",
                                    "biz_type": "item",
                                    "tbCatId": "1512",
                                    "index": "8",
                                    "spm": "a2170.8011571.1.8",
                                    "catId": "50025386",
                                    "original_q": "iphone",
                                    "p_type": "2",
                                    "page": "1",
                                    "position": "8",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "tcDistance": "0.0",
                                    "abid": "290827",
                                    "singleControl": "false",
                                    "cpvNavWlTbCatId": "1512",
                                    "layerInfo": "22845#0#290827#5_22845#10269#446628#67_22845#12929#480547#54_22845#26994#481509#6_22845#12961#449492#47_22845#26899#481719#11_22845#25306#477353#13_22845#12936#453303#2_22845#12926#482457#52_22845#12928#482555#57",
                                    "item_id": "782639796439",
                                    "oldZhima": "false",
                                    "unShowLabelParams": "{}",
                                    "userIsUseFishShopCard": "false",
                                    "bucketid": "26",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": "a5507830d9f36fc69894e2684c958bc9",
                                    "idle_mount_tai_task_abs": "0:T:1;1192:T:0;768:T:0;793:T:0;130:T:0;343:T:0;467:T:0;1222:T:1;573:T:0;123:T:0;350:T:0;1209:C:0;212:T:0;505:T:0;1193:T:0;354:C:0;353:T:0;892:T:0;972:T:0;193:T:0;370:T:0;-4:C:1;340:T:0;359:T:0;363:T:0;536:T:0;169:T:0;788:T:0;487:T:0;199:T:0;223:T:0;792:T:0;598:T:0;1134:T:0;126:T:0;517:T:0;542:T:0;470:T:0;1229:C:0;356:T:0;593:T:0;-10:T:1;551:T:0;789:T:0;194:T:0;1210:C:0;592:T:0;543:T:0;225:T:0;552:T:0;500:T:0;226:T:0;366:T:0;933:T:0;337:T:0;1156:T:0;1173:T:0;558:T:0;341:T:0;1075:T:0;514:T:0;1190:T:0;244:T:0;893:T:0;969:T:0;227:T:0;1211:T:0;1142:T:0;1185:T:0;361:T:0;368:T:0;1228:C:0;766:T:0;1205:T:0;342:T:0;797:T:0;466:T:0;533:T:0",
                                    "q": "iphone",
                                    "CoinPay_Morediscount": "false",
                                    "isFromAISuggestion": "false",
                                    "tai_match_type": "14",
                                    "HideUserInfo": "false",
                                    "serviceUtParams": "[{\"arg1\":\"4_tag_r2_36\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"几乎全新\"}},{\"arg1\":\"4_tag_r2_38\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"Apple/苹果\"}},{\"arg1\":\"4_tag_r2_34\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"128GB\"}},{\"arg1\":\"4_tag_r3_9\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"46人想要\"}},{\"arg1\":\"4_tag_r4_750\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"百分百好评\"}}]",
                                    "labelBucketId": "9",
                                    "zhimaLogBucketId": "9"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "广东",
                                "detailParams": {
                                    "picWidth": "1080",
                                    "itemId": "782639796439",
                                    "itemType": "detailCommonBuy",
                                    "picHeight": "1440",
                                    "userNick": "小冰冰金刚",
                                    "soldPrice": "1000",
                                    "isVideo": "false",
                                    "title": "苹果 15 128蓝 国行双卡99新 电池效率99  100 0出 #苹果 #苹果手表"
                                },
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "782639796439",
                                            "bizType": "item",
                                            "picHeight": "218.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "10",
                                            "keyword": "iphone",
                                            "referPage": "Page_xySearchResult_FindSimilar"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "itemPicUrl": "http://img.alicdn.com/bao/uploaded/i1/O1CN01ykBdH320PgpSWHogv_!!53-fleamarket.heic",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "zvE2/UpTi78mU48aJoJfww==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "782639796439",
                                                "targetIndex": "10",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "782639796439",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "10",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "zvE2/UpTi78mU48aJoJfww==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "782639796439",
                                                "targetIndex": "10",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "782639796439",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "10",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "zvE2/UpTi78mU48aJoJfww==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "782639796439",
                                                "targetIndex": "10",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "782639796439",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "10",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "zvE2/UpTi78mU48aJoJfww==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "782639796439",
                                                "targetIndex": "10",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "782639796439",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "10",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "zvE2/UpTi78mU48aJoJfww==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "782639796439",
                                                "targetIndex": "10",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "782639796439",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "10",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01nEHAUr1bTw528ELSv_!!6000000003467-2-tps-96-96.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "zvE2/UpTi78mU48aJoJfww==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "782639796439",
                                                "targetIndex": "10",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "782639796439",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "10",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i4/O1CN01d2x4An1z5FVcHazR1_!!6000000006662-2-tps-96-96.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "zvE2/UpTi78mU48aJoJfww==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "782639796439",
                                                "targetIndex": "10",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "782639796439",
                                                    "bizType": "item",
                                                    "picHeight": "218.0",
                                                    "picWicth": "164.0",
                                                    "name": "结果不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "10",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01XMrXCG1W2OB7JmJIY_!!6000000002730-2-tps-96-96.png",
                                            "index": "3",
                                            "text": "结果不相关"
                                        }
                                    ],
                                    "similarTargetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-photo-search/pages/home?kun=true&wh_ttid=native&opaque=false&extra=%7B%22imageInfo%22%3A%7B%22bizCode%22%3A%22graph_similarity%22%2C%22reqFromPage%22%3A%22main_search_feeds_dislike%22%2C%22source%22%3A%22itemPic%22%2C%22url%22%3A%22http%3A%2F%2Fimg.alicdn.com%2Fbao%2Fuploaded%2Fi1%2FO1CN01ykBdH320PgpSWHogv_%21%2153-fleamarket.heic_640x640q90.jpg%22%7D%7D",
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTagCustomParam": {
                                    "feedStyle202208": "1",
                                    "feedStyle202304": "1"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "36",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "几乎全新"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "几乎全新"
                                                    },
                                                    "arg1": "4_tag_r2_36"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "38",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "Apple/苹果"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "Apple/苹果"
                                                    },
                                                    "arg1": "4_tag_r2_38"
                                                }
                                            },
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "34",
                                                    "lineHeight": "1.33",
                                                    "bold": "false",
                                                    "type": "gradientImageText",
                                                    "content": "128GB"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "128GB"
                                                    },
                                                    "arg1": "4_tag_r2_34"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "delimiterMarginRight": "4.5",
                                            "delimiterWidth": "0.5",
                                            "delimiterPosition": "between",
                                            "delimiterColor": "#D6D6D6",
                                            "delimiterHeight": "10",
                                            "hasDelimiter": "true",
                                            "delimiterMarginLeft": "4.5",
                                            "delimiterMarginBottom": "3",
                                            "mutualLabelBizGroup": "true",
                                            "delimiterMarginTop": "3"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "9",
                                                    "lineHeight": "1.3",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "46人想要",
                                                    "marginLeft": "4"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "46人想要"
                                                    },
                                                    "arg1": "4_tag_r3_9"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r4": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "bgColor": "#FFF4EB",
                                                    "color": "#FF7900",
                                                    "borderRadius": "8",
                                                    "size": "11",
                                                    "labelId": "750",
                                                    "borderPaddingLeft": "6",
                                                    "lineHeight": "1.3",
                                                    "borderPaddingRight": "6",
                                                    "type": "gradientImageText",
                                                    "content": "百分百好评",
                                                    "height": "16"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "百分百好评"
                                                    },
                                                    "arg1": "4_tag_r4_750"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "false",
                                "isAuction": "false",
                                "itemId": "782639796439",
                                "jump2XianYuHao": {
                                    "clickParam": {
                                        "arg1": "Jump2User",
                                        "args": {
                                            "bucket_id": "26",
                                            "spm": "a2170.8011571.Jump2User.10",
                                            "user_id": "9VqNOYOLgTeQTHkg/H/fnQ==",
                                            "item_id": "782639796439",
                                            "userIsUseFishShopCard": "false",
                                            "HideUserInfo": "false",
                                            "seller_id": "zvE2/UpTi78mU48aJoJfww=="
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "targetUrl": "z9xpXnwzz6eu3JHQFPK2nb4PAGLvMlrcMmttP6latErSJX3F6+aN0j4/47nlKmEA+jswFpxxzmGTZMvIwCluV5TqzjBQEkZnqdcG48zHQ4o="
                                },
                                "picHeight": "218.66666666666666",
                                "picUrl": "http://img.alicdn.com/bao/uploaded/i1/O1CN01ykBdH320PgpSWHogv_!!53-fleamarket.heic",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1000",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [],
                                "richTitle": [
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "苹果 15 128蓝 国行双卡99新 电池效率99  100 0出 #苹果 #苹果手表",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "stuffStatusTagHeight": "0.0",
                                "stuffStatusTagWidth": "0.0",
                                "title": "苹果 15 128蓝 国行双卡99新 电池效率99  100 0出 #苹果 #苹果手表",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "苹果 15 128蓝 国行双卡99新 电池效率99  100 0出 #苹果 #苹果手表",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userAvatarUrl": "http://img.alicdn.com/bao/uploaded/i1/O1CN01STCcql20PgpLFP6Yu_!!0-mtopupload.jpg",
                                "userFishShopLabel": {
                                    "config": {
                                        "delimiterColor": "#D6D6D6",
                                        "delimiterHeight": "12",
                                        "delimiterMarginLeft": "4.5",
                                        "delimiterMarginRight": "4.5",
                                        "delimiterPosition": "between",
                                        "delimiterWidth": "0.5",
                                        "hasDelimiter": "true",
                                        "mutualLabelBizGroup": "true"
                                    },
                                    "tagList": [
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "45条评价",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        },
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "好评率100%",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        }
                                    ]
                                },
                                "userIdentityShow": "",
                                "userIsUseFishShopCard": "false",
                                "userNickName": "小冰冰金刚",
                                "want": ""
                            },
                            "targetUrl": "fleamarket://awesome_detail?id=782639796439&flutter=true&referPageArgs=iphone&gulSource=search&extra=%7B%22labelIds%22%3A%2236%2C38%2C34%2C9%2C750%22%2C%22source%22%3A%227%22%7D&referPage=Page_xySearchResult&trackParamsJson=%7B%22q%22%3A%22iphone%22%2C%22item_id%22%3A%22782639796439%22%2C%22item_type%22%3A%22goods%22%2C%22index%22%3A%2210%22%2C%22page%22%3A%221%22%2C%22id%22%3A%22782639796439%22%2C%22rn%22%3A%227403a9b4d78f5a8665effe56a1b9c058%22%2C%22search_from_page%22%3A%22xyHome%22%2C%22search_id%22%3A%22a5507830d9f36fc69894e2684c958bc9%22%7D"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            },
            {
                "data": {
                    "item": {
                        "main": {
                            "clickParam": {
                                "arg1": "Item",
                                "args": {
                                    "picWidth": "164.0",
                                    "zhimaOffline": "false",
                                    "item_type": "goods",
                                    "disableHierarchicalSort": "0",
                                    "searchProjectLayerInfo": "DoubleShade_21|DEFAULT_26|202305152329_3090_1",
                                    "pageSize": "10",
                                    "type": "1",
                                    "q_type": "0",
                                    "search_from_page": "xyHome",
                                    "tagname": "全新/包邮",
                                    "wantNum": "0",
                                    "id": "789366572728",
                                    "tag": "new/freeship",
                                    "keyword": "iphone",
                                    "scm": "1007.32845.290827.0",
                                    "seller_id": "65ZweWDmuZHbk5LmTgxnfg==",
                                    "publishTime": "1714280903000",
                                    "search_tab_from": "SEARCH_TAB_MAIN",
                                    "picHeight": "164.0",
                                    "cCatId": "126862528",
                                    "biz_type": "item",
                                    "tbCatId": "1512",
                                    "index": "9",
                                    "spm": "a2170.8011571.1.9",
                                    "catId": "50025386",
                                    "original_q": "iphone",
                                    "p_type": "2",
                                    "page": "1",
                                    "position": "9",
                                    "rn": "7403a9b4d78f5a8665effe56a1b9c058",
                                    "tcDistance": "0.0",
                                    "abid": "290827",
                                    "singleControl": "false",
                                    "cpvNavWlTbCatId": "1512",
                                    "layerInfo": "22845#0#290827#5_22845#10269#446628#67_22845#12929#480547#54_22845#26994#481509#6_22845#12961#449492#47_22845#26899#481719#11_22845#25306#477353#13_22845#12936#453303#2_22845#12926#482457#52_22845#12928#482555#57",
                                    "item_id": "789366572728",
                                    "oldZhima": "false",
                                    "unShowLabelParams": "{}",
                                    "userIsUseFishShopCard": "false",
                                    "bucketid": "26",
                                    "card_type": "idlefish_search_item_new_tags",
                                    "search_id": "a5507830d9f36fc69894e2684c958bc9",
                                    "idle_mount_tai_task_abs": "0:T:1;1192:T:0;768:T:0;793:T:0;130:T:0;343:T:0;467:T:0;573:T:0;1222:T:0;123:T:0;350:T:0;1209:C:0;212:T:0;505:T:0;1193:T:0;354:C:0;353:T:0;892:T:0;972:T:0;193:T:0;370:T:0;-4:C:1;340:T:0;359:T:0;363:T:0;536:T:0;169:T:0;788:T:0;487:T:0;199:T:0;223:T:0;792:T:0;598:T:0;1134:T:0;126:T:0;517:T:0;542:T:0;470:T:0;1229:C:0;356:T:0;593:T:0;-10:T:1;551:T:0;789:T:0;194:T:0;1210:C:0;592:T:0;543:T:0;225:T:0;552:T:0;500:T:0;226:T:0;366:T:0;933:T:0;337:T:0;1156:T:0;1173:T:0;558:T:0;341:T:0;1075:T:0;514:T:0;1190:T:0;244:T:0;893:T:0;969:T:0;227:T:0;1211:T:0;1142:T:0;1185:T:0;361:T:0;368:T:0;1228:C:0;766:T:0;1205:T:0;342:T:0;797:T:0;466:T:0;533:T:0",
                                    "q": "iphone",
                                    "CoinPay_Morediscount": "false",
                                    "isFromAISuggestion": "false",
                                    "tai_match_type": "0",
                                    "HideUserInfo": "false",
                                    "serviceUtParams": "[{\"arg1\":\"4_tag_r2_752\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"2小时前发布\"}},{\"arg1\":\"4_tag_r3_9\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"5人想要\"}},{\"arg1\":\"4_tag_r4_750\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"发货极快\"}},{\"arg1\":\"4_tag_r1_472\",\"args\":{\"LabelSystem2.0\":\"1\",\"content\":\"验货宝\"}}]",
                                    "labelBucketId": "9",
                                    "zhimaLogBucketId": "9"
                                },
                                "page": "Page_xySearchResult"
                            },
                            "exContent": {
                                "area": "广东",
                                "detailParams": {
                                    "picWidth": "1080",
                                    "itemId": "789366572728",
                                    "itemType": "detailCommonBuy",
                                    "picHeight": "1080",
                                    "userNick": "黑猫鲸长",
                                    "soldPrice": "1006",
                                    "isVideo": "false",
                                    "title": "女生自用闲置苹果iPhone 14pro灵动岛银白色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！"
                                },
                                "dislikeFeedback": {
                                    "clickParam": {
                                        "arg1": "DisLikePanel",
                                        "args": {
                                            "itemId": "789366572728",
                                            "bizType": "item",
                                            "picHeight": "164.0",
                                            "picWicth": "164.0",
                                            "itemPosition": "11",
                                            "keyword": "iphone",
                                            "referPage": "Page_xySearchResult_FindSimilar"
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "dislikeStyle": "dislikeStyle202304",
                                    "itemPicUrl": "http://img.alicdn.com/bao/uploaded/i2/O1CN01J1KjEA1x9iAYGyP0a_!!0-fleamarket.jpg",
                                    "moreList": [
                                        {
                                            "apiParams": {
                                                "actType": "fakePrice",
                                                "extra": "65ZweWDmuZHbk5LmTgxnfg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789366572728",
                                                "targetIndex": "11",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.1",
                                                    "itemId": "789366572728",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "虚假价格",
                                                    "index": "1",
                                                    "actType": "fakePrice",
                                                    "itemPosition": "11",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i4/O1CN01AeEtqS1cxXCmlX2IC_!!6000000003667-2-tps-64-64.png",
                                            "index": "1",
                                            "text": "虚假价格"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeImage",
                                                "extra": "65ZweWDmuZHbk5LmTgxnfg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789366572728",
                                                "targetIndex": "11",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.2",
                                                    "itemId": "789366572728",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "引起不适",
                                                    "index": "2",
                                                    "actType": "dislikeImage",
                                                    "itemPosition": "11",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01o871mh1p61wNfFLOb_!!6000000005310-2-tps-64-64.png",
                                            "index": "2",
                                            "text": "引起不适"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "fakeItem",
                                                "extra": "65ZweWDmuZHbk5LmTgxnfg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789366572728",
                                                "targetIndex": "11",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.3",
                                                    "itemId": "789366572728",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "疑似假货",
                                                    "index": "3",
                                                    "actType": "fakeItem",
                                                    "itemPosition": "11",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i1/O1CN01bSL1jD1GvJk2haDqH_!!6000000000684-2-tps-64-64.png",
                                            "index": "3",
                                            "text": "疑似假货"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "alreadyBuy",
                                                "extra": "65ZweWDmuZHbk5LmTgxnfg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789366572728",
                                                "targetIndex": "11",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemMore",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemMore.4",
                                                    "itemId": "789366572728",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "已经买过",
                                                    "index": "4",
                                                    "actType": "alreadyBuy",
                                                    "itemPosition": "11",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://img.alicdn.com/imgextra/i3/O1CN01ahXcOL1b152UnCUr1_!!6000000003404-2-tps-64-64.png",
                                            "index": "4",
                                            "text": "已经买过"
                                        }
                                    ],
                                    "showList": [
                                        {
                                            "apiParams": {
                                                "actType": "dislikeGoods",
                                                "extra": "65ZweWDmuZHbk5LmTgxnfg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789366572728",
                                                "targetIndex": "11",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.1",
                                                    "itemId": "789366572728",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该商品",
                                                    "index": "1",
                                                    "actType": "dislikeGoods",
                                                    "itemPosition": "11",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01nEHAUr1bTw528ELSv_!!6000000003467-2-tps-96-96.png",
                                            "index": "1",
                                            "text": "不喜欢该商品"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "dislikeAuthor",
                                                "extra": "65ZweWDmuZHbk5LmTgxnfg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789366572728",
                                                "targetIndex": "11",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.2",
                                                    "itemId": "789366572728",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "不喜欢该卖家",
                                                    "index": "2",
                                                    "actType": "dislikeAuthor",
                                                    "itemPosition": "11",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i4/O1CN01d2x4An1z5FVcHazR1_!!6000000006662-2-tps-96-96.png",
                                            "index": "2",
                                            "text": "不喜欢该卖家"
                                        },
                                        {
                                            "apiParams": {
                                                "actType": "queryUnrelated",
                                                "extra": "65ZweWDmuZHbk5LmTgxnfg==",
                                                "queryWord": "iphone",
                                                "scene": "Page_xySearchResult",
                                                "targetId": "789366572728",
                                                "targetIndex": "11",
                                                "targetType": "item"
                                            },
                                            "clickParam": {
                                                "arg1": "DisLikeItemFirst",
                                                "args": {
                                                    "spm": "a2170.8011571.DisLikeItemFirst.3",
                                                    "itemId": "789366572728",
                                                    "bizType": "item",
                                                    "picHeight": "164.0",
                                                    "picWicth": "164.0",
                                                    "name": "结果不相关",
                                                    "index": "3",
                                                    "actType": "queryUnrelated",
                                                    "itemPosition": "11",
                                                    "keyword": "iphone"
                                                },
                                                "page": "Page_xySearchResult"
                                            },
                                            "icon": "https://gw.alicdn.com/imgextra/i2/O1CN01XMrXCG1W2OB7JmJIY_!!6000000002730-2-tps-96-96.png",
                                            "index": "3",
                                            "text": "结果不相关"
                                        }
                                    ],
                                    "similarTargetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-photo-search/pages/home?kun=true&wh_ttid=native&opaque=false&extra=%7B%22imageInfo%22%3A%7B%22bizCode%22%3A%22graph_similarity%22%2C%22reqFromPage%22%3A%22main_search_feeds_dislike%22%2C%22source%22%3A%22itemPic%22%2C%22url%22%3A%22http%3A%2F%2Fimg.alicdn.com%2Fbao%2Fuploaded%2Fi2%2FO1CN01J1KjEA1x9iAYGyP0a_%21%210-fleamarket.jpg_640x640q90.jpg%22%7D%7D",
                                    "targetUrl": "https://h5.m.goofish.com/wow/moyu/moyu-project/idle-negative-feedback-layer/pages/home-71050?kun=true&opaque=false&loadingVisible=false&wh_ttid=native&__kun_load_policy=nc_ac"
                                },
                                "fishTagCustomParam": {
                                    "feedStyle202208": "1",
                                    "feedStyle202304": "1"
                                },
                                "fishTags": {
                                    "r2": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "gradientColors": [
                                                        "#F7F7CC",
                                                        "#FFFFFF"
                                                    ],
                                                    "color": "#48483B",
                                                    "borderRadius": "9",
                                                    "size": "12",
                                                    "labelId": "752",
                                                    "lineHeight": "1.2",
                                                    "gradientDirection": "to right",
                                                    "gradientType": "linear",
                                                    "type": "gradientImageText",
                                                    "content": "2小时前发布",
                                                    "height": "16",
                                                    "leftImage": {
                                                        "marginRight": "2",
                                                        "width": "14",
                                                        "url": "https://gw.alicdn.com/imgextra/i3/O1CN01Z6BeDa1w4qA2xZLFJ_!!6000000006255-2-tps-42-42.png",
                                                        "height": "14",
                                                        "marginLeft": "2"
                                                    }
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "2小时前发布"
                                                    },
                                                    "arg1": "4_tag_r2_752"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "true"
                                        }
                                    },
                                    "r3": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "color": "#999999",
                                                    "size": "12",
                                                    "labelId": "9",
                                                    "lineHeight": "1.3",
                                                    "bold": "false",
                                                    "type": "text",
                                                    "content": "5人想要",
                                                    "marginLeft": "4"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "5人想要"
                                                    },
                                                    "arg1": "4_tag_r3_9"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r4": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "bgColor": "#FFF4EB",
                                                    "color": "#FF7900",
                                                    "borderRadius": "8",
                                                    "size": "11",
                                                    "labelId": "750",
                                                    "borderPaddingLeft": "6",
                                                    "lineHeight": "1.3",
                                                    "borderPaddingRight": "6",
                                                    "type": "gradientImageText",
                                                    "content": "发货极快",
                                                    "height": "16"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "发货极快"
                                                    },
                                                    "arg1": "4_tag_r4_750"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    },
                                    "r1": {
                                        "tagList": [
                                            {
                                                "data": {
                                                    "marginRight": "4",
                                                    "labelId": "472",
                                                    "width": "41",
                                                    "type": "img",
                                                    "alignment": "middle",
                                                    "content": "验货宝",
                                                    "url": "https://gw.alicdn.com/imgextra/i3/O1CN01gVzTNw1nMrFzcRUFt_!!6000000005076-2-tps-123-48.png",
                                                    "height": "16"
                                                },
                                                "utParams": {
                                                    "args": {
                                                        "LabelSystem2.0": "1",
                                                        "content": "验货宝"
                                                    },
                                                    "arg1": "4_tag_r1_472"
                                                }
                                            }
                                        ],
                                        "config": {
                                            "mutualLabelBizGroup": "false"
                                        }
                                    }
                                },
                                "hideUserInfo": "false",
                                "isAliMaMaAD": "false",
                                "isAuction": "false",
                                "itemId": "789366572728",
                                "jump2XianYuHao": {
                                    "clickParam": {
                                        "arg1": "Jump2User",
                                        "args": {
                                            "bucket_id": "26",
                                            "spm": "a2170.8011571.Jump2User.11",
                                            "user_id": "9VqNOYOLgTeQTHkg/H/fnQ==",
                                            "item_id": "789366572728",
                                            "userIsUseFishShopCard": "false",
                                            "HideUserInfo": "false",
                                            "seller_id": "65ZweWDmuZHbk5LmTgxnfg=="
                                        },
                                        "page": "Page_xySearchResult"
                                    },
                                    "targetUrl": "z9xpXnwzz6eu3JHQFPK2nb4PAGLvMlrcMmttP6latEoQotW4yStYWJDVZWtAfh4IZU8T5ZVP6ArKlLpg6Cgnek5eJGFBBPxz0j+ZlxQBa9o="
                                },
                                "picHeight": "164.0",
                                "picUrl": "http://img.alicdn.com/bao/uploaded/i2/O1CN01J1KjEA1x9iAYGyP0a_!!0-fleamarket.jpg",
                                "picWidth": "164.0",
                                "placeholderColor": "#F7F7F7",
                                "price": [
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "4.5",
                                        "marginLeft": "0.0",
                                        "text": "¥",
                                        "textColor": "#ff4400",
                                        "textSize": "11.0"
                                    },
                                    {
                                        "bold": "false",
                                        "fontFamily": "xianyubeta",
                                        "marginBottom": "3.0",
                                        "marginLeft": "0.0",
                                        "text": "1006",
                                        "textColor": "#ff4444",
                                        "textSize": "18.0"
                                    }
                                ],
                                "priceTag": [],
                                "richTitle": [
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1nTuTp0Tfau8jSZFwXXX1mVXa-114-48.png",
                                            "width": "47.5"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "alignment": "middle",
                                            "height": "20.0",
                                            "marginBottom": "0.0",
                                            "marginLeft": "0.0",
                                            "marginRight": "4.0",
                                            "marginTop": "0.0",
                                            "url": "https://gw.alicdn.com/tfs/TB1eCD602b2gK0jSZK9XXaEgFXa-84-48.png",
                                            "width": "35.0"
                                        },
                                        "type": "Image"
                                    },
                                    {
                                        "data": {
                                            "bold": "false",
                                            "fontWeight": "w400",
                                            "lineHeight": "1.43",
                                            "text": "女生自用闲置苹果iPhone 14pro灵动岛银白色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                            "textColor": "#1F1F1F",
                                            "textSize": "14.0"
                                        },
                                        "type": "Text"
                                    }
                                ],
                                "showVideoIcon": "false",
                                "stuffStatusTagHeight": "0.0",
                                "stuffStatusTagWidth": "0.0",
                                "title": "女生自用闲置苹果iPhone 14pro灵动岛银白色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                "titleSpan": {
                                    "bold": "false",
                                    "color": "#1F1F1F",
                                    "content": "女生自用闲置苹果iPhone 14pro灵动岛银白色国行   512G  成色全新    全网通 ，双卡双待    纯原装，无拆无修，没有磕碰，没有暗病，手机所有功能都正常的使用，面容好用。七天无理由退换货，全国联保一年！",
                                    "fontWeight": "w400",
                                    "lineHeight": "1.43",
                                    "maxLines": "2",
                                    "size": "14.0"
                                },
                                "userActiveUrl": "https://gw.alicdn.com/tfs/TB1zIymVUz1gK0jSZLeXXb9kVXa-30-30.png",
                                "userAvatarUrl": "http://img.alicdn.com/bao/uploaded/i2/164010154071743492/TB23pU6iFXXXXcXXXXXXXXXXXXX_!!0-mytaobao.jpg",
                                "userFishShopLabel": {
                                    "config": {
                                        "delimiterColor": "#D6D6D6",
                                        "delimiterHeight": "12",
                                        "delimiterMarginLeft": "4.5",
                                        "delimiterMarginRight": "4.5",
                                        "delimiterPosition": "between",
                                        "delimiterWidth": "0.5",
                                        "hasDelimiter": "true",
                                        "mutualLabelBizGroup": "true"
                                    },
                                    "tagList": [
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "0条评价",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        },
                                        {
                                            "data": {
                                                "color": "#999999",
                                                "content": "好评率0%",
                                                "lineHeight": "1.33",
                                                "size": "10",
                                                "type": "gradientImageText"
                                            }
                                        }
                                    ]
                                },
                                "userIdentityShow": "",
                                "userIsUseFishShopCard": "false",
                                "userNickName": "黑猫鲸长",
                                "want": ""
                            },
                            "targetUrl": "fleamarket://awesome_detail?id=789366572728&flutter=true&referPageArgs=iphone&gulSource=search&extra=%7B%22labelIds%22%3A%22752%2C9%2C750%2C472%22%2C%22source%22%3A%227%22%7D&referPage=Page_xySearchResult&trackParamsJson=%7B%22q%22%3A%22iphone%22%2C%22item_id%22%3A%22789366572728%22%2C%22item_type%22%3A%22goods%22%2C%22index%22%3A%2211%22%2C%22page%22%3A%221%22%2C%22id%22%3A%22789366572728%22%2C%22rn%22%3A%227403a9b4d78f5a8665effe56a1b9c058%22%2C%22search_from_page%22%3A%22xyHome%22%2C%22search_id%22%3A%22a5507830d9f36fc69894e2684c958bc9%22%7D"
                        }
                    },
                    "template": {
                        "name": "idlefish_search_item_new_tags",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_new_tags/1712647656006/idlefish_search_item_new_tags.zip",
                        "version": "1712647656006"
                    },
                    "templateSingle": {
                        "name": "idlefish_search_item_single_column",
                        "url": "https://dinamicx.alibabausercontent.com/pub/idlefish_search_item_single_column/1704445459595/idlefish_search_item_single_column.zip",
                        "version": "1704445459595"
                    }
                },
                "style": "flow",
                "type": "DX"
            }
        ],
        "resultPrefixBar": [],
        "tabList": [
            {
                "apiName": "mtop.taobao.idlemtopsearch.search",
                "apiVersion": "1.0",
                "searchTabType": "SEARCH_TAB_MAIN",
                "showName": "全部"
            },
            {
                "apiName": "mtop.taobao.idlemtopsearch.market.tab.list",
                "apiVersion": "1.0",
                "extra": {
                    "categoryId": "126862528",
                    "categoryName": "手机",
                    "showType": "SEARCH_TAB_MARKET_QUERY",
                    "spuId": "100000000067",
                    "spuName": "iphone"
                },
                "searchTabType": "SEARCH_TAB_MARKET",
                "showName": "行情"
            },
            {
                "apiName": "mtop.taobao.idlemtopsearch.search",
                "apiVersion": "1.0",
                "searchTabType": "SEARCH_TAB_INSPECT",
                "showName": "验货好物"
            },
            {
                "apiName": "mtop.taobao.idle.fun.post.search",
                "apiVersion": "2.0",
                "searchTabType": "SEARCH_TAB_FUN",
                "showName": "会玩"
            },
            {
                "apiName": "mtop.taobao.idlemtopsearch.user.search",
                "apiVersion": "1.0",
                "searchTabType": "SEARCH_TAB_USER",
                "showName": "用户"
            }
        ]
```


