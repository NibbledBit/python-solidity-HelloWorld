# python-solidity-HelloWorld

In order to make this work a .env file must be added.

The file contains the Private Key for the my_address variable in the deploy.py script.
    
    export PRIVATE_KEY=f5640d642a44b02ee57eba4d0a3455e569f1435262349e7a919ac516043870

Once done, you must go into the deploy.py script and update the variable values:
    
    # testnet rinkeby env
    w3 = Web3(
        Web3.HTTPProvider("https://rinkeby.infura.io/v3/someapikey")
    )
    chain_id = 4
    my_address = "0x5b9EAaE5C190B773f889413B78121612341235123"
    private_key = os.getenv("PRIVATE_KEY")
