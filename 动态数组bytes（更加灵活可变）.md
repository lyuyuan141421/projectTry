pragma solidity ^0.4.0;

contract DynamicByte
{
    bytes public name = new bytes(2);  // create dynamic byte, 2 bytes
    
    function InitName()
    {
        name[0] = 0x7a;      // get first byte
        name[1] = 0x68;      // get second byte
        
    }
    
    function getLength() view returns(uint)
    {
        return name.length;
    }
    
    function changeName()       // bytes value can be changed 
    {
        name[0] = 88;
    }
    
    function changeLength()    // length can be changed
    {
        name.length = 5;
    }
    
    function pushtest()
    {
        name.push(0x99);       // add value into dynamic bytes, length also changed
    }
    
}
