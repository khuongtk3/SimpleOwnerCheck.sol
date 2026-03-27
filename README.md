# SimpleOwnerCheck.sol
Contract deployed via Web3 SimpleOwnerCheck.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SimpleOwnerCheck {
    address public owner;

    constructor() {
        owner = msg.sender;
    }

    function isOwner() public view returns (bool) {
        return msg.sender == owner;
    }
}
