# STRUCTURE-CLEAN — Архитектура проекта (после 2025-11-05)

_Фильтры: код, конфиги, сервисы, зависимости. Исключён мусор._
_Корни: /home/ubuntu/lab /home/ubuntu/services /etc/systemd/system /etc/caddy /etc/cron.d /usr/local/bin /usr/local/lib /opt_

## /home/ubuntu/lab
```text
2025-11-05 13:00 d /home/ubuntu/lab/accounting/.env.lab
2025-11-05 13:08 f /home/ubuntu/lab/Добавляем venv.txt
2025-11-05 13:10 f /home/ubuntu/lab/README.md
2025-11-05 13:18 f /home/ubuntu/lab/personal/requirements.txt
2025-11-05 15:41 f /home/ubuntu/lab/personal/scratch/2025-11-05-pf-webhook/app_dev_test.py
2025-11-05 15:43 f /home/ubuntu/lab/personal/scratch/results/last.json
2025-11-05 17:57 f /home/ubuntu/lab/personal/scratch/2025-11-05-pf-webhook/app_dev.py
2025-11-05 19:56 f /home/ubuntu/lab/personal/docs/LAB-Personal-Webhook.md
2025-11-06 19:10 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/backups/20251108T010737Z/Caddyfile
2025-11-06 23:42 f /home/ubuntu/lab/invest/scratch/2025-11-06-pf-webhook/app_dev.py
2025-11-07 15:32 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/requirements.txt
2025-11-07 15:48 f /home/ubuntu/lab/invest/repos/invest-services/src/pf_invest_webhook/requirements.txt
2025-11-07 16:01 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/test_airtable_write.py
2025-11-07 17:31 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/backups/20251108T010737Z/.env.invest.lab
2025-11-07 17:31 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/snapshots/20251107T214903Z/.env.invest.lab
2025-11-07 17:31 f /home/ubuntu/lab/invest/env/.env.invest.lab
2025-11-07 18:27 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/backups/20251108T010737Z/telemetry.py
2025-11-07 18:27 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/services/telemetry.py
2025-11-07 18:27 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/snapshots/20251107T214903Z/telemetry.py
2025-11-07 18:40 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/backups/20251108T010737Z/pf_invest_webhook-lab.service
2025-11-07 18:57 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/backups/20251108T010737Z/app.py
2025-11-07 20:06 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/backups/20251108T010737Z/airtable_writer.py
2025-11-07 21:36 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/airtable_writer.py
2025-11-07 21:36 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/snapshots/20251107T214903Z/airtable_writer.py
2025-11-07 22:20 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/patch_sync.sh
2025-11-07 22:27 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/snapshots/20251107T214903Z/app.py
2025-11-07 23:10 f /home/ubuntu/lab/invest/tools/e2e_webhook.sh
2025-11-08 00:13 f /home/ubuntu/lab/invest/results/invest_sizes.txt
2025-11-08 00:13 f /home/ubuntu/lab/invest/results/invest_tree_full.txt
2025-11-08 01:18 f /home/ubuntu/lab/invest/apps/pf_invest_webhook_fastapi/app.py
2025-11-10 17:38 f /home/ubuntu/lab/invest/repos/invest-services/README.md
2025-11-10 17:38 f /home/ubuntu/lab/invest/repos/invest-services/doc/adr/0001-repo-structure.md
2025-11-10 17:38 f /home/ubuntu/lab/invest/repos/invest-services/doc/project-notes/NEXT.md
2025-11-10 17:38 f /home/ubuntu/lab/invest/repos/invest-services/pyproject.toml
2025-11-10 17:38 f /home/ubuntu/lab/invest/repos/invest-services/requirements-dev.txt
2025-11-10 19:52 f /home/ubuntu/lab/invest/repos/invest-services/doc/project-notes/COMMENT-2025-11-10.md
2025-11-11 01:32 f /home/ubuntu/lab/invest/repos/invest-services/.github/workflows/docs-sync.yml
2025-11-11 16:07 f /home/ubuntu/lab/personal/repos/personal-services/README.md
2025-11-11 17:49 f /home/ubuntu/lab/personal/repos/personal-services/docs/projects/invest/how-to/systemd/git-autopush@.timer
2025-11-11 21:25 f /home/ubuntu/lab/invest/repos/invest-services/doc/project-notes/CHAT-2025-11-11-invest-sync.md
2025-11-11 21:26 f /home/ubuntu/lab/personal/repos/personal-services/docs/common/how-to/_index.md
2025-11-11 21:26 f /home/ubuntu/lab/personal/repos/personal-services/docs/projects/invest/how-to/_chat-quick-start.md
2025-11-11 21:48 f /home/ubuntu/lab/personal/repos/personal-services/docs/projects/invest/how-to/systemd/git-autopush@.service
2025-11-11 21:51 f /home/ubuntu/lab/personal/repos/personal-services/docs/common/how-to/README.md
2025-11-11 22:01 f /home/ubuntu/lab/personal/repos/personal-services/test.txt
2025-11-11 22:51 f /home/ubuntu/lab/invest/repos/invest-docs/NEXT.md
2025-11-11 22:51 f /home/ubuntu/lab/invest/repos/invest-docs/README.md
2025-11-11 22:51 f /home/ubuntu/lab/invest/repos/invest-docs/adr/0001-repo-structure.md
2025-11-11 22:51 f /home/ubuntu/lab/invest/repos/invest-docs/project-notes/CHAT-2025-11-11-invest-sync.md
2025-11-11 22:51 f /home/ubuntu/lab/invest/repos/invest-docs/project-notes/COMMENT-2025-11-10.md
2025-11-11 22:51 f /home/ubuntu/lab/invest/repos/invest-docs/project-notes/COMMENT-2025-11-12.md
2025-11-11 22:51 f /home/ubuntu/lab/invest/repos/invest-docs/project-notes/NEXT.md
2025-11-11 23:17 f /home/ubuntu/lab/invest/repos/invest-services/doc/NEXT.md
2025-11-11 23:17 f /home/ubuntu/lab/invest/repos/invest-services/doc/project-notes/COMMENT-2025-11-12.md
2025-11-12 00:21 f /home/ubuntu/lab/invest/repos/invest-services/doc/README.md
2025-11-12 00:23 f /home/ubuntu/lab/personal/repos/personal-services/docs/common/how-to/git-ritual.md
2025-11-12 00:23 f /home/ubuntu/lab/personal/repos/personal-services/docs/projects/invest/how-to/00-start.md
2025-11-12 00:25 f /home/ubuntu/lab/personal/repos/personal-services/repo-STRUCTURE.txt
2025-11-12 11:38 f /home/ubuntu/lab/invest/repos/invest-services/doc/how-to/README.md
2025-11-12 15:51 f /home/ubuntu/lab/invest/repos/invest-services/tools/gen_structure_since.sh
2025-11-12 16:31 f /home/ubuntu/lab/invest/repos/invest-services/tools/gen_system_structure.sh
2025-11-12 16:36 f /home/ubuntu/lab/invest/repos/invest-services/tools/gen_clean_structure.sh
2025-11-12 16:43 f /home/ubuntu/lab/invest/repos/invest-services/tools/gen_structure_index.sh
2025-11-12 17:03 f /home/ubuntu/lab/invest/repos/invest-services/tools/gen_index_raw_links.sh
2025-11-12 18:09 f /home/ubuntu/lab/invest/repos/invest-services/tools/gen_docs.sh
2025-11-12 18:48 f /home/ubuntu/lab/invest/repos/invest-services/doc/INDEX-RAW-LINKS.md
2025-11-12 19:17 f /home/ubuntu/lab/invest/repos/invest-services/doc/STRUCTURE-system-since-2025-11-05.md
2025-11-12 19:18 f /home/ubuntu/lab/invest/repos/invest-services/doc/STRUCTURE-CLEAN.md
2025-11-12 19:18 f /home/ubuntu/lab/invest/repos/invest-services/doc/STRUCTURE-since-2025-11-05.md
```

