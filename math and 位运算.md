pragma solidity ^0.4.0;

contract math
{
    // int(positive and negtive) uint(just positive)
    
    uint num1 = 100;    // int256 == int
    uint num2 = 200;    // uint256 == int
    
    function add(uint num1, uint num2) pure public returns (uint)
    {
        return num1 + num2;
    }
    
     function jian(uint num1, uint num2) pure public returns (uint)
    {
        return num1 - num2;
    }
    
     function chen(uint num1, uint num2) pure public returns (uint)
    {
        return num1 * num2;
    }
    
     function chu(uint num1, uint num2) pure public returns (uint)
    {
        return num1 / num2;
    }
    
     function yushu(uint num1, uint num2) pure public returns (uint)
    {
        return num1 % num2;
    }
    
    function pingfang(uint num1, uint num2) pure public returns (uint)
    {
        return num1 ** num2;
    }
    
    uint8 a = 3;
    uint8 b = 4;
    
     function weiyu() view public returns (uint)
    {
        return a & b;
    }
    
     function weihuo() view public returns (uint)
    {
        return a | b;
    }
    
     function weiyihuo() view public returns (uint)
    {
        return a ^ b;
    }
    
    function weifan() view public returns (uint)
    {
        return ~a;
    }
    
     function weizuoyi() view public returns (uint)
    {
        return a << 1;
    }
    
     function weiyouyi() view public returns (uint)
    {
        return a >> 1;
    }
    
}
