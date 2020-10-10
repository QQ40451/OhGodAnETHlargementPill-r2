OhGodAnETHlargementPill-r2

安装：

cd /opt/

sudo mkdir ./tabletka

cd ./tabletka/

sudo wget https://github.com/QQ40451/OhGodAnETHlargementPill-r2/raw/master/OhGodAnETHlargementPill-r2

sudo chmod +x ./OhGodAnETHlargementPill-r2

安装服务：

sudo nano /etc/systemd/system/ethpill.service

黏贴以下内容:

[Unit]
Description=OhGodAnETHlargementPill-r2

[Service]  

Type=simple

ExecStart=/opt/tabletka/OhGodAnETHlargementPill-r2

Restart=on-failure

User=root 

[Install]

WantedBy=multi-user.target


运行:

sudo systemctl daemon-reload

sudo systemctl start ethpill

sudo systemctl enable ethpill


常见问题：

可以用参数 --revA,来指定哪些卡加载补丁.例如 GPU 0, 3 和 4 需要打补丁的话这样运行：

./OhGodAnETHlargementPill-r2 --revA 0,3,4   

注意：补丁需要保持再后台运行。

状态查看:

sudo systemctl status ethpill
