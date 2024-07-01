![Alt Text](https://github.com/Winnode/Unit_Zero/raw/main/sc.png)


# Unix Winsnip

Unix Winsnip is a Python script for sending multiple Ethereum transactions using multiple accounts. Each account can send transactions concurrently using separate workers.

## Features

- Send Ethereum transactions using multiple accounts
- Randomized delays between transactions
- Customizable configurations via `config.json`
- Logs with timestamp, info, success, warning, and error levels
- Environment variable loading with `.env` support

## Installation

### Requirements

- Python 3.x
- Pip

### Download

```bash
git clone https://github.com/Winnode/Unit_Zero.git
```

### Dependencies

Install the required Python packages using pip:

```bash
pip install -r requirements.txt
```
or

```bash
pip install requests python-dotenv eth-account colorama pyfiglet
```

### Edit .env

```bash
mv .env_sampe .env
```

```bash
PRIVATE_KEY_1=PK1
PRIVATE_KEY_2=PK2
...
PRIVATE_KEY_N=PKN
```

### Edit Config.json

```bash
nano config.json
```


```bash
{
    "WAKTU_PENGIRIMAN": 5,
    "WAKTU_PENGULANGAN": 3,
    "MAKS_PENGULANGAN": 5,
    "JUMLAH_TRANSAKSI_PER_AKUN": 10,
    "BATAS_GAS": 21000,
    "HARGA_GAS": 1000000000,
    "URL_RPC": "https://rpc-testnet.unit0.dev",
    "ID_RANTAI": 88817,
    "JUMLAH_KIRIM": 0.0000000000001
}
```

### Run

```bash
python run.py
```

