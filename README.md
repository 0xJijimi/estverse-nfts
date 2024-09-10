## Estverse NFTs

The EstverseNFTs contract is an ERC1155 token implementation with the following features:

- Minting of NFTs with dynamic pricing
- Royalty support (ERC2981)
- Pausable functionality
- Token locking/unlocking
- Ownable with withdrawal function

### Key Functions:

- `mint(uint256 id)`: Mint an NFT
- `setTokenUnlock(uint256 id, bool unlocked, uint256 basePrice)`: Set token availability and base price
- `withdraw(address _addr)`: Withdraw contract balance to specified address

## Usage

### Deploy

```
forge create EstverseNFTs --rpc-url <testnet-or-mainnet-url> --constructor-args <initialOwnerAddress> --interactive
```
