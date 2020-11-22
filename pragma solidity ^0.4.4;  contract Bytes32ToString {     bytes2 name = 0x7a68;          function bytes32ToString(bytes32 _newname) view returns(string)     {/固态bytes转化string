pragma solidity ^0.4.4;

contract Bytes32ToString
{
    bytes2 name = 0x7a68;
    
    function bytes32ToString(bytes32 _newname) view returns(string)
    {
        // bytes memory newname = new bytes(_newname.length);
        uint count = 0;
        
        for(uint i = 0; i < _newname.length; i++)
        {
           bytes1 char = _newname[i];
           
           if (char != 0)
           {
               count++;
           }
        }
        
    bytes memory newname = new bytes(count);
    
    for(uint j = 0; j < count; j++)
    {
        newname[j] = _newname[j];
    }
    
    return string(newname);
    }
}
