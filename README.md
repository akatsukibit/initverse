![image](https://github.com/user-attachments/assets/35e841fa-a227-432a-bb05-0005e63d796a)

# Initchain Node : 

## req. : 

Minimum : 

- ∞ CPU+ / ∞ GB RAM /  ∞ MBit/sec 

## Lets Go ; 

Update first:

```bash
sudo apt update -y && sudo apt upgrade -y
```
## 2. need this packages:

```bash
sudo apt install htop ca-certificates zlib1g-dev libncurses5-dev libgdbm-dev libnss3-dev tmux iptables curl nvme-cli git wget make jq libleveldb-dev build-essential pkg-config ncdu tar clang bsdmainutils lsb-release libssl-dev libreadline-dev libffi-dev jq gcc screen unzip lz4 -y
```
## 3. Download the Miner:

```bash
curl -L -O https://github.com/Project-InitVerse/miner/releases/download/v1.0.0/iniminer-linux-x64
```

#### autorize : 

```bash
chmod +x iniminer-linux-x64
```

## 4.  set on Screen : 

```bash
screen -S init
```

## 5. Let's Do the Tuning - WARNING We recommend you do what the kernels are tuned for. 
#### When you want to stop, just press CTRL C and it will stop. 

- 0x0304f5193FCe6A27e3789c27EE2B9D95177e21A5 this is a random wallet, write your own wallet address instead
- Worker001 is the name you gave to the server, you can change it differently if you want, MyServer1 is an example.

##### Use all CPU : 

```bash
./iniminer-linux-x64 --pool stratum+tcp://0x0304f5193FCe6A27e3789c27EE2B9D95177e21A5.Worker001@pool-core-testnet.inichain.com:32672 
```
![image](https://github.com/user-attachments/assets/c1dd2098-a6a5-49a7-90cb-9ce42b7b8307)


##### If you wish, you can set it to be loaded on the cores. For example, the command below is to use 1 thread.  --cpu-devices :

```bash
./iniminer-linux-x64 --pool stratum+tcp://0x0304f5193FCe6A27e3789c27EE2B9D95177e21A5.Worker001@pool-core-testnet.inichain.com:32672 --cpu-devices 1
```

#### To set Multi CPU, you can add --cpu-devices, for example for 4 Threads - in short, we write for each core and increase the number : 

```bash
./iniminer-linux-x64 --pool stratum+tcp://0x0304f5193FCe6A27e3789c27EE2B9D95177e21A5.Worker001@pool-core-testnet.inichain.com:32672 --cpu-devices 1 --cpu-devices 2 --cpu-devices 3 --cpu-devices 4 
```

![image](https://github.com/user-attachments/assets/c5b535eb-47c8-4cc7-9167-9851438b18f4)

For example, he uses it like this in 9's : 

![image](https://github.com/user-attachments/assets/6ace2e49-9970-4f5d-b620-8d610ac13637)


#### When it works, the example will look like this:

![image](https://github.com/user-attachments/assets/bbbcd5ca-7660-4704-92e1-633d2c90b65f)

#### CTRL A + D ile screenden çalışmayı durdurmadna rahatlıkla çıkabilirsiniz.

## Check your Wallet how much you Earned INI coin. THE TESTNET COINS WILL BE AIRDROPED ON THE MAINNET 1:1! : 

- Link : https://genesis-testnet.yatespool.com/ 

- put your walletadress & press the Search button
