Rust Installation:

curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh

(1'i seçip enter)


Foundry Installation:

curl -L https://foundry.paradigm.xyz | bash
source ~/.bashrc
foundryup
cast --version


Installing OpenSSL and pkg-config:

sudo apt update && sudo apt install pkg-config libssl-dev


Import the address you want (preferably a burner address) Make sure it contains Holesky Eth:

[ -d ~/.aligned_keystore ] && rm -rf ~/.aligned_keystore && echo "Deleted existing directory ~/.aligned_keystore." ; mkdir -p ~/.aligned_keystore && cast wallet import ~/.aligned_keystore/keystore0 --interactive



To pull the Aligned Layer Repo:

[ -d aligned_layer ] && rm -rf aligned_layer && echo "Deleted existing aligned_layer directory." ; git clone https://github.com/yetanotherco/aligned_layer.git && cd aligned_layer/examples/zkquiz


Last command:


make answer_quiz KEYSTORE_PATH=~/.aligned_keystore/keystore0



At this stage, you will be asked some questions and the answers are as follows: C, C, A