## /home/ubuntu/services
```text
2025-11-05 13:18 f /home/ubuntu/services/requirements.txt
```

## /etc/systemd/system
```text
2025-11-05 15:00 l /etc/systemd/system/multi-user.target.wants/pf_personal_webhook-lab.service
2025-11-05 19:09 f /etc/systemd/system/pf_personal_webhook-lab.service
2025-11-06 13:37 f /etc/systemd/system/invest-vs-dedupe.service
2025-11-06 13:37 f /etc/systemd/system/invest-vs-dedupe.timer
2025-11-06 18:10 l /etc/systemd/system/multi-user.target.wants/pf_invest_webhook-lab.service
2025-11-07 18:40 f /etc/systemd/system/pf_invest_webhook-lab.service
2025-11-07 21:52 d /etc/systemd/system/pf_invest_webhook-lab.service.d
2025-11-08 00:44 f /etc/systemd/system/pf_invest_webhook-lab.service.d/env.conf
2025-11-11 17:23 l /etc/systemd/system/timers.target.wants/git-autopush@home-ubuntu-lab-personal-repos-personal\x2dservices.timer
2025-11-11 17:49 f /etc/systemd/system/git-autopush@.timer
2025-11-11 18:47 f /etc/systemd/system/ssh-agent.service
2025-11-11 18:49 l /etc/systemd/system/default.target.wants/ssh-agent.service
2025-11-11 19:37 f /etc/systemd/system/git-autopush@.env
2025-11-11 21:48 f /etc/systemd/system/git-autopush@.service
```

