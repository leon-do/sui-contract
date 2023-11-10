# Source

https://docs.sui.io/guides/developer/app-examples/e2e-counter

# Sui Deplyoment

`./sui move build`

`./sui move test`

`./sui client new-address`

`./sui client active-address`

`./sui client switch --env https://fullnode.testnet.sui.io:443`

`./sui client gas`

`./sui client publish ./ --gas-budget 50000000`

```
./sui client publish ./ --gas-budget 50000000
UPDATING GIT DEPENDENCY https://github.com/MystenLabs/sui.git
INCLUDING DEPENDENCY Sui
INCLUDING DEPENDENCY MoveStdlib
BUILDING my_first_package
Successfully verified dependencies on-chain against source.
----- Transaction Digest ----
CvhhAvBJXLYPq6Pxp3a55e8fi4u7qxKoRMeVsz1ncz5Z
----- Transaction Data ----
Transaction Signature: [Signature(Ed25519SuiSignature(Ed25519SuiSignature([0, 18, 255, 240, 1, 109, 204, 248, 41, 220, 107, 160, 193, 39, 158, 237, 152, 52, 46, 113, 137, 232, 203, 125, 254, 120, 171, 168, 78, 251, 22, 158, 173, 251, 239, 100, 152, 120, 163, 207, 203, 129, 70, 160, 165, 65, 39, 50, 241, 93, 58, 131, 177, 108, 149, 153, 209, 218, 204, 223, 168, 87, 176, 58, 3, 37, 165, 40, 30, 201, 128, 86, 69, 217, 156, 82, 164, 116, 40, 234, 174, 219, 141, 203, 29, 204, 34, 221, 200, 255, 225, 28, 75, 194, 252, 143, 157])))]
Transaction Kind : Programmable
Inputs: [Pure(SuiPureValue { value_type: Some(Address), value: "0x8c9afd0e729bf440887d7fee283ec77a7dc1248d74c4d0cde78004f8a0a4f2ae" })]
Commands: [
  Publish(<modules>,0x0000000000000000000000000000000000000000000000000000000000000001,0x0000000000000000000000000000000000000000000000000000000000000002),
  TransferObjects([Result(0)],Input(0)),
]

Sender: 0x8c9afd0e729bf440887d7fee283ec77a7dc1248d74c4d0cde78004f8a0a4f2ae
Gas Payment: Object ID: 0x1b4b207dff82629bdeeba416aa8cef8c0fc6e4d4499037d786327010c4cb9c2a, version: 0xe8c68, digest: FRdvcK9Svq8Z6hpMwRkwjByknPcR5F6f7zTWBM4X5jqD
Gas Owner: 0x8c9afd0e729bf440887d7fee283ec77a7dc1248d74c4d0cde78004f8a0a4f2ae
Gas Price: 1000
Gas Budget: 50000000

----- Transaction Effects ----
Status : Success
Created Objects:
  - ID: 0x3fb54d96e46848e7150a55ec1ccf7bc8c2d7fd1b952e51b6104cd4ce8aa24806 , Owner: Account Address ( 0x8c9afd0e729bf440887d7fee283ec77a7dc1248d74c4d0cde78004f8a0a4f2ae )
  - ID: 0x5f1cbf91020e986d82493bbb8d0efab99c848d5e5fa1eec71faf2db725e2c5f7 , Owner: Immutable
Mutated Objects:
  - ID: 0x1b4b207dff82629bdeeba416aa8cef8c0fc6e4d4499037d786327010c4cb9c2a , Owner: Account Address ( 0x8c9afd0e729bf440887d7fee283ec77a7dc1248d74c4d0cde78004f8a0a4f2ae )

----- Events ----
Array []
----- Object changes ----
Array [
    Object {
        "type": String("mutated"),
        "sender": String("0x8c9afd0e729bf440887d7fee283ec77a7dc1248d74c4d0cde78004f8a0a4f2ae"),
        "owner": Object {
            "AddressOwner": String("0x8c9afd0e729bf440887d7fee283ec77a7dc1248d74c4d0cde78004f8a0a4f2ae"),
        },
        "objectType": String("0x2::coin::Coin<0x2::sui::SUI>"),
        "objectId": String("0x1b4b207dff82629bdeeba416aa8cef8c0fc6e4d4499037d786327010c4cb9c2a"),
        "version": String("953449"),
        "previousVersion": String("953448"),
        "digest": String("43pihmCXcYoYbVPPU3e6Yoo2k5PrY5Wo3qT2NR8nfCWa"),
    },
    Object {
        "type": String("created"),
        "sender": String("0x8c9afd0e729bf440887d7fee283ec77a7dc1248d74c4d0cde78004f8a0a4f2ae"),
        "owner": Object {
            "AddressOwner": String("0x8c9afd0e729bf440887d7fee283ec77a7dc1248d74c4d0cde78004f8a0a4f2ae"),
        },
        "objectType": String("0x2::package::UpgradeCap"),
        "objectId": String("0x3fb54d96e46848e7150a55ec1ccf7bc8c2d7fd1b952e51b6104cd4ce8aa24806"),
        "version": String("953449"),
        "digest": String("8zufSmPn1pVfDv8rjLMmcP3NyK7TEQpSCjXdPq2A7waQ"),
    },
    Object {
        "type": String("published"),
        "packageId": String("0x5f1cbf91020e986d82493bbb8d0efab99c848d5e5fa1eec71faf2db725e2c5f7"),
        "version": String("1"),
        "digest": String("HVyMNmx7ej9QguudRQLv5PU7KPPcbS8w5prEL2E9946h"),
        "modules": Array [
            String("counter"),
        ],
    },
]
----- Balance changes ----
Array [
    Object {
        "owner": Object {
            "AddressOwner": String("0x8c9afd0e729bf440887d7fee283ec77a7dc1248d74c4d0cde78004f8a0a4f2ae"),
        },
        "coinType": String("0x2::sui::SUI"),
        "amount": String("-8055080"),
    },
]
```

https://suiexplorer.com/txblock/CvhhAvBJXLYPq6Pxp3a55e8fi4u7qxKoRMeVsz1ncz5Z?deviceId=2fecdba4-6644-49ff-b157-9d4fe9e2b5e1&network=testnet