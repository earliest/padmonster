# padmonstercrawl
simple testing crawl tool for pad monsters


fetched some monsters for testing purpose:
=============================================

erlisuo@MacBook-Air:~/practice/padguide/spider/padmonster$ scrapy crawl padmonster
2018-12-25 01:43:56 [scrapy.utils.log] INFO: Scrapy 1.5.1 started (bot: padmonster)
2018-12-25 01:43:56 [scrapy.utils.log] INFO: Versions: lxml 4.2.1.0, libxml2 2.9.8, cssselect 1.0.3, parsel 1.5.1, w3lib 1.19.0, Twisted 18.9.0, Python 3.6.5 |Anaconda, Inc.| (default, Apr 26 2018, 08:42:37) - [GCC 4.2.1 Compatible Clang 4.0.1 (tags/RELEASE_401/final)], pyOpenSSL 18.0.0 (OpenSSL 1.0.2o  27 Mar 2018), cryptography 2.2.2, Platform Darwin-16.7.0-x86_64-i386-64bit
2018-12-25 01:43:56 [scrapy.crawler] INFO: Overridden settings: {'BOT_NAME': 'padmonster', 'DOWNLOAD_DELAY': 1, 'HTTPCACHE_ENABLED': True, 'NEWSPIDER_MODULE': 'padmonster.spiders', 'ROBOTSTXT_OBEY': True, 'SPIDER_MODULES': ['padmonster.spiders']}
2018-12-25 01:43:56 [scrapy.middleware] INFO: Enabled extensions:
['scrapy.extensions.corestats.CoreStats',
 'scrapy.extensions.telnet.TelnetConsole',
 'scrapy.extensions.memusage.MemoryUsage',
 'scrapy.extensions.logstats.LogStats']
2018-12-25 01:43:56 [scrapy.middleware] INFO: Enabled downloader middlewares:
['scrapy.downloadermiddlewares.robotstxt.RobotsTxtMiddleware',
 'scrapy.downloadermiddlewares.httpauth.HttpAuthMiddleware',
 'scrapy.downloadermiddlewares.downloadtimeout.DownloadTimeoutMiddleware',
 'scrapy.downloadermiddlewares.defaultheaders.DefaultHeadersMiddleware',
 'scrapy.downloadermiddlewares.useragent.UserAgentMiddleware',
 'scrapy.downloadermiddlewares.retry.RetryMiddleware',
 'scrapy.downloadermiddlewares.redirect.MetaRefreshMiddleware',
 'scrapy.downloadermiddlewares.httpcompression.HttpCompressionMiddleware',
 'scrapy.downloadermiddlewares.redirect.RedirectMiddleware',
 'scrapy.downloadermiddlewares.cookies.CookiesMiddleware',
 'scrapy.downloadermiddlewares.httpproxy.HttpProxyMiddleware',
 'scrapy.downloadermiddlewares.stats.DownloaderStats',
 'scrapy.downloadermiddlewares.httpcache.HttpCacheMiddleware']
2018-12-25 01:43:56 [scrapy.middleware] INFO: Enabled spider middlewares:
['scrapy.spidermiddlewares.httperror.HttpErrorMiddleware',
 'scrapy.spidermiddlewares.offsite.OffsiteMiddleware',
 'scrapy.spidermiddlewares.referer.RefererMiddleware',
 'scrapy.spidermiddlewares.urllength.UrlLengthMiddleware',
 'scrapy.spidermiddlewares.depth.DepthMiddleware']
