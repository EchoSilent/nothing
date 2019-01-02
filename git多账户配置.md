### git 配置多个账户

- 生成sshkey
```
ssh-keygen -t rsa -C "foo@bar.com"
```
- 关联账户信息
- 配置.ssh/config
```
Host github.com
Hostname github.com
User git
IdentityFile ~/.ssh/id_rsa
```
- 测试链接
```
ssh -v git@github.com
ssh -T git@github.com
```
- 取消全局配置
```
git config --global --unset user.name
git config --global --unset user.email
```
- 关联repo账户
```
git config --lcoal user.name "foo"
git config --local user.email "bar"
```