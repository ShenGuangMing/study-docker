# 谈谈docker虚悬镜像是什么
## 是什么
仓库名、标签都是<none>的镜像，俗称虚悬镜像dangling image



# 为什么Dockers镜像要采用分层结构

镜像分层最大的好处就是共享资源，方便复制迁移，就是为了复用

比如说有个镜像都是从相同的base镜像构建而来，那么Docker Host只需在磁盘上保存一份base镜像；同时内存中也只需要加载一份base镜像，就可以为所有容器服务了。而且镜像的每一层都可以被共享



