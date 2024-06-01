# Token-solana
token Bitcash del proyecto Alena, by Hpe Unidad de negocios y Data Ing Blockchain


Cualquier creacion y/o 
bifurcación de nuestro token realizado desde este creador de token no tendra valor comercial ni podra ser considerado un token activo de la cadena bitcash by HPE DIV.Empresariales de Ing Blockchain
Smart Contract
// SPDX-License-Identifier: GPL-3.0

pragma solidity ^0.5.9;

import "@0x/contracts-erc20/contracts/src/ERC20Token.sol";

/**
 * @title SampleERC20
 * @dev Create a sample ERC20 standard token
 */
contract SampleERC20 is ERC20Token {

    string pub;
    string public symbol;
    uint256 public decimals;

    constructor (
        string memory,,
        string memory _symbol,
        uint256 _decimals,
        uint256 _totalSupply
    )
        public
    {
        name = _name;
        symbol = _symbol;
        decimals = _decimals;
        _totalSupply = _totalSupply;
        balances[msg.sender] = _totalSupply;
    }
}
este es un Creador de tokens  basado en la plataforma del ecosystem de Solana
El objetivo principal de este repositorio es ayudar a experimentar con el proceso de creación de tokens de Solana sin profundizar demasiado en los detalles.

Intenté hacerlo lo más intuitivo posible ya que hay muchos matices en comparación con las cadenas de bloques EVM.

El proyecto se basa en la plantilla dapp de Solana ; todas las instrucciones para ejecutar el proyecto localmente se pueden encontrar allí   https://github.com/solana-labs/dapp-scaffold     . Inspirado en el creador del token de Jacob.

La aplicación está implementada en vercel. Enlace .directo a Solana https://github.com/exitatmosphere/Solana-Token-Creator
