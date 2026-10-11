\# Bài 1: Kiểm tra cài đặt Docker Engine và chạy Container Hello-World



\## 1. Kiểm tra Docker Version



\### Lệnh thực hiện



```powershell

docker version

```



\### Kết quả



```text

Client:

&#x20;Version:           29.7.2

&#x20;API version:       1.55

&#x20;Go version:        go1.26.5

&#x20;Git commit:        a7dcaa6

&#x20;Built:             Wed Aug  5 18:31:33 2026

&#x20;OS/Arch:           windows/amd64

&#x20;Context:           desktop-linux



Server:

&#x20;Server Version: 29.7.2

```



Docker Client và Docker Server đã kết nối thành công.



\---



\## 2. Kiểm tra Docker Info



\### Lệnh thực hiện



```powershell

docker info

```



\### Kết quả



```text

Server:

&#x20;Containers: 11

&#x20; Running: 4

&#x20; Paused: 0

&#x20; Stopped: 7

&#x20;Images: 12

&#x20;Server Version: 29.7.2

&#x20;Storage Driver: overlayfs

&#x20;Cgroup Version: 2

&#x20;Operating System: Docker Desktop

&#x20;OSType: linux

&#x20;Architecture: x86\_64

&#x20;CPUs: 12

&#x20;Total Memory: 7.602GiB

&#x20;Name: docker-desktop

&#x20;Debug Mode: false

```



Docker Engine hoạt động bình thường và Docker Client có thể kết nối tới Docker Daemon.



\---



\## 3. Chạy Container Hello-World



\### Lệnh thực hiện



```powershell

docker run hello-world

```



\### Kết quả



```text

Unable to find image 'hello-world:latest' locally

latest: Pulling from library/hello-world

4f55086f7dd0: Pull complete

d5e71e642bf5: Download complete

Digest: sha256:5e23090353324d887c48ad5e5c56d294eab81588df9605b07d1afe895f9cc8f8

Status: Downloaded newer image for hello-world:latest



Hello from Docker!

This message shows that your installation appears to be working correctly.



To generate this message, Docker took the following steps:

&#x20;1. The Docker client contacted the Docker daemon.

&#x20;2. The Docker daemon pulled the "hello-world" image from the Docker Hub.

&#x20;   (amd64)

&#x20;3. The Docker daemon created a new container from that image which runs the

&#x20;   executable that produces the output you are currently reading.

&#x20;4. The Docker daemon streamed that output to the Docker client, which sent

&#x20;   it to your terminal.

```



\## 4. Kết luận



Docker Engine đã được cài đặt và hoạt động bình thường.



Docker Client kết nối thành công tới Docker Daemon và container `hello-world` đã được tạo và chạy thành công.



Kết quả kiểm tra đạt yêu cầu với thông báo:



```text

Hello from Docker!

This message shows that your installation appears to be working correctly.

```

