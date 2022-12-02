                                            PROJECT NAME: OSIZ-DICE

PROJECT URL : https://cryptowalletapi.io/

 
OVERVIEW: 

               First you have to  purchase your apikey through this link  https://cryptowalletapi.io/games/

then you can download a build file.

REGISTER:

                   If you are a new user you have to register. You have to fill  all the required

 fields,otherwise you have to login.


                     Register Link :  https://cryptowalletapi.io/

                     Login Link    :  https://cryptowalletapi.io/login/


WORKINGFLOW:

Once your payment is completed. It shows a Game Api Keys option show in your page.

In this page your APIKEY generated successfully.



In this coinDetails you have to set all the details for token name, token logo, token balance,and also token Id.






NOTE: “Here you have to set your apikey(Which apikey you buy)”

This findkey()  you have send the two params to the this.gameInstance.sendMessage.


  PARAMS:

    1.  "GameManager",
    2.  "apiupdatekey"


In JSON.stringify you have to pass the which apikey you buy (eg):apikey: “YOUR APIKEY”, 

if the apikey is wrong you can’t play the game.then call the sendBalance() function.

      






This sendBalance()  you have send the two params to the this.gameInstance.sendMessage.

                                               1. "GameManager"             
                                         2.  "BalanceUpdate"


 In JSON.stringify you have to pass the coinDetails:this.conDetails.

                                 


													
  unity will send the actiontype=="isGameOver"  with the help of actiontype to check the calculation for both win and loss the game.
                         
      if won the game you have to calculate: 
                          
                     this.coinDetails[index].balance= (+coinbalance -betprice+payout)+ “ ”



    if loss the game you have to  calculate:


                    this.coinDetails[index].balance= (+coinbalance -betprice+payout)+ “ ”

    if you loss the game payout reward will add to  this.coinDetails[index].balance
           




Unity will sent the request unityObj.apikey == ‘request’ you have to call the this.findkey() function in it.



 




checkDeviceType() is used to check a mobile view or web view, if the window inner width is less

than 600 then it’s a mobile view. Otherwise it’s a web view.
