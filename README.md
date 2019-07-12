# multiplayer server plugin getting started

## 测试服务器使用说明

### 启动

1. [在 Releases](https://github.com/leancloud/multiplayer-server-plugin-getting-started/releases) 内找最新一次 Release 记录打开 Assets 下载 game-standalone.tar.gz 
1. 解压 game-standalone.tar.gz 后进入 game-standalone 目录
1. 执行 game-standalone 目录内 launch.sh 来启动 game 服务
1. game 服务启动后，launch.sh 会自动展示 game 服务的 STDOUT 输出，不关心其输出时可以 CTRL + C 退出，game 服务会在后台继续运行

### 关闭

1. 进入 game-standalone 目录内执行 shutdown.sh 来关闭后台运行的 game 服务

### 重启

1. 进入 game-standalone 目录内执行 restart.sh 来重启后台运行的 game 服务

### 日志

game 服务在后台运行时产生的日志记录会留在 `game-standlone/logs` 目录内。目前日志名称和用途如下：

文件 | 说明
---- | ---
gc-XXX.current | GC 日志
server.log | game 服务运行日志
stdout.log | 进程的 STDOUT 输出
plugin.log | 用户实现的 plugin 输出的日志
event.log | 事件日志，如用户登录登出等
