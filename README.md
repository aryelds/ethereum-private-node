# Ethereum private node
How to create and initiate a private node using Ethereum Blockchain

![image](https://user-images.githubusercontent.com/8962452/54284641-16f79c00-457f-11e9-9d2f-e7c6dee95847.png)


## Installation
First of all you will need to install [Geth](https://geth.ethereum.org/downloads/)

## Create a new blockchain Genesis File using Puppeth

Just run on the terminal

```
$ puppeth
```

Choose the current values

![generateGenisis](https://user-images.githubusercontent.com/8962452/54286318-5f648900-4582-11e9-8e65-49d91d9cb7c8.png)

## Initialize the node

Now lets initialize the node with the Genesis file using the following Geth command.

```
geth --datadir . init .\MyNetWork.json
```

## Create new account

After initialize the node you should have a Geth directory ( this directory will store all the data for the chain ) and keystore directory ( this directory will store all the accounts )

You can create several accounts but the first account will receive the mining rewards. 

For create a new account just run

```
geth --datadir . account new
```

## List all the accounts

```
geth --datadir . account list
```

## Run the private node

Just run the command

```
./startprivatenode.sh
```

