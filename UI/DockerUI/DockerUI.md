DockerUI是一个开源的基于Docker API的web应用程序，提供等同Docker命令行的大部分功能，支持container管理，image管理。它最值得称道的是它华丽的设计和用来运行和管理docker的简洁的操作界面.
DockerUI优点：
	1）支持container批量操作；
	2）支持image管理（虽然比较薄弱）
DockerUI缺点：
	不支持多主机。
1.下载镜像
	docker pull uifd/ui-for-docker
2.启动容器
	docker run -it -d --name docker-web -p 9000:9000 -v /var/run/docker.sock:/var/run/docker.sock docker.io/uifd/ui-for-docker
3.查看容器
	docker ps
4.页面查看docker信息
	ip：9000
tips:
	1.注意防火墙问题。
	2.端口占用问题。
