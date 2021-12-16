# Marinade Finance on-chain CPI helper

This Rust lib will simplify integrating CPI calls by giving out the structure account and invoke signed function

## Usage

add to your .toml file

```
marinade-onchain-helper = { git = "https://github.com/marinade-finance/liquid-staking-onchain-sdk" }
```

Add to the begining of your file use (remove unused functions):

```
use marinade_onchain_helper::{
    cpi_context_accounts::{
        MarinadeDeposit, 
        MarinadeDepositStakeAccount, 
        MarinadeLiquidUnstake
    },
    cpi_util::{
        invoke_signed,
    }
};
```
