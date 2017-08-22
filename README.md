# Prepare
```
ssh-keygen -R [127.0.0.1]:2222
git clone https://github.com/dhalturin/Testing_owncloud-vagrant-ansible.git
cd Testing_owncloud-vagrant-ansible
```

# Steps to deploy ownCloud
- vagrant up

# Used versions
```
[06:49:43] {dhalturin@MacBook-Air.local}~/repos/owncloud-vagrant-ansible> ansible-playbook --version
ansible-playbook 2.3.2.0
  config file =
  configured module search path = Default w/o overrides
  python version = 2.7.13 (default, Dec 18 2016, 07:03:39) [GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.42.1)]
--------------------------------------------------------------------------------
[06:50:18] {dhalturin@MacBook-Air.local}~/repos/owncloud-vagrant-ansible> vagrant --version
Vagrant 1.9.5
```

# Result
```
Url: https://127.0.0.1:8087/
User: admin
Pass: password

[06:49:40] {dhalturin@MacBook-Air.local}~/repos/owncloud-vagrant-ansible> curl https://127.0.0.1:8087/ -k -I
HTTP/1.1 302 Found
Server: nginx/1.10.2
Date: Tue, 22 Aug 2017 03:49:43 GMT
Content-Type: text/html; charset=UTF-8
Connection: keep-alive
X-Powered-By: PHP/7.0.22
Set-Cookie: oczp3juaukvn=elcaiinc0otufrqsj8rp5rl1v0; path=/; HttpOnly
Expires: Thu, 19 Nov 1981 08:52:00 GMT
Cache-Control: no-store, no-cache, must-revalidate
Pragma: no-cache
Set-Cookie: oc_sessionPassphrase=06czx%2FYoZT7jSPbnvPxH24ebtPQKbn9T2s6pzJ%2FiORcodL%2Bp7hFQ%2FPYclkorGwNUdd4wrKQDGzN%2BMubqOQzWv9G%2FgN8qkCSXrJfCD7Jp2QbyzBSIDs2QFIwY%2BLVpPp17; path=/; secure; HttpOnly
Content-Security-Policy: default-src 'self'; script-src 'self' 'unsafe-eval'; style-src 'self' 'unsafe-inline'; frame-src *; img-src * data: blob:; font-src 'self' data:; media-src *; connect-src *
Location: https://127.0.0.1:8087/login
Strict-Transport-Security: max-age=15552000; includeSubDomains
X-Content-Type-Options: nosniff
X-Frame-Options: SAMEORIGIN
X-XSS-Protection: 1; mode=block
X-Robots-Tag: none
X-Download-Options: noopen
X-Permitted-Cross-Domain-Policies: none
```
