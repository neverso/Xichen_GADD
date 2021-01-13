# 前言

因为个人经验与能力的不足和内心种种悬而未决的念头与顾虑，这份在两年前就起了念头的游戏音频设计文档一直被拖到了现在才正式开篇，可见这对我来说着实是一个不小的挑战。入行至今已快满五年，在积累了 Ubisoft Shanghai Studios 的项目经验和经历了 NExT Studios 从零开始参与全新项目的开发之后，我觉得终于等到了一个合适的时机来正式开始撰写这份文档，跟大家详细地聊一聊我对游戏音频设计的各种想法。

首先，容我来说一下写这份文档的四个初衷。
第一点是主观的动机。从上大学开始，我就狂热地喜欢拍照，非常享受从按下快门、后期处理到最后呈现一张能给他人带来美感的作品的过程；工作之后，我做了一个专注声音设计的主题网站，在自我学习与沉淀的同时也给别人提供了便利的资讯渠道；两年前，我尝试拍起了 Vlog，想通过新的方式去更多地表达自己的想法。曾有朋友说我是“带有媒体属性的技术工作者”，这些我一直在做的事情，其实都是我强烈表达欲的体现。所以，这份文档就是一个新的表达出口。我希望能持续地输出有价值的内容，说得大一点，这可能就是我目前感悟到的人生终极意义：在这世上留下点东西，好让死后的自己“活”得更久一点。
第二点是客观的促因。从我以“声音设计”这个标签在网上被大家熟知之后，一直有人来咨询各种有关游戏音频设计的大小问题，我都尽可能地做出了力所能及的回复。但是很多时候，这些问题往往是无法用简短的私信或邮件往来就能解答清楚的，甚至有些问题连我们自己这些一线从业者们都还没有想清楚。所以，我想通过这份文档来做一次疏理，比较系统地把我对游戏音频设计的认知阐述出来。
第三点是自我的挑战。当下的互联网已经迅速步入了视频时代，个人表达的方式多种多样。综合比较下来，价值浓缩度最高的无疑还是文字。虽然文字这种形式与播客或者 Vlog 等媒介相比，确实没有那么大的吸引力，估计还会劝退不少人，但这或许并不是什么坏事——让真正想要深入了解游戏音频设计的朋友们的收益最大化，是这份文档最大的价值体现。如果只是为了博得更多的关注度，大家多去看看我的 Vlog 系列就可以了。
第四点是长远的价值。针对国内的游戏开发行业，一直有一个老生常谈的话题，那就是为什么我们做不出 3A 大作。这个问题涉及到非常多的因素，其中肯定会被提到的一点就是所谓的“缺乏技术积累”。那又如何来做技术积累呢？就以游戏音频设计来说，我想通过梳理在实际项目中的思考、与前辈同行们的深入交流、系统性的总结沉淀的途径，来让那些原本只在工作室内部小范围分享的工作流程、开发方法和经验教训，能被行业内更多的人所了解、所讨论、所学习。整个行业的提升才是真正的“技术积累”，才有可能让我们尽早做出 3A 大作。

再来聊一聊我对这份文档的定义。
首先，这是一份中文书写的文档，英语能力不足的朋友们请不用担心。虽然英语作为我的第一工作语言用来书写专业性文档可能更加合适，但正如上文提到的，我的首要目标受众是国内的朋友们，那就还是直接用中文吧。
第二，这不是一份纯技术向的文档。为了说明和演示的目的，文档中一定会涉及到一些游戏开发与声音设计的专业工具，但这都不是为了介绍工具本身的使用。大家如果想要学习开发工具，烦请自行查阅官方文档，肯定比我说得要更加清楚明了。文档的主体将会是以我参与过的项目为例，展开多个板块来阐述我的工作流程和方法、经验总结与教训和一些值得更多思考的话题。我想象中的这份文档应该是：对想入行或是刚入行的新朋友们来说，这可能是一本由浅入深的小指南，让你了解一下游戏音频设计师是做什么和怎么做的；对已经在业内的同行朋友们来说，这可能是一本抛砖引玉的随笔集，希望你看过之后也能有所收获，激发出新的想法。如果真的引到了玉，期待你也能跟大家来聊一聊。
第三，这是一份不断更新的在线文档。任何一本技术书，都会面临技术更新导致观点过时的情况，所以才会有经年不断的修订版。我觉得，游戏音频设计作为一门典型的艺术与技术相结合的学科，其中艺术方面的美学设计会随着大众审美的趋势和个人品味的提升而不断变化，而其中技术方面的实现逻辑则会随着开发工具和终端平台的更新而不断演进。所以，既然我已经有了个人网站，那就干脆做成一份在线文档，持续地与大家分享我在职业成长过程中的想法迭代和心路历程。
最后，这是一份完全免费的文档。游戏音频设计在整个游戏开发行业中是一个相对小众的领域，从业人数决定了想要靠这个知识分享来发家致富是不太可能的，所以我就不打算折腾那些知识付费的事情了。当然，我也欢迎你的小额资助，请我喝一杯咖啡，或者帮我分摊一下网站服务器的费用。

最后，我要感谢身边各位优秀的前辈、同事和朋友们，是你们追求卓越的品质和耳濡目染的影响，让我不得不逼迫自己要赶上你们的步伐，抓紧时间去完成给自己定下的一个个目标。
当然，还要特别感谢我的父母，你们完全的信任、充分的理解和无言的鼓励是我最坚实的后盾。以后我说要回家的时候，不要再用“家里没事你忙你的吧”的说辞来劝说我了，开车两小时的回家路途一点儿也不累，我就是想回来看看你们。

希辰
2020.1.8

***