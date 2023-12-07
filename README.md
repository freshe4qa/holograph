<p align="center">
  <img height="100" height="auto" src="https://github.com/freshe4qa/holograph/assets/85982863/36db333e-46eb-47b9-bb00-71f5801da0eb">
</p>

# Holograph - Testnet

Official documentation:
>- [Guide](https://docs.holograph.xyz/developer/cli/quick-start-cli)

Explorer:
>- [Explorer](-)

### Minimum Hardware Requirements
 - 2x CPUs; the faster clock speed the better
 - 2GB RAM
 - 40GB of storage (SSD or NVME)
 - Ubuntu 20.04

```
sudo apt update && sudo apt upgrade -y
```

```
apt install curl iptables build-essential git wget jq make gcc nano tmux htop nvme-cli pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev -y
```
```
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash -
```
```
apt install nodejs -y
```

Для запуска ноды рекомендуется использовать новый кошелек Metamask.
Создав новый кошелек, сохраняем адрес и закрытый ключ.
Нам понадобится тестовый $AVAX в сети Avalanche Fuji.

```
npm install -g @holographxyz/cli
```

```
holograph config
```

Выбираем fuji, жмем space для выбора, затем enter.
Далее enter, мы будем использовать стандартный RPC.
Вставляем private key кошелька.
Придумываем пароль.

```
holograph faucet
```

Пишем y.
Вводим пароль.
Нажимаем enter, чтобы выбрать сеть fuji.

```
screen -S holo
```
```
holograph operator:bond
```

Пишем y.
Вводим пароль.
Выбираем fuji, enter.
Выбираем 200, enter.
Пишем 200 и enter.
Пишем y.
Пишем y.
Вводим пароль.

Выйти со скринера CTRL + A + D

Сейчас минимум токенов $HLG нужно 200, чтобы запустить оператора. Через 24ч возвращаемся к крану "holograph faucet" и запрашиваем токены. Далее уже можно запустить валидатора.
