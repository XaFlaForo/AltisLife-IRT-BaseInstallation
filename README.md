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

class Belts {
        file = "IRT\SeatBelts";
        class initbelts {};
        class seatbeltaction {};
        class seatbeltOff {};
        class seatbeltOn {};
};

<br/> 

<b> Step 3: GO TO fn_keyhandler AND PASTE THE CODE BELOW IN ALSO MAKE SURE NO OTHER HANDLER IS CASE 48  </b>

<br/> 

//--- B KEY
    case 48: {
        if (vehicle player != player) then {
           [] spawn IRT_fnc_seatbeltaction;
        };
    };

<br/> 


<br/> 
<b> Step 4: GO TO  AND PASTE THE CODE BELOW </b>

<br/> 
<br/> 
//--- SeatBelt
[] spawn IRT_fnc_initbelts;
<br/> 

<br/> 

<b> Step 5: GO TO configuration.sqf AND PASTE THE CODE BELOW IN  </b>

<br/> 

IRT_SeatBelt = false;

## Copyright and License

Copyright (c) 2018 Ethan (XaLaForo), IRT Studios

### All code is licensed under the MIT license.

