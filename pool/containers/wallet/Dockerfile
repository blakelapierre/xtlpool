FROM blakelapierre/xtlpool-base

EXPOSE 8070
VOLUME daemon-data
VOLUME wallet-data

CMD cd coin/bin && if [ ! -f /wallet-data/container ]; then ./stellite-wallet-rpc --data-dir /wallet-data -g -w /wallet-data/container; fi; ./walletd --daemon-address xtlpool-daemon --daemon-port 11898 --data-dir /wallet-data -w /wallet-data/container