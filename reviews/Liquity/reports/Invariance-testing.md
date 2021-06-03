## Tools based  testing. 

## abstract : 

after understanding  the deploy sequence and vesting process  , i started  on  testing
    -  the liquidation logic  for property based testing  using Echidna 
    - Slither for  basic static testing  of whether best writing standards are being followed . 




## testing using Slither : 

- using StablityPool.sol for the entery point , we will try to detect the serious test coming :
    - method call msg.sender.call  {value: _amount} in '_sendETHGainToDepositor(uint256 _amount) internal' , here the call msg.sender  can be manipulated . given that its  being called in the contract with 'withdrawFromSP(uint _amount) external override' from 'provideToSP(uint _amount, address _frontEndTag) external override'.  
- now simple  checking that whether  RBAC is implemented in the 