Abrimos un terminal y lanzamos:

    npx hardhat node

Abrimos un segundo terminal y lanzamos:

    npx hardhat run

Para desplegar en Mainnet/testnet:

    npx hardhat run scritps/simpleDeploy.js --network testnet

Para verificar el contrato, debemos instalar lo siguiente:

    "@nomiclabs/hardhat-etherscan"

Y lanzamos el comando de verificación:

    npx hardhat verify --network testnet 0x5FbDB2315678afecb367f032d93F642f64180aa3

En el archivo "hardhat.config.js" descomentar esto y cambiar el dato a la de ethereum, o rinkeby.

    // testnet: {
    //   url: "https://data-seed-prebsc-1-s1.binance.org:8545",
    //   chainId: 97,
    //   gasPrice: 20000000000,
    //   accounts: [privateKey]
    // }
    // ,
    // mainnet: {
    //   url: "https://bsc-dataseed.binance.org/",
    //   chainId: 56,
    //   gasPrice: 20000000000,
    //   accounts: [privateKey]
    // }
