# eth-vanity-gen

NodeJS vanity ethereum address generator


## What is a vanity address?

A vanity address is an address that is personalized and is created respecting a series of parameters.

Examples: 
- `0x0000c3Caa36E2d9A8CD5269C976eDe05018f0000`
- `0x12345678a36E2d9A8CD5269C976eDe05018fa36E`
- `0xdead5678a36E2d9A8CD5269C976eDe05018fa36E`

## Usage

clone from github
``` 
git clone  https://github.com/d3or/eth-vanity-gen.git
```
Install dependencies

```
npm install
```

Setup config.json

```
{
    "prefix": "000", // beginning characters
    "suffix": "000", // end characters
    "cores":0 // set to 0 to automatically detect core count
}
```
Run
```
npm start
```

public/private address key pairs are outputed to `eth_wallet_list.txt` in the form of `public,private`

The time to generate an address matching the prefix and suffix depends on the length of `prefix + suffix`. As the length increases it takes exponentially longer to generate a matching address.




## Security

Nothing leaves your machine, and everything is done offline.

## Performance

Performance depends on core speed and core count. The more cores you have, the faster you will generate wallets.

Maxing out your core count will make your computer pretty unusable, so set it to like half of your total if you want to use your computer at the same time.


## Tips

`0x0000c3Caa36E2d9A8CD5269C976eDe05018f0000`