2018-12-25 01:43:56 [scrapy.middleware] INFO: Enabled item pipelines:
[]
2018-12-25 01:43:56 [scrapy.core.engine] INFO: Spider opened
2018-12-25 01:43:56 [scrapy.extensions.logstats] INFO: Crawled 0 pages (at 0 pages/min), scraped 0 items (at 0 items/min)
2018-12-25 01:43:56 [scrapy.extensions.httpcache] DEBUG: Using filesystem cache storage in /Users/erlisuo/practice/padguide/spider/padmonster/.scrapy/httpcache
2018-12-25 01:43:56 [scrapy.extensions.telnet] DEBUG: Telnet console listening on 127.0.0.1:6023
2018-12-25 01:43:56 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/robots.txt> (referer: None) ['cached']
2018-12-25 01:43:56 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/pets/1> (referer: None) ['cached']
^^^^^^^^^
2018-12-25 01:43:56 [scrapy.core.scraper] DEBUG: Scraped from <200 http://pad.skyozora.com/pets/1>
{'active_skill_description': '<td colspan="5">對敵方全體造成自身攻擊力×10倍的火屬性傷害</td>',
 'active_skill_init_cd': 8,
 'active_skill_name': 3,
 'att_lv_max': '71',
 'attrs': ['主屬性:火'],
 'hp_lv_max': '144',
 'leader_skill_description': '\n\t\t',
 'name': 'No.001 - ティラ',
 'rarity': 2,
 'rec_lv_max': '13',
 'types': ['龍']}
