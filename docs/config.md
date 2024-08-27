| 配置项                 | 默认值                                                                                                              | 描述                                                                                    |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| open_update            | True                                                                                                                | 开启更新，若关闭则只运行结果页面服务                                                    |
| open_use_old_result    | True                                                                                                                | 开启使用历史更新结果，合并至本次更新中                                                  |
| open_driver            | False                                                                                                               | 开启浏览器运行，若更新无数据可开启此模式，较消耗性能                                    |
| open_proxy             | True                                                                                                                | 开启代理，自动获取免费可用代理，若更新无数据可开启此模式                                |
| source_file            | config/demo.txt                                                                                                     | 模板文件路径                                                                            |
| source_channels        |                                                                                                                     | 获取更新的频道名称                                                                      |
| final_file             | output/result.txt                                                                                                   | 生成结果文件路径                                                                        |
| open_online_search     | False                                                                                                               | 开启线上检索源功能                                                                      |
| online_search_page_num | 5                                                                                                                   | 在线检索频道获取分页数量                                                                |
| urls_limit             | 15                                                                                                                  | 单个频道接口数量                                                                        |
| open_keep_all          | False                                                                                                               | 保留所有检索结果，会保留非模板频道名称的结果，推荐手动维护时开启                        |
| open_sort              | True                                                                                                                | 开启排序功能（响应速度、日期、分辨率）                                                  |
| open_ffmpeg            | True                                                                                                                | 开启使用 FFmpeg 进行测速，获取更准确的速度与分辨率信息，需要提前手动安装                |
| open_m3u_result        | True                                                                                                                | 开启转换生成 m3u 文件类型结果链接，支持显示频道图标                                     |
| response_time_weight   | 0.5                                                                                                                 | 响应时间权重值（所有权重值总和应为 1）                                                  |
| resolution_weight      | 0.5                                                                                                                 | 分辨率权重值 （所有权重值总和应为 1）                                                   |
| recent_days            | 30                                                                                                                  | 获取最近时间范围内更新的接口（单位天），适当减小可避免出现匹配问题                      |
| ipv_type               | ipv4                                                                                                                | 生成结果中接口的类型，可选值：ipv4、ipv6、全部                                          |
| domain_blacklist       | epg.pw                                                                                                              | 接口域名黑名单，用于过滤低质量含广告类域名的接口                                        |
| url_keywords_blacklist |                                                                                                                     | 接口关键字黑名单，用于过滤含特定字符的接口                                              |
| open_subscribe         | False                                                                                                               | 开启订阅源功能                                                                          |
| subscribe_urls         | https://m3u.ibert.me/txt/fmml_dv6.txt,<br>https://m3u.ibert.me/txt/o_cn.txt,<br>https://m3u.ibert.me/txt/j_iptv.txt | 订阅源列表                                                                              |
| open_multicast         | True                                                                                                                | 开启组播源功能                                                                          |
| multicast_region_list  | 广东                                                                                                                | 组播源地区列表，[更多地区](../updates/multicast/multicast_map.json)，"全部"表示所有地区 |
| multicast_page_num     | 5                                                                                                                   | 组播地区获取分页数量                                                                    |
| open_hotel             | False                                                                                                               | 开启酒店源功能                                                                          |
| open_hotel_tonkiang    | True                                                                                                                | 开启 Tonkiang 酒店源工作模式                                                            |
| open_hotel_fofa        | True                                                                                                                | 开启 FOFA 酒店源工作模式                                                                |
| hotel_region_list      | 广东                                                                                                                | 酒店源地区列表，[更多地区](../updates/fofa/fofa_map.py)，"全部"表示所有地区             |
| hotel_page_num         | 5                                                                                                                   | 酒店地区获取分页数量                                                                    |