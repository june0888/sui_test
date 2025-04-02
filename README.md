# SUI setting

	sudo apt-get install curl git-all cmake gcc libssl-dev pkg-config libclang-dev libpq-dev build-essential

	cargo install --locked --git https://github.com/MystenLabs/sui.git --branch testnet sui --features tracing

	sh -c "$(curl -fsSL https://raw.githubusercontent.com/Linuxbrew/install/master/install.sh)"
	touch ~/.zshrc
	vim ~/.zshrc

Add the following code to your .zshrc file.

	export PATH="/home/linuxbrew/.linuxbrew/bin:$PATH"
	export MANPATH="/home/linuxbrew/.linuxbrew/share/man:$MANPATH"
	export INFOPATH="/home/linuxbrew/.linuxbrew/share/info:$INFOPATH"

Before running SUI, you should enter the following code.

	source ~/.zshrc

for adding Testnet for SUI,

	sui client new-env --alias testnet --rpc https://fullnode.testnet.sui.io:443

for checking your address, please enter 

	sui keytool list

You can request SUI at https://faucet.sui.io/?network=testnet

If you get SUI, you can confirm that you get SUI.

	sui client gas



