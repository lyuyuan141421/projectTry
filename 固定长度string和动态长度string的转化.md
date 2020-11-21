pragma solidity ^0.4.0;

contract FixToDynmic
{
    bytes12 name = 0x3a43e231a3432e22;
    
    function fixBytesToDynmicBytes() view returns(bytes)
    {
       bytes memory newName = new bytes(name.length);
       
       for(uint i = 0; i < name.length; i++)
       {
           newName[i] = name[i];
       }
       
       return newName;
       
    }
}
