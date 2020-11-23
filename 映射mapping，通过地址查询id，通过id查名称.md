pragma solidity ^0.4.0;

contract mappingTest   // yi yi dui ying
{
    mapping(address => uint) idMapping;       // id
    mapping(uint => string)  nameMapping;
    
    uint public sum = 0;      // zhu ce de zong liang
    
    function register(string name)
    {
        address account = msg.sender;  // huo de dang qian  he yue de diao yong zhe 
        
        sum++;
        idMapping[account] = sum;    // di zhi he zhu ce zong liang id lian xi dao yiqi
        nameMapping[sum] = name;     // id zong liang he ming zi bang ding dao yiqi
    }
    
    function getIdByAddress(address are) view returns(uint)   //  tong guo di zhi huo de id 
    {
        return idMapping[are];
    }
    
     function getNameById(uint Id) view returns(string)   // tong guo id huo de ming zi
    {
        return nameMapping[Id];
    }
    
}
