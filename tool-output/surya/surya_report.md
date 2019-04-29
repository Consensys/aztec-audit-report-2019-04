## Sūrya's Description Report

### Files Description Table


|  File Name  |  SHA-1 Hash  |
|-------------|--------------|
| contracts/ZkAsset/ZkAsset.sol | 0a6283f060898d079e85713d89c4b92f41ce7c85 |
| contracts/ZkAsset/ZkAssetBurnable.sol | ff32633d2e65ebc6986d41b4e4aa54466e77c3ea |
| contracts/ZkAsset/ZkAssetDetailed.sol | c875d5fd628c34ec839d9338a10f4c0aed0237b0 |
| contracts/ZkAsset/ZkAssetMintable.sol | 51c88b89233c3719342b1fac067f22a66ba23838 |
| contracts/ZkAsset/ZkAssetOwnable.sol | 78d8faf458527c996110ddc59b8c32c0da96a50d |
| contracts/ZkAsset/ZkAssetOwnableTest.sol | f84212b030cb85e23ec42e83624c6795531074fc |
| contracts/ACE/validators/joinSplit/JoinSplit.sol | cbb6dc936ea50227b744d86a74689b4d62e7d836 |
| contracts/ACE/NoteRegistry.sol | 639a474f6dfdf68df06b03022c7488b738ba3f19 |
| contracts/ACE/ACE.sol | 2511c7d5184f3028b4c211a6d4e1f0a27a0df630 |
| contracts/ERC20/ERC20Mintable.sol | 18e55d340c7066f3d7e2fae22cb9b6fed8f3a1ab |
| contracts/libs/LibEIP712.sol | 27b1a46129272b6b4cc56e4c1ea4cd61220af6c2 |


### Contracts Description Table


|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **ZkAsset** | Implementation | IZkAsset, IAZTEC, LibEIP712 |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | |
| └ | confidentialTransfer | Public ❗️ | 🛑  |NO❗️ |
| └ | confidentialApprove | Public ❗️ | 🛑  |NO❗️ |
| └ | confidentialTransferFrom | Public ❗️ | 🛑  |NO❗️ |
| └ | confidentialTransferInternal | Internal 🔒 | 🛑  | |
| └ | logInputNotes | Internal 🔒 | 🛑  | |
| └ | logOutputNotes | Internal 🔒 | 🛑  | |
||||||
| **ZkAssetBurnable** | Implementation | ZkAssetOwnable |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | ZkAssetOwnable |
| └ | confidentialBurn | External ❗️ | 🛑  |NO❗️ |
||||||
| **ZkAssetDetailed** | Implementation | ZkAsset |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | ZkAsset |
||||||
| **ZkAssetMintable** | Implementation | ZkAssetOwnable |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | ZkAssetOwnable |
| └ | confidentialMint | External ❗️ | 🛑  |NO❗️ |
| └ | confidentialTransfer | Public ❗️ | 🛑  |NO❗️ |
||||||
| **ZkAssetOwnable** | Implementation | ZkAsset |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | ZkAsset |
| └ | setProofs | External ❗️ | 🛑  |NO❗️ |
| └ | confidentialTransferFrom | Public ❗️ | 🛑  |NO❗️ |
| └ | supportsProof | Public ❗️ |   |NO❗️ |
||||||
| **ZkAssetOwnableTest** | Implementation |  |||
| └ | setZkAssetOwnableAddress | Public ❗️ | 🛑  |NO❗️ |
| └ | callValidateProof | Public ❗️ | 🛑  |NO❗️ |
| └ | callConfidentialTransferFrom | Public ❗️ | 🛑  |NO❗️ |



|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **JoinSplit** | Implementation | LibEIP712 |||
| └ | \<Fallback\> | External ❗️ | 🛑  |NO❗️ |


|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **NoteRegistry** | Implementation | IAZTEC |||
| └ | supplementTokens | External ❗️ | 🛑  |NO❗️ |
| └ | validateProofByHash | Public ❗️ |   |NO❗️ |
| └ | createNoteRegistry | Public ❗️ | 🛑  |NO❗️ |
| └ | updateNoteRegistry | Public ❗️ | 🛑  |NO❗️ |
| └ | publicApprove | Public ❗️ | 🛑  |NO❗️ |
| └ | getRegistry | Public ❗️ |   |NO❗️ |
| └ | getNote | Public ❗️ |   |NO❗️ |
| └ | updateInputNotes | Internal 🔒 | 🛑  | |
| └ | updateOutputNotes | Internal 🔒 | 🛑  | |



|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **ACE** | Implementation | IAZTEC, Ownable, NoteRegistry |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | Ownable |
| └ | mint | External ❗️ | 🛑  |NO❗️ |
| └ | burn | External ❗️ | 🛑  |NO❗️ |
| └ | validateProof | External ❗️ | 🛑  |NO❗️ |
| └ | clearProofByHashes | External ❗️ | 🛑  |NO❗️ |
| └ | setCommonReferenceString | Public ❗️ | 🛑  |NO❗️ |
| └ | invalidateProof | Public ❗️ | 🛑  |NO❗️ |
| └ | validateProofByHash | Public ❗️ |   |NO❗️ |
| └ | setProof | Public ❗️ | 🛑  |NO❗️ |
| └ | incrementLatestEpoch | Public ❗️ | 🛑  |NO❗️ |
| └ | getCommonReferenceString | Public ❗️ |   |NO❗️ |
| └ | getValidatorAddress | Public ❗️ |   |NO❗️ |

|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **ERC20Mintable** | Implementation | ERC20 |||
| └ | mint | Public ❗️ | 🛑  |NO❗️ |


|  Contract  |         Type        |       Bases      |                  |                 |
|:----------:|:-------------------:|:----------------:|:----------------:|:---------------:|
|     └      |  **Function Name**  |  **Visibility**  |  **Mutability**  |  **Modifiers**  |
||||||
| **LibEIP712** | Implementation |  |||
| └ | \<Constructor\> | Public ❗️ | 🛑  | |
| └ | hashEIP712Message | Internal 🔒 |   | |
| └ | recoverSignature | Internal 🔒 |   | |


### Legend

|  Symbol  |  Meaning  |
|:--------:|-----------|
|    🛑    | Function can modify state |
|    💵    | Function is payable |


