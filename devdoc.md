{
	"methods": {
		"allowance(address,address)": {
			"details": "Function to check the amount of tokens that an owner allowed to a spender.",
			"params": {
				"owner": "address The address which owns the funds.",
				"spender": "address The address which will spend the funds."
			},
			"return": "A uint256 specifying the amount of tokens still available for the spender."
		},
		"approve(address,uint256)": {
			"details": "Approve the passed address to spend the specified amount of tokens on behalf of msg.sender. Beware that changing an allowance with this method brings the risk that someone may use both the old and the new allowance by unfortunate transaction ordering. One possible solution to mitigate this race condition is to first reduce the spender's allowance to 0 and set the desired value afterwards: https://github.com/ethereum/EIPs/issues/20#issuecomment-263524729",
			"params": {
				"spender": "The address which will spend the funds.",
				"value": "The amount of tokens to be spent."
			}
		},
		"balanceOf(address)": {
			"details": "Gets the balance of the specified address.",
			"params": {
				"owner": "The address to query the balance of."
			},
			"return": "An uint256 representing the amount owned by the passed address."
		},
		"decimals()": {
			"return": "the number of decimals of the token."
		},
		"decreaseAllowance(address,uint256)": {
			"details": "Decrease the amount of tokens that an owner allowed to a spender. approve should be called when allowed_[_spender] == 0. To decrement allowed value is better to use this function to avoid 2 calls (and wait until the first transaction is mined) From MonolithDAO Token.sol Emits an Approval event.",
			"params": {
				"spender": "The address which will spend the funds.",
				"subtractedValue": "The amount of tokens to decrease the allowance by."
			}
		},
		"increaseAllowance(address,uint256)": {
			"details": "Increase the amount of tokens that an owner allowed to a spender. approve should be called when allowed_[_spender] == 0. To increment allowed value is better to use this function to avoid 2 calls (and wait until the first transaction is mined) From MonolithDAO Token.sol Emits an Approval event.",
			"params": {
				"addedValue": "The amount of tokens to increase the allowance by.",
				"spender": "The address which will spend the funds."
			}
		},
		"name()": {
			"return": "the name of the token."
		},
		"symbol()": {
			"return": "the symbol of the token."
		},
		"totalSupply()": {
			"details": "Total number of tokens in existence"
		},
		"transfer(address,uint256)": {
			"details": "Transfer token for a specified address",
			"params": {
				"to": "The address to transfer to.",
				"value": "The amount to be transferred."
			}
		},
		"transferFrom(address,address,uint256)": {
			"details": "Transfer tokens from one address to another. Note that while this function emits an Approval event, this is not required as per the specification, and other compliant implementations may not emit the event.",
			"params": {
				"from": "address The address which you want to send tokens from",
				"to": "address The address which you want to transfer to",
				"value": "uint256 the amount of tokens to be transferred"
			}
		}
	},
	"title": "SimpleToken\r"
}
