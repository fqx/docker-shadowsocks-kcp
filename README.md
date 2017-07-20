

#### Enable `BBR congestion control algorithm`
For one use kernel version `>= 4.9`, should enable `TCP_CONG_BBR` in your host os in order to get a better network performance (especially in high packet-loss situation).


#### Environments
Change these environments list below to apply new settings.

##### privoxy
Set `PORT` to an non-zero value to enable privoxy http proxy (only avaliable in client mode).

Env.         | Val.
-------------|--------
PORT         | 0

##### shadowsocks-libev
Shadowsocks with `-u (udp relay)`, `--fast-open (tcp fast-open)` enabled.

Env.         | Val.
-------------|--------
SS_PORT      |10800
SS_LOCAL_PORT|1080
SS_PASSWORD  |123456
SS_METHOD    |chacha20
SS_TIMEOUT   |600
SS_SERVER    |0.0.0.0

