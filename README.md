# OhGodAnETHlargementPill-r2
OhGodAnETHlargementPill-r2
installation
cd /opt/
sudo mkdir ./tabletka
cd ./tabletka/
sudo wget https://github.com/format37/OhGodAnETHlargementPill-r2/raw/master/OhGodAnETHlargementPill-r2
sudo chmod +x ./OhGodAnETHlargementPill-r2
Systemd install
sudo nano /etc/systemd/system/ethpill.service
Paste this:

[Unit]
Description=OhGodAnETHlargementPill-r2

[Service]  
Type=simple
ExecStart=/opt/tabletka/OhGodAnETHlargementPill-r2
Restart=on-failure

User=root 

[Install]
WantedBy=multi-user.target
Then

sudo systemctl daemon-reload
sudo systemctl start ethpill
sudo systemctl enable ethpill
Troubleshooting
Does your ETHlargement not work as expected? You're likely running an older memory revision. Here at OhGodACompany, we believe in promotiong a healthy mining lifestyle - that's why we've got a solution for our senior users, too!

With the use of --revA, you can specify which device should be fed our senior solution. If, for example, GPU 0, 3 and 4 aren't the young studs you thought they were, feed them with the following commands:

./OhGodAnETHlargementPill-r2 --revA 0,3,4   
Be sure to leave ETHlargement running in the background, so your NVIDIA noodle can aldente.

sudo systemctl status ethpill
