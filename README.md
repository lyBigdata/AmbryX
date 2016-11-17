#Ambry

源项目地址：[Ambry](https://github.com/linkedin/ambry)

Ambry是领英开源的分布式对象存储框架，是一种NFS的实现。

以下翻译自Ambry团队官方博客：

 > 在当今互联网时代，多媒体内容越来越普遍。资料照片，邮件附件，微博博客等是常见的多媒体文件（例如图片，视频，PDF等等）的展示形式。用户上传这些文件至服务器，服务器保存这些文件至后台存储系统并且通过CDN（Content Delivery Network）来分发这些文件并展示在网站上。
随着Linkin业务量的增长，传统的后台存储系统暴露了很多在扩展性，可用性和易操作性上的问题。两年前，我们回顾了我们之前用的技术，并着手于优化改造，Ambry就是之后的成果。从我们在2014年开始分享关于Ambry这个内部项目的数据开始，Ambry在网络延迟和传输效率上有了长足的进步。并且， 在我们给一些公司做了相关的展示后，他们对Ambry展示了极大的兴趣，并想将Ambry最为他们的后台存储系统。
今天，我们宣布Ambry开源（Apache 2.0 协议）。Ambry适用于存储多媒体对象并且提供多媒体服务。多媒体内容对于任何一个网站在提高用户交互品质，提升用户体验上都是至关重要的。未来会有更多的公司投入到多媒体渠道中，尤其是随着视频技术和VR的发展。在这种趋势下，Ambry将扮演一个至关重要的角色。
Ambry是一个分布式不可变高可用对象存储系统，并且可容易扩展。 Ambry适用于存储从几KB到几GB的多媒体对象，并能保证高吞吐量以及低延迟。他也能实现从客户端到存储层端到端的直接通信，反之亦可。系统可以跨机房多活热部署，并且能提供非常廉价的存储。
我们发现没有现成的开源解决方案能满足我们对于水平扩展性，可用性和多活数据中心配置的需求。我们找到的分布式文件系统对于小对象的处理并不是很好，并且为了一致性牺牲了可用性，没有关注于实时应用并且难以操作维护。有一些对象存储解决方案，但是大部分不成熟，不适用于不同大小的对象存储，而且在性能上没有达到我们对于实时传输的要求。我们相信Ambry达到了我们各方面的需求并且在未来可以成为建设多媒体通道的核心。

#AmbryX
我们将基于Ambry做一些完善和补充，并且做一些适合于国内应用环境的改造。在此立项，欢迎大家补充想法。
#历史改造
1.改造项目依赖管理为更多国内人使用的maven