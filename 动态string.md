pragma solidity ^0.4.0;

contract DynamicString
{
    string name = "lyuyuan";
    
    function getLength() view returns(uint)
    {
        return bytes(name).length;
    }
    
    function changeName() view returns(bytes1)
    {
        return bytes(name)[0];
    }
    
    function getName() view returns(bytes)
    {
        return bytes(name);
    }
    
     function changeName_2()
    {
        bytes(name)[0] = "X";
    }
    
}
