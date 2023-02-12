<p align="center">
  <img height="100" height="auto" src="https://raw.githubusercontent.com/Nodeist/Kurulumlar/main/logos/blockx.png">
</p>


# Blockx Live Peers
Here is a list of active peers. Add them to your `config.toml` if you have trouble finding peers.
```
23b12388a6922cb3bb7b72b8b7cc7429b7444f80@142.93.3.163:26656,85f8e76274cb95d9dde3487d5b8547be27f58192@167.99.12.133:26656,6b0f6f7871beb1b16e3d306362bf17932c7268e8@192.241.149.124:26656,d7206cb001a85c9c7437f1f9c798ac6aef474cea@159.223.101.23:26656,8807db839efe14a9cd1b5b76ee5beac4f14bd622@104.248.249.90:26656,aefb7fa893e8218937b2094ffe4df18b76d19680@91.229.23.155:26656,3a36a796162153a6ef2a9f0fd56198b6c4870157@159.89.52.0:26656,0780cc4348dc8640a35467d73720c77e15a0e839@208.68.39.230:26656,f997153b25637ed58924994d7a168cb38a3f7602@4.193.55.49:26656,93208b250758151f8fe3408c09592bc0317297a0@85.239.238.220:26656,ce99a0050f5f92303eb2b384c62123b0cc1fff84@85.239.241.145:26656,68040a4e2a34a5cab55874fe7df0b422c0d24efd@164.92.129.182:26656,ba5ae81a368fea92f34699734bb344afdd337377@139.162.60.43:30656
```

Here is a script for you to update `persistent_peers` setting with these peers in `config.toml`.

```
PEERS=23b12388a6922cb3bb7b72b8b7cc7429b7444f80@142.93.3.163:26656,85f8e76274cb95d9dde3487d5b8547be27f58192@167.99.12.133:26656,6b0f6f7871beb1b16e3d306362bf17932c7268e8@192.241.149.124:26656,d7206cb001a85c9c7437f1f9c798ac6aef474cea@159.223.101.23:26656,8807db839efe14a9cd1b5b76ee5beac4f14bd622@104.248.249.90:26656,aefb7fa893e8218937b2094ffe4df18b76d19680@91.229.23.155:26656,3a36a796162153a6ef2a9f0fd56198b6c4870157@159.89.52.0:26656,0780cc4348dc8640a35467d73720c77e15a0e839@208.68.39.230:26656,f997153b25637ed58924994d7a168cb38a3f7602@4.193.55.49:26656,93208b250758151f8fe3408c09592bc0317297a0@85.239.238.220:26656,ce99a0050f5f92303eb2b384c62123b0cc1fff84@85.239.241.145:26656,68040a4e2a34a5cab55874fe7df0b422c0d24efd@164.92.129.182:26656,ba5ae81a368fea92f34699734bb344afdd337377@139.162.60.43:30656
sed -i.bak -e "s/^persistent_peers *=.*/persistent_peers = \"$PEERS\"/" $HOME/.blockxd/config/config.toml
```