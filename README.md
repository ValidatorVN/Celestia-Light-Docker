# Celestia-Light&Full-Docker

1/ Update hệ thống:

    sudo apt update && apt upgrade -y
    
2/ Cài Docker:

    apt install docker.io -y
    
3/ Chạy node: sửa IP address => địa chỉ VPS của bạn.

Dành cho chạy Light node:

    docker run -e NODE_TYPE=light -e P2P_NETWORK=blockspacerace ghcr.io/celestiaorg/celestia-node:v0.7.2 celestia light start --core.ip IP_ADDRESS --gateway --gateway.addr 127.0.0.1 --gateway.port 26659 --p2p.network mocha
    
Dành cho chạy Full node:

    docker run -e NODE_TYPE=full -e P2P_NETWORK=blockspacerace ghcr.io/celestiaorg/celestia-node:v0.7.2 celestia full start --core.ip IP_ADDRESS --gateway --gateway.addr 127.0.0.1 --gateway.port 26659 --p2p.network mocha
    
4/ Lưu thông tin ví lại, sẽ có dạng:

    NAME: my_celes_key
    ADDRESS: celestia1j3g6tw7jx9etf5etpesrrz8szh52l2gmyw2e23
    MNEMONIC (save this somewhere safe!!!): 
    range boat pencil usage recipe naive mesh wife vault travel section stone awesome virus involve life shadow silent quality gold crystal
    
5/ Faucet token vào ví trên, Done.

    Cộng đồng chạy Node & Validator VietNam, nơi thảo luận và chia sẻ kinh nghiệm về chạy node/validator, không bàn luận chính trị.
    Chanel: https://t.me/RunnodeVietNamese
    Youtube: https://www.youtube.com/@nodevalidatorvietnam
    Telegram: https://t.me/NodeValidatorVietNam
