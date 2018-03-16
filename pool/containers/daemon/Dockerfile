FROM blakelapierre/xtlpool-base

VOLUME daemon-data

CMD cd coin/bin && ./stellited --data-dir /daemon-data --rpc-bind-port 8888 --rpc-bind-ip 0.0.0.0 --confirm-external-bind --non-interactive