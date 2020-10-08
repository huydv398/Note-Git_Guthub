# Cài đặt git trên Linux
* CentOS - RHEL

`yum install -y git-all`

* Ubuntu:

`apt install -y git-all`

Chọn Repo muốn Add:

![](/image/Screenshot_1.png)

Sao chép link:

![](/image/Screenshot_2.png)

Chuyển xang máy Linux:

Tải git về máy:

`git clone [link]`

## Hướng dẫn tạo file và Push lên repo

```
# Tạo một file có tên là fiel
Touch file

git add *

git commit -m "update"

git push origin master
```

* Đăng nhập ssh push cho repo:


```
git config --global user.email "you@example.com"
git config --global user.name "Your Name"
```

Ví dụ:

```
[root@srv Bash-script]# git push origin master
Username for 'https://github.com': huydv398
Password for 'https://huydv398@github.com':
Counting objects: 3, done.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 249 bytes | 0 bytes/s, done.
Total 2 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/huydv398/Bash-script.git
   438e503..4a1762d  master -> master
[root@srv Bash-script]#
```


### Tạo file push

`vi push.md`

thêm vào lệnh:

```
git add *

git commit -m "update"

git push origin master

```

Cho phép quyền thực thi;

`chmod +x push.sh`

