pragma solidity ^0.4.0;

contract ByteArray
{
    bytes1 public num1 = 0x7a;
    bytes1 public num2 = 0x68;
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

 function bijiao1() returns(bool)
 {
     return num1 > num2;
 }

 function bijiao2() returns(bool)
 {
     return num1 < num2;
 }
 
 function bijiao3() returns(bool)
 {
     return num1 != num2;
 }
 
 function weiyu() view public returns (bytes1)
    {
        return num1 & num2;
    }

     function weihuo() view public returns (bytes1)
    {
        return num1 | num2;
    }

     function weiyihuo() view public returns (bytes1)
    {
        return num1 ^ num2;
    }

    function weifan() view public returns (bytes1)
    {
        return ~num1;
    }

     function weizuoyi() view public returns (bytes1)
    {
        return num1 << 1;
    }

     function weiyouyi() view public returns (bytes1)
    {
        return num1 >> 1;
    }
 
 
}
