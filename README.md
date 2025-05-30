
# setup tools
1. Go [here](https://docs.docker.com/get-docker/) to install Docker
2. Go [here](https://docs.kurtosis.com/install/) to install Kurtosis

# start up
```Shell
kurtosis run --enclave reth github.com/ethpandaops/ethereum-package --args-file ./network_params.yml
```

get rpc for executor layer:
```Shell
kurtosis port print local-reth el-1-reth-lighthouse rpc
```

# remove
```Shell
kurtosis enclave stop reth
kurtosis enclave rm reth
```

# reference
https://reth.rs/run/private-testnet.html