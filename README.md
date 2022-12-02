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

![image](https://user-images.githubusercontent.com/52325658/205275502-98cf2988-123c-4868-9b88-30f7762fa75b.png)

In this coinDetails you have to set all the details for token name, token logo, token balance,and also token Id.

![image](https://user-images.githubusercontent.com/52325658/205275563-47876e5e-b1a7-402c-84ae-fae1d33d9eed.png)

NOTE: “Here you have to set your apikey(Which apikey you buy)”

This findkey()  you have send the two params to the this.gameInstance.sendMessage.


  PARAMS:

    1.  "GameManager",
    2.  "apiupdatekey"


In JSON.stringify you have to pass the which apikey you buy (eg):apikey: “YOUR APIKEY”, 

if the apikey is wrong you can’t play the game.then call the sendBalance() function.

      
      ![image](https://user-images.githubusercontent.com/52325658/205275633-87e4a73b-6f46-48d0-8edd-c19200fe783d.png)

This sendBalance()  you have send the two params to the this.gameInstance.sendMessage.

                                               1. "GameManager"             
                                         2.  "BalanceUpdate"


 In JSON.stringify you have to pass the coinDetails:this.conDetails.

![image](https://user-images.githubusercontent.com/52325658/205275723-70efa109-831a-4181-9bc5-bcb5dfd55078.png)


unity will send the actiontype=="isGameOver"  with the help of actiontype to check the calculation for both win and loss the game.
                         
      if won the game you have to calculate: 
                          
                     this.coinDetails[index].balance= (+coinbalance -betprice+payout)+ “ ”
		    
		    ![image](https://user-images.githubusercontent.com/52325658/205275818-9a511ebf-9a02-4ee8-830a-9a7215e4f04b.png)


if loss the game you have to  calculate:this.coinDetails[index].balance= (+coinbalance -betprice+payout)+ “ ”

    if you loss the game payout reward will add to  this.coinDetails[index].balance
           
	   ![image](https://user-images.githubusercontent.com/52325658/205275935-7b237b0f-88af-419f-94eb-c21ab3883b02.png)

Unity will sent the request unityObj.apikey == ‘request’ you have to call the this.findkey() function in it.

![image](https://user-images.githubusercontent.com/52325658/205276026-ee996f11-92e8-4827-81b3-83816c7fbb37.png)

checkDeviceType() is used to check a mobile view or web view, if the window inner width is less

than 600 then it’s a mobile view. Otherwise it’s a web view.
                                 
