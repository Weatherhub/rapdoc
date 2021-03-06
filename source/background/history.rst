发展历史
=================

.. contents ::

美国RUC发展历史
-------------------

美国首先在1991年开始了快速更新同化预报技术的研究开发, 并于1994年开始在NCEP业务运行(RUC1)。RUC1采用静力平衡原始方程模式, 水平分辨率60km, 垂直方向25层, 使用最优插值(Optimal Interpolation, OI)技术每3h进行一次资料同化更新 ;之后经过几次更新和升级2005年系统水平分辨率已提升至13km, 垂直方向50层, 采用3维变分(3DVAR)技术, 进行1h同化更新。为得到更准确的云和水物质初始场, 从2002年(RUC20)起, 系统开始使用云分析技术利用卫星观, 之后通过逐步补充更多的观测资料(包括雷达反射率), 对云的描述更加完善。云分析技术在RUC系统初始化过程中起着至关重要的作用。

虽然RUC系统经历了多次升级, 但其模式动力框架还是静力模式。随着非静力模式的发展, NOAA/NCEP(RUC系统业务应用部门)和NOAA/ESRL/GSD(RUC系统研发机构)于2002年决定发展以非静力模式WRF为基础的新一代快速更新同化预报系统, 除模式替换外, 同化系统也将换成GSI(GridpointStatistical Interpolation)以增加系统对卫星辐射率的直接同化功能。自2003年以来, 在经过了WRF-RUC测试(以RUC初始场驱动WRF, Weather Researchand Forecasting)、WRF动力框架比较测试(在WRF-ARW和WRF-NMM两种动力框架中选择了WRF-ARW)、GSI系统功能拓展(移植RUC已有的云分析、雷达反射率资料同化、非绝热DFI、地表资料同化等技术)、云分析模块升级(增加深对流云量条件下, 连续高频次的低密度资料同化效果可能劣于低频次的高密度资料同化。这种时、空分辨率上的两难取舍取决于风暴的移速, 当风暴准静止时, 同化频率可取的非常低以获得空间上高密度的资料;当风暴移速较快时, 要适当增加同化频率以降低时间代表性误差, 但太高的频率又会造成资料空间代表性上的不足, 影响同化效果。


中国RUC发展历史
-------------------

近几年, 我国加大了针对中小尺度天气系统观测的布网力度, 观测手段及自动化水平逐步接近国际先进水平, 具备了发展快速同化系统的观测基础。在我国东部地区已建成包括自动气象站、单双频地基GPS(Global Position System)站、风廓线仪、多普勒雷达和微波辐射计在内的局地中小尺度观测网, 观测资料在时间和空间分辨率上都得到了极大的提高。通常一个时次的常规地面观测超过1000个, 自动站资料可达2万个以上, 雷达等非常规探测在硬件建设和布网上发展非常迅速。目前, 长三角地区已有13部多普勒天气雷达(徐州、连云港、盐城、南京、南通、上海南汇及青浦、杭州、金华、宁波、舟山、温州、衢州), 在建4部(江苏常州、浙江湖州、杭州及丽水)。计划建设25部风廓线仪, 其中江苏新建6部, 浙江新建5部(已建成湖州、义乌、嘉兴), 上海新建11部(已建成10部), 并完成长三角风廓线组网。长三角区域将有79个GPS站可参与加密观测, 其中参与中国气象局业务考核的有江苏62个、上海9个、浙江1个。这些观测在日常业务预报与科学研究中起着举足轻重的作用。如何有效利用各种常规和非常规气象资料, 充分发挥先进探测手段的作用, 提高突发灾害性天气的预报能力, 提供时间上更密集、空间和量级上更准确的精细数值预报服务, 已成为日益突出的问题。在国内, 虽然对快速更新同化和预报技术的研究和应用起步较晚, 但近年来发展迅速。以上海、北京及广州为代表, 基于本地特色, 分别建立了不同技术路线的快速更新同化预报系统。

2009年1月, 上海建立了基于ADAS资料同化系统和区域中尺度数值模式WRF的快速更新同化预报系统(SMB-WARR, Shanghai Meteorological Bureau-WRF ADAS Rapid Refresh System), 同年7月准业务运行, 2009年底实现业务运行至今。该系统的水平分辨率为3km, 垂直分辨率为51层, 预报区域覆盖华东及其周边地区, 系统采用逐小时循环同化的方式对观测资料进行同化, 每日02时冷启动, 冷启动的背景场和侧边界条件由NCEP GFS 6h的全球预报场提供, 其他时刻同化的背景场则由SMB-WARR系统上一时次的1h预报场提供。系统每小时启动一次预报, 预报时效为12h, 并提供逐小时高分辨率中尺度分析场。实时业务的同化观测资料包括常规天气观测、机场地面报、船舶、浮标、自动站、飞机报、探空、雷达反射率和FY-2E红外和可见光辐射率资料, 如图2所示。其中, 雷达反射率和FY-2E红外和可见光辐射率资料主要采用云分析技术进行同化, 雷达反射率资料主要用于改进和修正云和降水的垂直结构特征, 而FY-2E红外和可见光辐射率观测则主要用于修正初始场中有关云顶高度和云量的特征, 关于云分析技术的具体叙述。其他观测资料则是通过ADAS的逐步订正方法实现同化。通过3年来的测试及优化, 该系统在短时临近天气预报中发挥了越来越重要的作用;上海地区2011年汛期强对流预报检验表明, 其对午后强对流天气的预报明显优于同时次起报的华东区域中尺度预报模式(SMB-WARMS)和欧洲中心的高分辨模式的预报结果。

北京同化预报系统(BJ-RUC)亦采用WRF模式, 与SMB-WARR不同之处在于其同化系统采用三维变分技术。区域配置采用三重嵌套27×9×3km, 3km分辨率的预报区域主要覆盖北京及其周边地区, 垂直分辨率均为37层。每日20时冷启动, 冷启动的背景场和侧边界条件由NCEP GFS 6h的全球预报场提供, 每隔3h同化一次探空、地面、船舶观测资料以及北京地区的自动站和地基GPS PW可降水量观测资料, 预报时效为18h。其业务运行结果表明, 3km分辨率无论是降水时段、落区和雨量均较9km分辨率有更好的预报效果, 尤其是大量级降水的预报, 但系统对局地对流降水的预报能力仍然有限。

广州在GRAPES_meso及三维变分同化基础上发展了快速更新同化预报系统(GRAPES-CHAF)。模式分辨率为0.12° , 预报区域主要覆盖华南地区。采用三维变分同化方法对卫星反演的云迹风、雷达径向风、VAD风、飞机报、地面、船舶和探空观测资料进行同化, 通过云分析技术和nudging方法对雷达回波进行同化。该系统采用逐小时循环同化和每3h间隔的滚动预报, 预报时效为24h。多种测试和汛期连续试验表明, 系统运行稳定可靠。通过1个月的滚动预报综合分析和个例预报分析均表明, 预报稳定有效, 与观测分布基本一致, 初步具备开展短时临近预报的能力。在原广州热带海洋气象研究所GRAPES-CHAF基础上, 国家气象中心采用新版的GRAPES-Meso模式与区域GRAPES-3DVAR, 建立了优化后的RUC同化预报系统。其模式分辨率为0.15°, 预报区域覆盖全国, 其同化的观测资料类型与GRAPES-CHAF类似。每3h启动一次预报, 预报时效为24h。

对比国内各家快速更新同化预报系统, 北京和广州均采用3DVAR而上海使用ADAS方案;从同化资料的种类看, 广州的系统资料种类相对较多(如云导风、雷达径向风等)。然而和美国的RUC/RR系统相比, 国内系统可同化的高空资料种类和数量严重不足, 尤其是飞机报资料。飞机报是美国RUC/RR系统高频资料的重要来源, 每小时的资料量为数千个, 而国内使用的飞机报不到上述资料量的十分之一。此外, 国内卫星、雷达及其反演资料的质量也一定程度上影响了快速更新同化预报系统的发展。
