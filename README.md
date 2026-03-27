# EtherReceiver.sol
How to deploy a contract on Base Chain
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract EtherReceiver {
    function getBalance() public view returns (uint) {
        return address(this).balance;
    }

    receive() external payable {}
}