---------------
http://pad.skyozora.com/pets/501
2018-12-25 01:43:59 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/pets/501> (referer: http://pad.skyozora.com/pets/1)
^^^^^^^^^
2018-12-25 01:43:59 [scrapy.core.scraper] DEBUG: Scraped from <200 http://pad.skyozora.com/pets/501>
{'active_skill_description': '<td colspan="5">對敵方1體造成自身攻擊力×30倍的光屬性傷害</td>',
 'active_skill_init_cd': 20,
 'active_skill_name': 15,
 'att_lv_max': '1023',
 'attrs': ['主屬性:光'],
 'awaken_skills': ['【光ドロップ強化】掉落的光寶珠有20%機率直接出現<img '
                   'src="images/drops/Light+.png" width="25" alt="光強化寶珠" /><br '
                   '/>\n'
                   '效果以加法累積，全隊伍有5個此覺醒技能時則可達到100%出現<img '
                   'src="images/drops/Light+.png" width="25" alt="光強化寶珠" '
                   '/>；<br />\n'
                   '<br />\n'
                   '另外消除至少1顆<img src="images/drops/Light+.png" width="25" '
                   'alt="光強化寶珠" />時，該組寶珠的攻擊力提升5%<br />\n'
                   '此效果以加法累積，如隊伍一共有 y 個此覺醒技能，可為該組寶珠額外提升 5y %的傷害',
                   '【封印耐性】20%機率可將敵人使用的技能封印無效化<br '
                   '/>效果以加法累積，全隊伍有5個此覺醒技能時則可達到100%無效化<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享'],
 'hp_lv_max': '2201',
 'leader_skill_description': '平衡類寵物的HP、攻擊力和回復力1.5倍',
 'leader_skill_name': '我がまま姫の愛情',
 'leader_skill_type': 'images/type/balance.png',
 'name': 'No.501 - アン・パント・ケットバス',
 'rarity': 5,
 'rec_lv_max': '420',
 'types': ['平衡']}
---------------
http://pad.skyozora.com/pets/1001
2018-12-25 01:44:02 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/pets/1001> (referer: http://pad.skyozora.com/pets/501)
^^^^^^^^^
2018-12-25 01:44:03 [scrapy.core.scraper] DEBUG: Scraped from <200 http://pad.skyozora.com/pets/1001>
{'active_skill_description': '<td colspan="5">4回合內，受到傷害時進行受到傷害3倍的暗屬性反擊；並<img '
                             'src="images/drops/Wood.png" width="25"><img '
                             'src="images/change.gif"><img '
                             'src="images/drops/Dark.png" width="25"></td>',
 'active_skill_init_cd': 18,
 'active_skill_name': 8,
 'att_lv_max': '1350',
 'attrs': ['主屬性:暗', '副屬性:光'],
 'awaken_skills': ['【バインド耐性】受到敵人的綁定攻擊時，持有此技能的寵物有50%機率令綁定對自己無效化<br '
                   '/>效果以加法累積，當該寵物持有2個此覺醒技能時則可達到100%無效化',
                   '【バインド耐性】受到敵人的綁定攻擊時，持有此技能的寵物有50%機率令綁定對自己無效化<br '
                   '/>效果以加法累積，當該寵物持有2個此覺醒技能時則可達到100%無效化',
                   '【操作時間延長】寶珠移動時間延長0.5秒',
                   '【自動回復】消除寶珠的回合，回復1000HP',
                   '【マルチブースト】持有此覺醒技能的寵物在協力模式時，HP、攻擊力和回復力全部提升1.5倍',
                   '【封印耐性】20%機率可將敵人使用的技能封印無效化<br '
                   '/>效果以加法累積，全隊伍有5個此覺醒技能時則可達到100%無效化<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享'],
 'hp_lv_max': '2948',
 'leader_skill_description': '8COMBO時攻擊力4倍，每多1COMBO+3倍，最大10COMBO時10倍',
 'leader_skill_name': '冥狼の怒号',
 'name': 'No.1001 - 天臨冥狼神・アヌビス',
 'rarity': 7,
 'rec_lv_max': '588',
 'types': ['神', '攻擊']}
---------------
http://pad.skyozora.com/pets/1501
2018-12-25 01:44:06 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/pets/1501> (referer: http://pad.skyozora.com/pets/1001)
^^^^^^^^^
2018-12-25 01:44:06 [scrapy.core.scraper] DEBUG: Scraped from <200 http://pad.skyozora.com/pets/1501>
{'active_skill_description': '<td colspan="5"><img '
                             'src="images/drops/Heart.png" width="25"><img '
                             'src="images/change.gif"><img '
                             'src="images/drops/Light.png" '
                             'width="25">；並將綁定狀態減少3回合</td>',
 'active_skill_init_cd': 11,
 'active_skill_name': 6,
 'att_lv_max': '1027',
 'attrs': ['主屬性:光', '副屬性:暗'],
 'awaken_skills': ['【2体攻撃】消除4顆與自身屬性相同的寶珠時，持有該技能的寵物、該組寶珠的攻擊力上升50%<br />\n'
                   '並可同時攻擊2個敵人（4顆以上不會有攻擊加乘）<br />\n'
                   '<br />\n'
                   '效果以乘法累積，如該寵物持有2個此覺醒技能時<br />\n'
                   '該組寶珠傷害提升為 (1+50%)(1+50%) = 2.25倍，如此類推',
                   '【スキルブースト】進入地下城的時候，隊伍全體的技能先儲了1回合<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享'],
 'hp_lv_max': '2849',
 'leader_skill_description': '惡魔類寵物的HP、攻擊力和回復力1.5倍',
 'leader_skill_name': 'ビックリマン世代！',
 'leader_skill_type': 'images/type/demon.png',
 'name': 'No.1501 - ヤ魔モトＰ',
 'rarity': 5,
 'rec_lv_max': '0',
 'types': ['惡魔', '體力']}
---------------
http://pad.skyozora.com/pets/2001
2018-12-25 01:44:08 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/pets/2001> (referer: http://pad.skyozora.com/pets/1501)
^^^^^^^^^
2018-12-25 01:44:08 [scrapy.core.scraper] DEBUG: Scraped from <200 http://pad.skyozora.com/pets/2001>
{'active_skill_description': '<td '
                             'colspan="5">對敵方全體造成自身攻擊力×50倍的火屬性傷害；並2回合內，火屬性和暗屬性的攻擊力變成2倍</td>',
 'active_skill_init_cd': 20,
 'active_skill_name': 20,
 'att_lv_max': '108',
 'attrs': ['主屬性:火', '副屬性:暗'],
 'hp_lv_max': '108',
 'leader_skill_description': '\n\t\t',
 'name': 'No.2001 - 神羅魂獣神サイ カード',
 'rarity': 4,
 'rec_lv_max': '108',
 'types': ['強化合成用']}
---------------
http://pad.skyozora.com/pets/2501
2018-12-25 01:44:11 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/pets/2501> (referer: http://pad.skyozora.com/pets/2001)
^^^^^^^^^
2018-12-25 01:44:11 [scrapy.core.scraper] DEBUG: Scraped from <200 http://pad.skyozora.com/pets/2501>
{'active_skill_description': '<td colspan="5">所有寶珠變成<img '
                             'src="images/drops/Heart.png" '
                             'width="25">；並2回合內，受到的傷害減少100%</td>',
 'active_skill_init_cd': 23,
 'active_skill_name': 16,
 'att_lv_max': '1278',
 'attrs': ['主屬性:光', '副屬性:火'],
 'awaken_skills': ['【光属性強化】消除一橫行的<img src="images/drops/Light.png" width="25" '
                   'alt="光寶珠" />時，光屬性的攻擊力上升10%<br />\n'
                   '由此覺醒技能產生的攻擊力計算為 1 + 10%×覺醒數目×橫排數目<br />\n'
                   '（如2橫行或以上連在一起消除，只作1行計算）<br />',
                   '【スキルブースト】進入地下城的時候，隊伍全體的技能先儲了1回合<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享',
                   '【バインド回復】消除一橫行的<img src="images/drops/Heart.png" width="25" '
                   'alt="回復寶珠" />時，綁定狀態縮短3回合<br />\n'
                   '※協力模式時，此覺醒技能效果同時適用於友方的隊伍',
                   '【光属性強化】消除一橫行的<img src="images/drops/Light.png" width="25" '
                   'alt="光寶珠" />時，光屬性的攻擊力上升10%<br />\n'
                   '由此覺醒技能產生的攻擊力計算為 1 + 10%×覺醒數目×橫排數目<br />\n'
                   '（如2橫行或以上連在一起消除，只作1行計算）<br />',
                   '【光属性強化】消除一橫行的<img src="images/drops/Light.png" width="25" '
                   'alt="光寶珠" />時，光屬性的攻擊力上升10%<br />\n'
                   '由此覺醒技能產生的攻擊力計算為 1 + 10%×覺醒數目×橫排數目<br />\n'
                   '（如2橫行或以上連在一起消除，只作1行計算）<br />',
                   '【光属性強化】消除一橫行的<img src="images/drops/Light.png" width="25" '
                   'alt="光寶珠" />時，光屬性的攻擊力上升10%<br />\n'
                   '由此覺醒技能產生的攻擊力計算為 1 + 10%×覺醒數目×橫排數目<br />\n'
                   '（如2橫行或以上連在一起消除，只作1行計算）<br />',
                   '【スキルブースト】進入地下城的時候，隊伍全體的技能先儲了1回合<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享',
                   '【封印耐性】20%機率可將敵人使用的技能封印無效化<br '
                   '/>效果以加法累積，全隊伍有5個此覺醒技能時則可達到100%無效化<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享',
                   '【光属性強化】消除一橫行的<img src="images/drops/Light.png" width="25" '
                   'alt="光寶珠" />時，光屬性的攻擊力上升10%<br />\n'
                   '由此覺醒技能產生的攻擊力計算為 1 + 10%×覺醒數目×橫排數目<br />\n'
                   '（如2橫行或以上連在一起消除，只作1行計算）<br />'],
 'hp_lv_max': '3720',
 'leader_skill_description': '光屬性寵物的HP和回復力2倍、攻擊力1.5倍',
 'leader_skill_name': '輝天使の導引',
 'leader_skill_type': 'images/drops/Light.png',
 'name': 'No.2501 - 創智の大天使・ラファエル',
 'rarity': 8,
 'rec_lv_max': '635',
 'types': ['神', '回復', '體力']}
---------------
http://pad.skyozora.com/pets/3001
2018-12-25 01:44:13 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/pets/3001> (referer: http://pad.skyozora.com/pets/2501)
^^^^^^^^^
2018-12-25 01:44:13 [scrapy.core.scraper] DEBUG: Scraped from <200 http://pad.skyozora.com/pets/3001>
{'active_skill_description': '<td colspan="5">隨機生成<img '
                             'src="images/drops/Water.png" width="25"><img '
                             'src="images/drops/Heart.png" '
                             'width="25">寶珠各3粒；並將自身以外寵物的技能冷卻時間縮短1回合</td>',
 'active_skill_init_cd': 12,
 'active_skill_name': 7,
 'att_lv_max': '1075',
 'attrs': ['主屬性:水'],
 'awaken_skills': ['【水ドロップ強化】掉落的水寶珠有20%機率直接出現<img '
                   'src="images/drops/Water+.png" width="25" alt="水強化寶珠" /><br '
                   '/>\n'
                   '效果以加法累積，全隊伍有5個此覺醒技能時則可達到100%出現<img '
                   'src="images/drops/Water+.png" width="25" alt="水強化寶珠" '
                   '/>；<br />\n'
                   '<br />\n'
                   '另外消除至少1顆<img src="images/drops/Water+.png" width="25" '
                   'alt="水強化寶珠" />時，該組寶珠的攻擊力提升5%<br />\n'
                   '此效果以加法累積，如隊伍一共有 y 個此覺醒技能，可為該組寶珠額外提升 5y %的傷害',
                   '【水ドロップ強化】掉落的水寶珠有20%機率直接出現<img '
                   'src="images/drops/Water+.png" width="25" alt="水強化寶珠" /><br '
                   '/>\n'
                   '效果以加法累積，全隊伍有5個此覺醒技能時則可達到100%出現<img '
                   'src="images/drops/Water+.png" width="25" alt="水強化寶珠" '
                   '/>；<br />\n'
                   '<br />\n'
                   '另外消除至少1顆<img src="images/drops/Water+.png" width="25" '
                   'alt="水強化寶珠" />時，該組寶珠的攻擊力提升5%<br />\n'
                   '此效果以加法累積，如隊伍一共有 y 個此覺醒技能，可為該組寶珠額外提升 5y %的傷害'],
 'hp_lv_max': '2125',
 'leader_skill_description': '龍類寵物的攻擊力和回復力1.5倍；',
 'leader_skill_name': '海神の龍力',
 'leader_skill_type': 'images/type/dragon.png',
 'name': 'No.3001 - 藍海司・ワダツミ＝ドラゴン',
 'rarity': 6,
 'rec_lv_max': '235',
 'types': ['龍']}
---------------
http://pad.skyozora.com/pets/3501
2018-12-25 01:44:16 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/pets/3501> (referer: http://pad.skyozora.com/pets/3001)
^^^^^^^^^
2018-12-25 01:44:16 [scrapy.core.scraper] DEBUG: Scraped from <200 http://pad.skyozora.com/pets/3501>
{'active_skill_description': '<td colspan="5">4回合內，回復力變成2倍；並將綁定狀態減少4回合</td>',
 'active_skill_init_cd': 12,
 'active_skill_name': 8,
 'att_lv_max': '1685',
 'attrs': ['主屬性:火', '副屬性:光'],
 'awaken_skills': ['【火ドロップ強化】掉落的火寶珠有20%機率直接出現<img src="images/drops/Fire+.png" '
                   'width="25" alt="火強化寶珠" /><br />\n'
                   '效果以加法累積，全隊伍有5個此覺醒技能時則可達到100%出現<img '
                   'src="images/drops/Fire+.png" width="25" alt="火強化寶珠" />；<br '
                   '/>\n'
                   '<br />\n'
                   '另外消除至少1顆<img src="images/drops/Fire+.png" width="25" '
                   'alt="火強化寶珠" />時，該組寶珠的攻擊力提升5%<br />\n'
                   '此效果以加法累積，如隊伍一共有 y 個此覺醒技能，可為該組寶珠額外提升 5y %的傷害',
                   '【自動回復】消除寶珠的回合，回復1000HP',
                   '【自動回復】消除寶珠的回合，回復1000HP',
                   '【火属性強化】消除一橫行的<img src="images/drops/Fire.png" width="25" '
                   'alt="火寶珠" />時，火屬性的攻擊力上升10%<br />\n'
                   '由此覺醒技能產生的攻擊力計算為 1 + 10%×覺醒數目×橫排數目<br />\n'
                   '（如2橫行或以上連在一起消除，只作1行計算）<br />',
                   '【火属性強化】消除一橫行的<img src="images/drops/Fire.png" width="25" '
                   'alt="火寶珠" />時，火屬性的攻擊力上升10%<br />\n'
                   '由此覺醒技能產生的攻擊力計算為 1 + 10%×覺醒數目×橫排數目<br />\n'
                   '（如2橫行或以上連在一起消除，只作1行計算）<br />',
                   '【スキルブースト】進入地下城的時候，隊伍全體的技能先儲了1回合<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享',
                   '【バインド耐性】受到敵人的綁定攻擊時，持有此技能的寵物有50%機率令綁定對自己無效化<br '
                   '/>效果以加法累積，當該寵物持有2個此覺醒技能時則可達到100%無效化',
                   '【バインド耐性】受到敵人的綁定攻擊時，持有此技能的寵物有50%機率令綁定對自己無效化<br '
                   '/>效果以加法累積，當該寵物持有2個此覺醒技能時則可達到100%無效化',
                   '【コンボ強化】7COMBO或以上時攻擊力2倍',
                   '【チームHP強化】隊伍的HP量提升5%',
                   '【コンボ強化】7COMBO或以上時攻擊力2倍',
                   '【L字消し攻撃】將5個與自身屬性相同的寶珠以L字形的方式消除，該寵物的攻擊力1.5倍，並可以解除盤面上的寶珠鎖定狀態'],
 'hp_lv_max': '5418',
 'leader_skill_description': '體力類和',
 'leader_skill_name': '芸女神の魂',
 'leader_skill_type': 'images/type/strength.png',
 'name': 'No.3501 - 転生アメノウズメ',
 'rarity': 8,
 'rec_lv_max': '363',
 'types': ['體力', '惡魔', '神']}
---------------
http://pad.skyozora.com/pets/4001
2018-12-25 01:44:19 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/pets/4001> (referer: http://pad.skyozora.com/pets/3501)
^^^^^^^^^
2018-12-25 01:44:19 [scrapy.core.scraper] DEBUG: Scraped from <200 http://pad.skyozora.com/pets/4001>
{'active_skill_description': '<td '
                             'colspan="5">1回合內，敵人的指定傷害值以上吸收技能無效化；並1回合內，結算時增加2COMBO</td>',
 'active_skill_init_cd': 25,
 'active_skill_name': 20,
 'att_lv_max': '3004',
 'attrs': ['主屬性:光'],
 'awaken_skills': ['【スキルブースト】進入地下城的時候，隊伍全體的技能先儲了1回合<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享',
                   '【2体攻撃】消除4顆與自身屬性相同的寶珠時，持有該技能的寵物、該組寶珠的攻擊力上升50%<br />\n'
                   '並可同時攻擊2個敵人（4顆以上不會有攻擊加乘）<br />\n'
                   '<br />\n'
                   '效果以乘法累積，如該寵物持有2個此覺醒技能時<br />\n'
                   '該組寶珠傷害提升為 (1+50%)(1+50%) = 2.25倍，如此類推',
                   '【2体攻撃】消除4顆與自身屬性相同的寶珠時，持有該技能的寵物、該組寶珠的攻擊力上升50%<br />\n'
                   '並可同時攻擊2個敵人（4顆以上不會有攻擊加乘）<br />\n'
                   '<br />\n'
                   '效果以乘法累積，如該寵物持有2個此覺醒技能時<br />\n'
                   '該組寶珠傷害提升為 (1+50%)(1+50%) = 2.25倍，如此類推',
                   '【スキルブースト】進入地下城的時候，隊伍全體的技能先儲了1回合<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享',
                   '【操作時間延長】寶珠移動時間延長0.5秒',
                   '【封印耐性】20%機率可將敵人使用的技能封印無效化<br '
                   '/>效果以加法累積，全隊伍有5個此覺醒技能時則可達到100%無效化<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享',
                   '【スキルブースト】進入地下城的時候，隊伍全體的技能先儲了1回合<br />\n'
                   '※協力模式時，此覺醒技能的效果可與友方隊伍共享',
                   '【バインド耐性】受到敵人的綁定攻擊時，持有此技能的寵物有50%機率令綁定對自己無效化<br '
                   '/>效果以加法累積，當該寵物持有2個此覺醒技能時則可達到100%無效化',
                   '【バインド耐性】受到敵人的綁定攻擊時，持有此技能的寵物有50%機率令綁定對自己無效化<br '
                   '/>效果以加法累積，當該寵物持有2個此覺醒技能時則可達到100%無效化',
                   '【2体攻撃】消除4顆與自身屬性相同的寶珠時，持有該技能的寵物、該組寶珠的攻擊力上升50%<br />\n'
                   '並可同時攻擊2個敵人（4顆以上不會有攻擊加乘）<br />\n'
                   '<br />\n'
                   '效果以乘法累積，如該寵物持有2個此覺醒技能時<br />\n'
                   '該組寶珠傷害提升為 (1+50%)(1+50%) = 2.25倍，如此類推',
                   '【追加攻撃】消除一直行的回復寶珠時，對敵人追加1點固定傷害',
                   '【雲耐性】可將敵人的雲攻撃100%無效化'],
 'hp_lv_max': '3021',
 'leader_skill_description': '龍類和',
 'leader_skill_name': '今の一撃 申し分なし！',
 'leader_skill_type': 'images/type/dragon.png',
 'name': 'No.4001 - 飛天御剣流継承者・比古清十郎',
 'rarity': 7,
 'rec_lv_max': '20',
 'types': ['攻擊', '龍']}
---------------
http://pad.skyozora.com/pets/4501
2018-12-25 01:44:22 [scrapy.core.engine] DEBUG: Crawled (200) <GET http://pad.skyozora.com/pets/4501> (referer: http://pad.skyozora.com/pets/4001)
^^^^^^^^^
2018-12-25 01:44:22 [scrapy.core.scraper] DEBUG: Scraped from <200 http://pad.skyozora.com/pets/4501>
{'active_skill_description': '<td colspan="5"><img '
                             'src="images/drops/Light.png" width="25"><img '
                             'src="images/change.gif"><img '
                             'src="images/drops/Water.png" width="25">；<img '
                             'src="images/drops/Heart.png" width="25"><img '
                             'src="images/change.gif"><img '
                             'src="images/drops/Wood.png" '
                             'width="25">；並1回合內，寶珠移動時間延長2秒</td>',
 'active_skill_init_cd': 11,
 'active_skill_name': 11,
 'att_lv_max': '150',
 'attrs': ['主屬性:水'],
 'hp_lv_max': '150',
 'leader_skill_description': '\n',
 'name': 'No.4501 - 蒼頂の華龍・スターリングの希石',
 'rarity': 7,
 'rec_lv_max': '150',
 'types': ['進化用', '龍']}
---------------
2018-12-25 01:44:22 [scrapy.core.engine] INFO: Closing spider (finished)
2018-12-25 01:44:22 [scrapy.statscollectors] INFO: Dumping Scrapy stats:
{'downloader/request_bytes': 4607,
 'downloader/request_count': 11,
 'downloader/request_method_count/GET': 11,
 'downloader/response_bytes': 238014,
 'downloader/response_count': 11,
 'downloader/response_status_count/200': 11,
 'finish_reason': 'finished',
 'finish_time': datetime.datetime(2018, 12, 25, 9, 44, 22, 313420),
 'httpcache/firsthand': 9,
 'httpcache/hit': 2,
 'httpcache/miss': 9,
 'httpcache/store': 9,
 'item_scraped_count': 10,
 'log_count/DEBUG': 23,
 'log_count/INFO': 7,
 'memusage/max': 49868800,
 'memusage/startup': 49868800,
 'request_depth_max': 9,
 'response_received_count': 11,
 'scheduler/dequeued': 10,
 'scheduler/dequeued/memory': 10,
 'scheduler/enqueued': 10,
 'scheduler/enqueued/memory': 10,
 'start_time': datetime.datetime(2018, 12, 25, 9, 43, 56, 458011)}
2018-12-25 01:44:22 [scrapy.core.engine] INFO: Spider closed (finished)
