# gtwisted
Twisted的gevent版本
这个版本主要fix了gevent版本高于1.0.2时, gfirefly启动服务器报node [x] lose

主要原因是gevent的新版本有一个特性(引用自gevent Issues作者的原话):
As mentioned, that is the desired behaviour. Keep the handler alive to keep the socket alive.
https://github.com/gevent/gevent/issues/700
https://github.com/gevent/gevent/issues/594
