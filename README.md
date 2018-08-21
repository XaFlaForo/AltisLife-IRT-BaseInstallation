<p>
<h3 align="center">Altis Life: IRT SeatBelts Installation</h3>
</p>
<h3> Synopsis:</h3>
To install any script with (IRT) in its name you must install this dependency first

<h3> Installation Guide</h3>

<b> Step 1: DOWNLOAD THE SEATBELTS FOLDER AND PUT IT IN THE ROOT OF YOUR MISSION </b>
<br/> 


<b> Step 2: GO TO IRT_Functions.hpp AND PASTE THE CODE IN </b>

<br/> 

class Belts { <br/> 
        file = "IRT\SeatBelts"; <br/> 
        class initbelts {}; <br/> 
        class seatbeltaction {}; <br/>  
        class seatbeltOff {}; <br/> 
        class seatbeltOn {}; <br/> 
}; <br/> 

<br/> 

<b> Step 3: GO TO fn_keyhandler AND PASTE THE CODE BELOW IN ALSO MAKE SURE NO OTHER HANDLER IS CASE 48  </b>

<br/> 

//--- B KEY <br/> 
    case 48: { <br/> 
        if (vehicle player != player) then { <br/> 
           [] spawn IRT_fnc_seatbeltaction; <br/> 
        }; <br/> 
    }; <br/> 

<br/> 


<br/> 
<b> Step 4: GO TO  AND PASTE THE CODE BELOW </b>

<br/> 
<br/> 
//--- SeatBelt <br/> 
[] spawn IRT_fnc_initbelts;
<br/> 

<br/> 

<b> Step 5: GO TO configuration.sqf AND PASTE THE CODE BELOW IN  </b>

<br/> 

IRT_SeatBelt = false;

## Copyright and License

Copyright (c) 2018 Ethan (XaLaForo), IRT Studios

### All code is licensed under the MIT license.

