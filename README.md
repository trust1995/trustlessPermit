## Rationale
The ERC20 `permit()` extension suffers from a significant design oversight. When contracts call `permit()` they must always take into account it may revert because of a frontrunning attack. More info is available at the [Trust Security blog](https://www.trust-security.xyz/post/permission-denied). 

## TrustlessPermit
Consider using the `trustlessPermit()` function in this library if the intention is to continue execution when the user allowance is sufficient (As if the `permit()` executed successfully)

## Disclaimer
The code in this repo is provided as-is, with no warranty whatsoever. The user takes all responsibility and risks associated with using this library.

## Credit
[Trust Security](https://trust-security.xyz/)
