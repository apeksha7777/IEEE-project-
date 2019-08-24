# Run ganache
$ ganache-cli

# Migrate the contract
$ truffle migrate -reset

## Open the truffle console
$ truffle console

#### To create a contract instance:
> Election.deployed().then(function(i) { app=i; })

#### To display the details of candidate 1:
> app.candidates(1)

#### To create an instance of candidate mapping:
> app.candidates(1).then(function(c) { candidate=c; })

#### To display individual details of candidates
> candidate[0].toNumber()<br/>
> candidate[1]<br/>
> candidate[2].toNumber()

#### To vote candidate with candidateId = 1
> app.vote(1)

#### Vote with another account
> addr = (await web3.eth.getAccounts())[2]<br/>
> app.vote(2,{from: addr})

# Using the web interface

### Install lite-server
$ npm install lite-server

### Run ganache
$ ganache-cli

### Migrate the contracts
$ truffle migrate --reset

### Run the web interface
$ npm run dev

### Once the webpage is open
1. Go to the metamask extension and select accept address<br/>
2. Import accounts into metamask from ganache<br/>
    2.1 Copy the private key of the account you want to import from ganache<br/>
    2.2 Go to the metamask extension<br/>
    2.3 Choose import account<br/>
    2.4 Paste the private key and import<br/>
3. Change your account on metamask, reload browser and vote<br/>
