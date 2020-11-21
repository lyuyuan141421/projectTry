pragma solidity ^0.4.0;

contract Helloworld {
         string Myname = "yuanlyu";
          
 function getName() public view returns(string)
 {
    return Myname;
 }

function changeName(string newName) public
{
    Myname = newName;
}
    
function pureTest(string _name) pure public returns(string)
{
  return _name;      
}


}
