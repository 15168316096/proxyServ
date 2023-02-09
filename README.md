# proxyServ

## mock eth-light-client
python -m proxyserver 

## example
```
guopenglin@MacBook-Pro-4 ~ % curl https://www.lightclientdata.org/eth/v1/beacon/headers/5745928
{"execution_optimistic":true,"data":{"root":"0x0cda06740f50dc05b763073078e8ad9e0794ba4ecbfe0d16e42938d85c43db59","canonical":true,"header":{"message":{"slot":"5745928","proposer_index":"371154","parent_root":"0xa5301a40cc81be37fbddaf4f8edd7f53190314f7b154b020ee91a5f6799575c8","state_root":"0xbf29e05faf4899d2e142c4b48af73e6228a3c89a11541c82acfa39a25d6d22cd","body_root":"0xe6684371c8923859475d0a02ca14f637e7353c253f9a6438cdcc52a64d64379c"},"signature":"0xb4ec471b9a770ad78671e783c45e4e9d4ba10a24abab06d604ef1969471fa5824a56947cc91093b7ee21b6dbb0ba436c12de0181da961e2730c4852b816393df044b97feb9a072685a6c4bf24ef08e584517a7b5aab865f51b7e6b7e6064aadc"}}}%                                                                  
guopenglin@MacBook-Pro-4 ~ % curl http://localhost:8080/eth/v1/beacon/headers/5745928
{"execution_optimistic":true,"data":{"root":"0x0cda06740f50dc05b763073078e8ad9e0794ba4ecbfe0d16e42938d85c43db59","canonical":true,"header":{"message":{"slot":"5745928","proposer_index":"371154","parent_root":"0xa5301a40cc81be37fbddaf4f8edd7f53190314f7b154b020ee91a5f6799575c8","state_root":"0xbf29e05faf4899d2e142c4b48af73e6228a3c89a11541c82acfa39a25d6d22cd","body_root":"0xe6684371c8923859475d0a02ca14f637e7353c253f9a6438cdcc52a64d64379c"},"signature":"0xb4ec471b9a770ad78671e783c45e4e9d4ba10a24abab06d604ef1969471fa5824a56947cc91093b7ee21b6dbb0ba436c12de0181da961e2730c4852b816393df044b97feb9a072685a6c4bf24ef08e584517a7b5aab865f51b7e6b7e6064aadc"}}}```
