# uniswap

class uniswap.Uniswap(address: Optional[Union[Address, ChecksumAddress, str]], private_key: Optional[str], provider: Optional[str] = None, web3: Optional[web3.main.Web3] = None, version: int = 1, default_slippage: float = 0.01, use_estimate_gas: bool = True, factory_contract_addr: Optional[str] = None, router_contract_addr: Optional[str] = None, enable_caching: bool = False)
Wrapper around Uniswap contracts.

Parameters
address – The public address of the ETH wallet to use.

private_key – The private key of the ETH wallet to use.

provider – Can be optionally set to a Web3 provider URI. If none set, will fall back to the PROVIDER environment variable, or web3 if set.

web3 – Can be optionally set to a custom Web3 instance.

version – Which version of the Uniswap contracts to use.

default_slippage – Default slippage for a trade, as a float (0.01 is 1%). WARNING: slippage is untested.

factory_contract_addr – Can be optionally set to override the address of the factory contract.

router_contract_addr – Can be optionally set to override the address of the router contract (v2 only).

enable_caching – Optionally enables middleware caching RPC method calls.