## /etc/caddy
```text
2025-11-06 19:10 d /etc/caddy
2025-11-06 19:10 f /etc/caddy/Caddyfile
2025-11-07 13:35 f /etc/caddy/sites-enabled/dashboard.debet.credit.caddy.bak.1762518910
2025-11-07 13:47 d /etc/caddy/sites-enabled
2025-11-07 13:47 f /etc/caddy/sites-enabled/dashboard.debet.credit.caddy
2025-11-07 13:47 f /etc/caddy/sites-enabled/dashboard.debet.credit.caddy.bak.1762519657
```

## /etc/cron.d
```text
```

## /usr/local/bin
```text
```

## /usr/local/lib
```text
```

## /opt
```text
```

## Установленные Python-пакеты (pip)
```text
Babel==2.8.0
Brlapi==0.8.3
Flask==3.1.0
Jinja2==3.1.5
Mako==1.1.3
MarkupSafe==3.0.2
Pillow==9.0.1
PyGObject==3.42.1
PyJWT==2.3.0
PyNaCl==1.5.0
PyYAML==5.4.1
SecretStorage==3.3.1
Werkzeug==3.1.3
apturl==0.5.2
blinker==1.9.0
catfish==4.16.3
certifi==2020.6.20
cffi==1.15.0
chardet==4.0.0
click==8.1.8
colorama==0.4.4
cryptography==3.4.8
cupshelpers==1.0
dbus-python==1.2.18
defer==1.0.6
distro-info==1.1+ubuntu0.2
distro==1.7.0
httplib2==0.20.2
idna==3.3
importlib-metadata==4.6.4
itsdangerous==2.2.0
jeepney==0.7.1
keyring==23.5.0
language-selector==0.1
launchpadlib==1.10.16
lazr.restfulclient==0.14.4
lazr.uri==1.0.6
lightdm-gtk-greeter-settings==1.2.2
louis==3.20.0
macaroonbakery==1.3.1
menulibre==2.2.2
more-itertools==8.10.0
mugshot==0.4.3
oauthlib==3.2.0
olefile==0.46
onboard==1.4.1
pexpect==4.8.0
ply==3.11
protobuf==3.12.4
psutil==5.9.0
ptyprocess==0.7.0
pyOpenSSL==21.0.0
pyRFC3339==1.1
pycairo==1.20.1
pycparser==2.21
pycups==2.0.1
pyinotify==0.9.6
pymacaroons==0.13.0
pyparsing==2.4.7
python-apt==2.4.0+ubuntu4
python-dateutil==2.8.1
python-debian==0.1.43+ubuntu1.1
python-dotenv==0.19.2
pytz==2022.1
pyxdg==0.27
reportlab==3.6.8
requests==2.25.1
sgt-launcher==0.2.7
simplejson==3.17.6
six==1.16.0
ssh-import-id==5.11
systemd-python==234
ubuntu-drivers-common==0.0.0
ubuntu-pro-client==8001
ufw==0.36.1
unattended-upgrades==0.1
urllib3==1.26.5
wadllib==1.3.6
wheel==0.37.1
xcffib==0.11.1
xdg==5
xkit==0.0.0
zipp==1.0.0
```

## Установленные apt-пакеты (не системные)
```text
--fix-broken
--reinstall
-y
apache2-utils
cockpit
code
curl
docker-ce
firefox
mc
net-tools
python3
software-properties-common
tcpdump
tree
unbound
wireguard
wireguard-tools
xrdp
xubuntu-desktop
```

_Сгенерировано: 2025-11-12T19:18:06+01:00 — host: klichevs3.oblaka.tech_
