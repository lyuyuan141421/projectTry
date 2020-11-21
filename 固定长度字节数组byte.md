pragma solidity ^0.4.0;

contract ByteArray
{
    bytes1 public num1 = 0x7a;
    bytes2 public num2 = 0x7a68;
    bytes12 public num3 = 0x7a686464335a324e;
    
    function getlength1() returns(uint)
    {
        return num1.length;
    }
    
    function getlength2() returns(uint)
    {
        return num2.length;
    }

function getlength3() returns(uint)
    {
        return num3.length;
    }

}
